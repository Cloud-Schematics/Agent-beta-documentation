---

copyright:
  years: 2017, 2022
lastupdated: "2022-06-13"

keywords: schematics remote agents, remote agents, set up remote agents

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}

# Deploying an {{site.data.keyword.bpshort}} agent 
{: #agents-setup}

The {{site.data.keyword.bpshort}} agent feature is currently in beta and should not be used for production workloads.
{: beta}

The {{site.data.keyword.bpshort}} agent is deployed in your {{site.data.keyword.cloud}} account and is configured to connect to your {{site.data.keyword.bpshort}} service instance. You can follow these steps to use a Terraform automation to provision the Kubernetes cluster and to install an Agent in the cluster.
{: shortdesc}

## Prerequisites
{: #agents-infra-prereq}

Before you begin, complete the following prerequisites.

- Your {{site.data.keyword.cloud_notm}} account must be a paid account, and have the permissions to provision VPC, {{site.data.keyword.containerlong_notm}} cluster, {{site.data.keyword.cos_full}}, and logging service in a predefined resource group.

## Expected outcome
{: #agents-infra-outcome}

On completion, you can view the following resources provisioned in your {{site.data.keyword.cloud_notm}} account, in the specified region.
- `cos_instance`, `cos_key`, `cos_bucket`
- `logdna_instance`, `logdna_key`
- `VPC infrastructure`, `public_gateways`, `subnets`
- `vpc_kubernetes_cluster`
- `k8s_deployments` such as `jobrunner`, `terraform-job`, and `logdna-agent` in the respective namespaces.
- `cos_instance`, `cos_key`, `cos_bucket`
- `logdna_instance`, `logdna_key`
- `VPC infrastructure`, `public_gateways`, `subnets`
- `vpc_kubernetes_cluster`
- `k8s_deployments` such as `jobrunner`, `terraform-job`, and `logdna-agent` in the respective namespaces. 

## Step 1: Provisioning the cluster infrastructure for an Agent
{: #agent-infra-step1}

1. Login to [{{site.data.keyword.cloud_notm}}](https://cloud.ibm.com/)
2. Navigate to **Schematics** > **Workspaces** > [**Create**](https://cloud.ibm.com/schematics/workspaces/create){: external}
    - Specify your template - https://github.ibm.com/schematics-solution/schematics-remote-agents/tree/docs/templates/infrastructure
    - Select Terraform Version - `terraform_v1.0`.
    - Click `Next`.
    - Enter a Workspace Name - `schematics-agent-infrastructure`.
    - Click `Create`.
3. On successsful creation of the `schematics-agent-infrastructure` workspace, open the **Settings** page, to review and edit the following variables.
    | Input variable  | Description |
    |--|--|
    | `ibmcloud_api_key` | The API key used to deploy the Agent infrastructure resources.|
    | `agent_region`| The region to provision your Agent infrastructure. For example, **eu**.|
    | `Agent_resource_group` | Name of the resource group used to provision the Agent infrastructure. For example, **Default** |
    | `cluster_size` | The flavor and size of the {{site.data.keyword.containerlong_notm}} cluster used to deploy an Agent. It can be one or **extra-large**, **large**, **medium**, or **small**. For example, **medium**| 
    | `tags` | List of tags to add to the Agent infrastructure resources, such as `test`, `prod`.|
    {: caption="{{site.data.keyword.bpshort}} agent infrastructure input" caption-side="bottom"}

4. Run {{site.data.keyword.bpshort}} Workspace plan on the `schematics-agent-infrastructure` workspace to view the results in the Job logs, without an error.
5. Run {{site.data.keyword.bpshort}} Workspace apply on the `schematics-agent-infrastructure` Workspace page to view the results in the Job logs. Now you can view the Workspace status as `ACTIVE`. 

## Step 2: Reviewing an Agent service
{: #agent-infra-step2}

1.	Navigate to the [{{site.data.keyword.cloud_notm}} Resources](https://cloud.ibm.com/resources){: external}.
2.	Filter by tags `schematics:<workspace_ID>`
3.	Verify the following resources
    - **VPC Infrastructure** > `remoteagent-vpc` the status as **Available**.
    - **Services and Software** > `remoteagent-logdna` the status as **Active**.
    - **Storage** > `remoteagent-cos` the status as **Active**.
    - **Clusters** > `remoteagent-iks` the status as **Normal**.

## Step 3: Deploying an Agent service
{: #agent-infra-step3}

1. Login to [{{site.data.keyword.cloud_notm}}](https://cloud.ibm.com/)
2. Navigate to **Schematics** > **Workspaces** > [**Create**](https://cloud.ibm.com/schematics/workspaces/create){: external}
      - Select existing template - https://github.ibm.com/schematics-solution/schematics-remote-agents/tree/master/templates/service
      - Select Terraform Version - `terraform_v1.0`.
      - Click `Next`.
      - Enter a Workspace Name - `schematics-agent-service`.
      - Click `Create`.
3. On successful creation of `schematics-agent-service` Workspace, open the **Settings** page to review and edit the following input variables.

    | Input variables | Description   | 
    |----|----|
    | `cluster_id` | The {{site.data.keyword.containerlong_notm}} cluster ID provisioned by an Agent infrastructure Workspace. |
    | `agent_resource_group` | The resource group name that are used in an Agent infrastructure. |
    | `agent_region` | Region used to setup the Agent infrastructure. |
    | `agent_registry_password` | The Api key used to pull {{site.data.keyword.bpshort}} agent container images. Check as `Sensitive`. |
    | `logdna_ingestion_key` | The LogDNA ingestion key from the Agent infrastructure workspace Check as `Sensitive`. |
    {: caption="{{site.data.keyword.bpshort}} remote service input" caption-side="bottom"}

4. Run {{site.data.keyword.bpshort}} Workspace plan on the `schematics-agent-service` Workspace to view the results in the Job logs, without any error.
5.	Run {{site.data.keyword.bpshort}} Workspace apply on the `schematics-agent-service` Workspace page, to view the results in the Job logs. Now you can view the Workspace status as `ACTIVE`.

## Step 4: Review the cluster infrastructure for an Agent
{: #agent-runtime-step3}

1. Navigate to the target [{{site.data.keyword.cloud_notm}} clusters page](https://cloud.ibm.com/kubernetes/clusters/<target_iks_cluster_ID>){: external}.
2. Click **Kubernetes Dashboard** to view the Kubernetes dashboard.
3. Verify the Kubernetes resources are created from the Kubernetes dashboard.
    - Pods (All namespaces)
        - `job1.0` pods (3 instances - one on each worker node) > Status: `Running`
        - `jobrunner` pod (1 instance) > Status: `Running`
        - `logdna-agent` pods (3 instances - one on each worker node) > Status: `Running`


## Uninstall the {{site.data.keyword.bpshort}} agent
{: #uninstall-agent}

The {{site.data.keyword.bpshort}} agent that are deployed in your {{site.data.keyword.cloud}} account can be uninstalled from your {{site.data.keyword.bpshort}} service instance by following the given cleanup steps.
{: shortdesc}

### Cleanup the agent infrastructure
{: #cleanup-agent-infra}

1. From the [{{site.data.keyword.bpshort}} Workspace](https://cloud.ibm.com/schematics/workspaces/<workspace_id_schematics-agent-infrastructure>) page, open your workspace.
2. Select **Actions** > **Destroy resources** > **Type the name of workspace** > click **Destroy**.
3. From the Workspace `schematics-agent-infrastructure` page > **Jobs** tab
    - Wait for Terraform destroy job to complete. It takes about 10 to 15 minutes.
    - From the Workspace `schematics-agent-infrastructure` page, click **Jobs** to view a message as `Destroy successful`. 
4. Select **Actions** > **Delete workspace** > **Type the name of workspace** > click **Delete**.

### Cleanup the agent service
{: #cleanup-agent-service}

1. From the [{{site.data.keyword.bpshort}} Workspace](https://cloud.ibm.com/schematics/workspaces/<workspace_id_schematics-agent-service-workspace>) page, open your workspace.
2. Select **Actions** > **Destroy resources** > **Type the name of workspace** > click **Destroy**.
3. From the Workspace `schematics-agent-service-workspace` page > **Jobs** tab
    - Wait for Terraform destroy job to complete. It takes about 10 to 15 minutes.
    - From the Workspace `schematics-agent-service-workspace` page, click **Jobs** to view a message as `Destroy successful`.
4. Select **Actions** > **Delete workspace** > **Type the name of workspace** > click **Delete**.

