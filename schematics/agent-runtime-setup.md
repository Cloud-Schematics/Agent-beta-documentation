---

copyright:
  years: 2017, 2022
lastupdated: "2022-06-13"

keywords: remote agent runtime service, runtime service workspace, schematics agent runtime service

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}

# Setting an agent runtime service
{: #agent-runtime-svc}

The {{site.data.keyword.bpshort}} agent feature is currently in beta and should not be used for production workloads.
{: beta}

{{site.data.keyword.bpshort}} agent is an experimental feature that describes the steps to deploy the {{site.data.keyword.bpshort}} agents created by the [`{{site.data.keyword.bpshort}} agent infrastructure workspace`](/docs/schematics?topic=schematics-agents-setup) set up. 
{: shortdesc}

## Prerequisites
{: #agents-runtime-prereq}

Before you begin, complete the following prerequisites.

- Your {{site.data.keyword.bpshort}} agents infrastructure workspace must be in `ACTIVE` status. For more information, refer to, [`{{site.data.keyword.bpshort}} agent infrastructure workspace`](/docs/schematics?topic=schematics-agents-setup).
- You must have the permissions to deploy microservices on the {{site.data.keyword.containerlong}} cluster.
- Make sure of the resource group ID in which the infrastructre resources were provisioned. To find the resource group ID: 
    - Navigate to your [resource groups](https://cloud.ibm.com/account/resource-groups){: external}.
    - From the resource groups page, you will observe the ID for the cluster's resource group name.
- Make a note of the `cluster_id` for the IKS cluster provisioned. The agents gets deployed onto this cluster. To find the cluster ID:
    - Navigate to [IKS cluster](https://cloud.ibm.com/kubernetes/clusters) and click on the target cluster. For example, `remoteagent-iks`. 
    - In the cluster's **Details** section, you will observe the `Cluster ID` value. In the same **Details** page. Make a note of the `Resource Group` name. 
- Make a note of the LogDNA ingestion key from the LogDNA instance provisioned. To find the LogDNA ingestion key:
    - Navigate to [Logging page](https://cloud.ibm.com/observe/logging) and click on the target Logging instance. For example, `remoteagent-logdna`. 
    - In the Logging instance **Details Overview** tab, select **Actions** dropdown > **View Key** > **Ingestion Key for remoteagent-logdna**.
- Make a note of your Account ID and API Key that are associated with this account in `https://test.cloud.ibm.com`.
    - To find your stage account API Key. Navigate to [API keys](https://test.cloud.ibm.com/iam/apikeys) > **My Cloud API Keys** > **View**.
    - To find your stage account ID. Navigate to [Account](https://test.cloud.ibm.com/account/settings) > **Account ID**.
- Access to {{site.data.keyword.cloud_notm}} production account is sufficient to access the {{site.data.keyword.bpshort}} agent container images such as jobrunner and job12 from the {{site.data.keyword.registryshort}} `icr.io/schematics-remote`.


## Expected outcome
{: #agents-runtime-outcome}

When the {{site.data.keyword.bpshort}} agent infrastructure set up is completed. You can see following {{site.data.keyword.bpshort}} agent runtime resources are provisioned in your {{site.data.keyword.containerlong_notm}} cluster.

1. namespaces
   - schematics-job-runtime
   - schematics-runtime
   - schematics-ibm-observe
2. deployments
   - jobrunner (schematics-job-runtime namespace)
   - job12 (schematics-runtime namespace)
3. daemonsets
   - logdna-agent (schematics-ibm-observe namespace)
4. secrets
   - schematics-jobrunner-image-secret (schematics-job-runtime namespace)
   - schematics-job12-image-secret (schematics-runtime namespace)
   - logdna-agent-token (schematics-ibm-observe namespace)
5. configmaps
   - schematics-jobrunner-config (schematics-job-runtime namespace)
   - schematics-job12-config (schematics-runtime namespace)
   - schematics-logdna-agent-config (schematics-ibm-observe namespace)
6. services
   - job-runner-loadbalancer (schematics-job-runtime namespace)
   - job-service-12-clusterip (schematics-runtime namespace)
7. serviceaccount
   - logdna-agent (schematics-ibm-observe namespace)
8. cluster role and bindings
   - logdna-agent (schematics-ibm-observe namespace)

## Step 1: Creating a {{site.data.keyword.bpshort}} agents runtime service workspace
{: #agent-runtime-step1}

1. Login to [{{site.data.keyword.cloud_notm}}](https://cloud.ibm.com/)
2. Navigate to **Schematics** > **Workspaces** > [**Create**](https://cloud.ibm.com/schematics/workspaces/create){: external}
      - Select existing template - https://github.ibm.com/schematics-solution/schematics-remote-agents/tree/master/templates/service
      - Select Terraform Version - `terraform_v0.13`.
      - Click `Next`.
      - Enter a Workspace Name - `schematics-remote-service-workspace`.
      - Click `Next`.
      - Click `Create`.
      - You will be redirected to the Workspace `schematics-remote-service-workspace` page.
3. From the workspace `schematics-remote-service-workspace` page.
      - Navigate to the **Jobs** to view a message `Workspace creation successful`. 
      - Note that the workspace status is in `INACTIVE` status.
4. From the workspace `schematics-remote-service-workspace` page.
      - Navigate to the **Settings** tab to edit the input variables as shown in the table.

        | Input variables | Description   | Example |
        |----|----|---|
        | `user_cluster_id` | Enter the IKS Cluster ID created as part of the agent infrastructure workspace. |   |
        | `user_resource_group_id` | Enter the resource group ID where the IKS Cluster is provisioned. |   |
        | `registry_password`    | Enter your production `ibmcloud api key` to pull {{site.data.keyword.bpshort}} agent images and mark as `Sensitive`. |  |
        | `LOGDNA_AGENT_KEY` | Enter the ingestion key of the LogDNA instance that was created as part of agent infrastructure workspace and mark as `Sensitive`. |  |
        | `JR_SCHEMATICSENDPOINT` | Enter the target {{site.data.keyword.bpshort}} API endpoint. <br/> Initially, target the **{{site.data.keyword.bpshort}} atage API**, override with `https://us.schematics.test.cloud.ibm.com` <br/> For the {{site.data.keyword.bpshort}} agent feature in production, internally it gets switched to {{site.data.keyword.bpshort}} production private CSE endpoint. | `https://private-us-south.schematics.test.cloud.ibm.com` |
        | `JR_APIKEY` | Enter your {{site.data.keyword.cloud_notm}} API key and mark this as `Sensitive`. |  |
        | `JR_ACCOUNTID` | Enter your {{site.data.keyword.bpshort}} account ID. |  | 
        | `JR_REGION` | Enter the target region to deploy runtime services. **Note** The region must be same as IKS cluster region. |  |
        | `JOB_ENVIRONMENT` | This is set to default `stage` value. | `stage` |
        | `JOB_CMMODULESMACHINE` | This is set to default stage global catalog endpoint. | `cm.globalcatalog.cloud.test.ibm.com` |
        {: caption="{{site.data.keyword.bpshort}} agent runtime service workspace input" caption-side="top"}

## Step 2: Provisioning the {{site.data.keyword.bpshort}} agents runtime service
{: #agent-runtime-step2}

1. From the Workspace `schematics-agent-service-workspace` page, run {{site.data.keyword.bpshort}} workspace plan.
    - Click `Generate Plan` button from the top right corner of the page
    - Open the **Jobs** to view the message as `Generate plan successful. 18 resources to add`.
2. From the Workspace `schematics-agent-service-workspace` page, run {{site.data.keyword.bpshort}} workspace apply.
    - Click `Apply Plan` button from the top right corner of the page.
    - Open the **Jobs** to view the message as `Wait for terraform apply job to complete`. 
       It will take about 10 to 15 minutes.
       {: note}

    - Review the **Jobs** to view the message `Apply plan successful` 
3. From the Workspace `schematics-agent-service-workspace` settings page, the Workspace status will now be in `ACTIVE` status.

## Step 3: Review the provisioned {{site.data.keyword.bpshort}} agents runtime service
{: #agent-runtime-step3}

1. Navigate to the target [{{site.data.keyword.cloud_notm}} clusters page](https://cloud.ibm.com/kubernetes/clusters/<target_iks_cluster_ID>){: external}.
2. Click on **Kubernetes Dashboard** that redirects to the Kubernetes dashboard.
3. Verify the Kubernetes resources are created from the Kubernetes dashboard.
    - Pods (All namespaces)
    - job12 pods (3 instances - one on each worker node) > Status: `Running`
    - jobrunner pod (1 instance) > Status: `Running`
    - logdna-agent pods (3 instances - one on each worker node) > Status: `Running`
    - Service (All namespaces)
    - job-service12-clusterip
    - job-runner-loadbalancer
    - Config Maps (All namespaces)
        - schematics-job12-config
        - schematics-jobrunner-config
        - schematics-logdna-agent-config

## Cleanup the Remote Agents Runtime Services
{: #agents-runtime-cleanup}

Follow the given steps to cleanup the Remote Agents Runtime Services.
1. From the [{{site.data.keyword.bpshort}} Workspace](https://cloud.ibm.com/schematics/workspaces/<workspace_id_schematics-remote-service-workspace>) page, open your workspace.
2. Select **Actions** > **Destroy resources** > **Type the name of workspace** > click **Destroy**.
3. From the Workspace `schematics-remote-service-workspace` page > **Jobs** tab
    - Wait for Terraform destroy job to complete. It takes about 10 to 15 minutes.
    - From the Workspace `schematics-remote-service-workspace` page, click **Jobs** to view a message as `Destroy successful`. 
     The Workspace status will now be in `INACTIVE` status.
     {: note}

4. Select **Actions** > **Delete workspace** > **Type the name of workspace** > click **Delete**.

