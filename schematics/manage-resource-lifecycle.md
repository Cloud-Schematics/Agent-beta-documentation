---

copyright:
  years: 2017, 2022
lastupdated: "2022-12-02"

keywords: manage resources with schematics, schematics resource lifecycle, deploy resources with schematics, update resources with schematics, create terraform execution plan, apply terraform template

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}





# Managing resources with {{site.data.keyword.bpshort}}
{: #manage-lifecycle}

Deploy, modify, and remove {{site.data.keyword.cloud}} resources by changing the infrastructure code in your Terraform template and by using {{site.data.keyword.bplong_notm}} to apply the template in your {{site.data.keyword.cloud_notm}} account. 
{: shortdesc}

To keep your {{site.data.keyword.bplong_notm}} state file and the {{site.data.keyword.cloud_notm}} resources in your account in sync, use {{site.data.keyword.bplong_notm}} to provision, or remove your resources. 
{: important}

## Supporting features
{: #resource-features}

The following features are supported in the {{site.data.keyword.bpshort}} Workspaces resource view page.

- The resources related data are displayed in a tabular format.
- You can search for resources by using a table search.
- You can sort the resources by using a table sort.
- You can view the support of pagination.

The resources that are displayed are about Terraform resources that includes related resources and null resources.
{: note}

**The table lists the primary data of a resource.**

| Data | Description |
| --- | --- |
| Resource | The name of the resource. The resource name can have a resource controller URL that appear as a anchor link, so that you can click on the link and navigate to the resource dashboard page. If a resource does not have a resource controller URL, it appears as a plain text. The resource controller URL is derived from the Terraform state file. |
| Type | The resource type. For example, `ibm_is_vpc`, `ibm_is_subnet`. |
| Taint status | States the resource is `degraded` or `damaged`. When a resource is tainted the value displayed will be `Tainted`. If a resource is not `degraded` or `damaged`, empty value is displayed. |
| Resource group | Displays the [resource group](/docs/account?topic=account-rgs) that are used to provision your resource. |
| Tags | The [tags](/docs/account?topic=account-tag) that are attached to the resources. It can be a `user tag` or `Access management tag`. |
{: caption="{{site.data.keyword.bpshort}} resources" caption-side="bottom"}

The data that are shown in the primary data depends on your workspace status. Following are the supporting workspace state for the resource state.

| State | Description |
| -- | -- |
| `Not applied` | When your workspace state is in `Draft`, `Connecting`, or `Inactive`. In this state, your resources are yet to provision. You need to **Generate plan** and run **Apply plan** to provision the resources. |
| `Inprogress` | When your workspaces state is in `Inprogress` means your job is in progress, and you need to check after sometime. |
| `Active`| When your workspace state is in `Active` means your apply job is successful. Also you can view the resource related data, else you would see `Your plan did not generate any resource` message. |
{: caption="{{site.data.keyword.bpshort}} Workspaces status versus resource state" caption-side="bottom"}

## Deploying your resources
{: #deploy-resources}
{: ui}

Run your infrastructure code to provision, or modify your {{site.data.keyword.cloud_notm}} resources with {{site.data.keyword.bpshort}}. 
{: shortdesc}

**Before you begin**: 
- [Create a workspace from UI](/docs/schematics?topic=schematics-workspace-setup#create-workspace), [upload a workspace through CLI](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-upload), or [upload a tape archive file (`.tar`) through API](/apidocs/schematics/schematics#create-workspace) that hosts your Terraform template. 
- Make sure that you have the required [permissions](/docs/schematics?topic=schematics-access) to deploy the resources in {{site.data.keyword.cloud_notm}}. 

**To deploy your resources**: 

1. From the [workspace dashboard](https://cloud.ibm.com/schematics/workspaces){: external}, select the workspace that points to the Terraform template that you want to apply. 
   Sample templates examples are listed in [Cloud {{site.data.keyword.bpshort}}](https://github.com/Cloud-Schematics){: external} GitHub, you can use one of the template for testing. For example, [Easy multizone VPC](https://github.com/Cloud-Schematics/easy-multizone-vpc){: external}.
   {: note}

2. Select the **Settings** tab.
3. In the **Details** section, click **Pull latest** to get the latest version of your Terraform template from the linked GitHub source repository. If you provided your Terraform template by uploading a tape archive file (`.tar`), you must use the [`ibmcloud schematics workspace upload`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-upload) command to provide a new version of your template.
4. Optional: Review the variables that you set for your workspace. The values of your variables are used every time that you reference the variable in your Terraform template. Make sure that your variables use the correct values. 
5. Click **Generate plan** to create a Terraform execution plan. This action equals the `terraform plan` command. After you click this button, the workspace **Jobs** page opens and {{site.data.keyword.bpshort}} starts to compare the state of the resources that you already provisioned in your {{site.data.keyword.cloud_notm}} account with the resources that you want to provision with your Terraform template. 
6. Click **Jobs** to review the log of your execution plan. The execution plan includes a summary of {{site.data.keyword.cloud_notm}} resources that must be created, modified, or deleted to achieve the state that you described in your Terraform template. If you have syntax errors in your Terraform configuration files, you can review the error message in the log file. 
7. Review available service plans and pricing information for each of the {{site.data.keyword.cloud_notm}} resources that {{site.data.keyword.bpshort}} is about to create or change. Some services come with a limit per {{site.data.keyword.cloud_notm}} account. If you are about to reach the service limit for your account, the resource is not provisioned until you increase the service quota, or remove existing services first. 
8. When you are ready, apply your Terraform template by clicking **Apply plan**. This action equals the `terraform apply` command. After you click the button, {{site.data.keyword.bplong_notm}} starts provisioning, modifying, or deleting your {{site.data.keyword.cloud_notm}} resources based on what actions were identified in the execution plan. Depending on the type and number of resources that you want to provision or modify, this process might take couple of minutes, or even up to hours to complete. During this time, you cannot make changes to your workspace. After all updates are applied, the state of your {{site.data.keyword.cloud_notm}} resources is stored in a Terraform state file that {{site.data.keyword.bplong_notm}} uses to determine what resources exist in your {{site.data.keyword.cloud_notm}} account. 

    If you want to stop applying your Terraform template, you can use the **Stop** button. Note that all resources that are already created are not removed. If a resource is currently provisioning, {{site.data.keyword.bpshort}} waits for the provisioning to complete, and then stops the creation, update, or deletion of any other resources in your Terraform template. 
    {: note}

9. Review the job log to ensure that no errors occurred during the provisioning, modification, or deletion process. 
10. From the navigation, select **Resources** to find a summary of {{site.data.keyword.cloud_notm}} resources that are available in your {{site.data.keyword.cloud_notm}} account.

## Updating your resources
{: #update-resources}
{: ui}

To update {{site.data.keyword.cloud_notm}} resources, you must first change the infrastructure code in your Terraform template before you can run your code in {{site.data.keyword.bplong_notm}}.  
{: shortdesc}

Depending on how you change the configuration of an existing resources, {{site.data.keyword.bplong_notm}} might not be able to update your resource. Instead, {{site.data.keyword.bplong_notm}} might decide to apply the change, the resource must be removed, and a new resource must be created. If your resource must be removed, make sure that you do not interrupt a working environment, or delete data. 
{: note}

To update your resources: 

1. From the [workspace dashboard](https://cloud.ibm.com/schematics/workspaces){: external}, select the workspace that points to the Terraform template that you updated. 
2. Select the **Settings** tab.
3. In the **Details** section, click **Pull latest** to get the latest version of your Terraform template from the linked GitHub source repository. If you provided your Terraform template by uploading a tape archive file (`.tar`), you must use the [`ibmcloud schematics workspace upload`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-upload) command to provide a new version of your template.
4. If you want to change the variable values that you set when you created the workspace, change the variable values. 
5. Click **Generate plan** to create a Terraform execution plan. Note that during this time, you cannot make changes to your workspace. 
6. Click **Jobs** to review the log of your execution. The job log provides a summary of all the resources that {{site.data.keyword.bplong_notm}} is about to modify. {{site.data.keyword.bplong_notm}} might not be able to modify some of your resources, and suggest removing and re-creating the resource.
7. Click **Apply plan** to apply the new Terraform template version. Depending on the changes that you made, it might take couple of minutes or up to few hours for the template to be applied. Note that during this time, you cannot make changes to your workspace.

    If you want to stop applying your Terraform template, you can use the **Stop** button. Note that updates to resources that were already performed are not reverted. If a resource is currently updating, {{site.data.keyword.bpshort}} waits for the update to complete, and then stops the creation, update, or deletion of any other resources in your Terraform template. 
    {: note}

8. Review the job log to ensure that no errors occurred during the modification process. 
9. From the navigation, select **Resources** and verify that your resources show the updated configuration. 

## Managing drift between your cloud environment and Terraform configuration
{: #drift-report}
{: ui}

Use Terraform-native capabilities to determine the differences between the infrastructure and platform services that you provisioned in {{site.data.keyword.cloud_notm}} and the resources that you specified in your Terraform configuration files. 
{: shortdesc}

Managing deviations between the real-world state of your cloud environment and your infrastructure code, also referred to as `drift`, is a key challenge when implementing infrastructure as code. Deviations can happen for many reasons, such as: 

- You added, updated, or removed resources in your Terraform configuration file without running your infrastructure code.
- You manually added, updated, or removed {{site.data.keyword.cloud_notm}} without Terraform.
- You used other automation tools, such as scripts to manipulate the state of your {{site.data.keyword.cloud_notm}} resources.
  
**To view deviations between the resources in your {{site.data.keyword.cloud_notm}} account and your Terraform configuration:** 

1. From the [workspace dashboard](https://cloud.ibm.com/schematics/workspaces){: external}, select the workspace where you want to inspect deviations between the resources that are provisioned in your account and the resources that you defined in your Terraform configuration file. 
2. Select the **Settings** tab.
3. In the **Details** section, click **Pull latest** to get the latest version of your Terraform template from the linked GitHub source repository. If you provided your Terraform template by uploading a tape archive file (`.tar`), you must use the [`ibmcloud schematics workspace upload`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-upload) command to provide a new version of your template.
4. Review the values of your input variables and make sure that you want to create the deviation report with the values that you see. 
5. Click **Generate plan** to create a Terraform execution plan. Note that during this time, you cannot make changes to your workspace. During the creation of the Terraform execution plan, Terraform compares the required state that you described in your Terraform configuration files with the actual state of your cloud resources. If changes are found, Terraform analyzes what actions need to be performed to get your actual cloud resources to the required state. 
6. Click **Jobs** to review the log files of your execution plan. The log file provides a summary of all the resources that {{site.data.keyword.bplong_notm}} identified to achieve the state that you want. These actions can include adding, modifying, or removing resources. 
7. Optional: Apply the changes in your cloud environment by clicking **Apply plan**. 

## Reviewing resource and deployment details
{: #review-logs}
{: ui}

View the details of the {{site.data.keyword.bplong_notm}} deployments and the {{site.data.keyword.cloud_notm}} resources that you currently manage with {{site.data.keyword.bplong_notm}}.
{: shortdesc}

1. From the [workspace dashboard](https://cloud.ibm.com/schematics/workspaces){: external}, select the workspace that you want to inspect.
2. From the navigation, select **Settings** to find a summary of activities in your workspace.
3. Review the logs of previous Terraform execution plans and the plans that you applied. 
4. From the navigation, select **Resources** to review the state of the {{site.data.keyword.cloud_notm}} resources that you created with this workspace. 
5. To review who made a change to your Terraform template, go to the source repository in GitHub that is linked to your workspace, and use the built-in capabilities such as the commit history and pull requests to review changes.
6. To review events that {{site.data.keyword.bpshort}} sent to {{site.data.keyword.at_full_notm}}, see [{{site.data.keyword.at_full_notm}} events](/docs/schematics?topic=schematics-at_events). 

## Removing your resources
{: #destroy-resources}
{: ui}

To remove an {{site.data.keyword.cloud_notm}} resource that you provisioned with {{site.data.keyword.bplong_notm}}, you can either remove your resources with {{site.data.keyword.bpshort}}, delete your workspace, or remove the infrastructure code in the Terraform template. 
{: shortdesc}

Removing an {{site.data.keyword.cloud_notm}} resource cannot be undone. Make sure that you backed up your data before you remove a resource. If you choose to remove the infrastructure code, or comment out the resource in your Terraform configuration file, make sure to thoroughly review the log file of your execution plan to verify that all your resources are included in the removal.   
{: important}

**To remove your resources by deleting the infrastructure code from your Terraform template:**

1. Open the Terraform configuration file in your source repository in GitHub or on your local machine. 
2. Either remove the infrastructure code from the file, or comment out the resources that you want to remove by adding `#` to the beginning of each line. 

    **Example for commenting out a resource:**

    ```terraform
    ...
    #resource ibm_is_instance "vsi1" {
    #  name    = "${local.BASENAME}-vsi2"
    #  vpc     = ibm_is_vpc.vpc.id
    #  zone    = "${local.ZONE}"
    #  keys    = [data.ibm_is_ssh_key.ssh_key_id.id]
    #  image   = data.ibm_is_image.ubuntu.id
    #  profile = "cc1-2x4"

    #  primary_network_interface {
    #    subnet          = ibm_is_subnet.subnet1.id
    #    security_groups = [ibm_is_security_group.sg1.id]
    #  }
    #}
    ```
    {: codeblock}

3. Commit the change to your Terraform configuration file. 
4. From the [workspace dashboard](https://cloud.ibm.com/schematics/workspaces){: external}, select the workspace that points to the Terraform template that you just changed. 
5. From the navigation, select **Settings**. 
6. In the **Details** section, click **Pull latest** to get the latest version of your Terraform template from the linked GitHub source repository. If you provided your Terraform template by uploading a tape archive file (`.tar`), you must use the [`ibmcloud schematics workspace upload`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-upload) command to provide a new version of your template.
7. Click **Generate plan** to create a Terraform execution plan. The workspace **Jobs** page opens. Note that during this time, you cannot make changes to your workspace.
8. Click **Jobs** to review the log of your execution plan. The log provides a summary of all the resources that {{site.data.keyword.bplong_notm}} is about to remove. 
9. Click **Apply plan** to remove the {{site.data.keyword.cloud_notm}} resources from your account. 

    If you want to stop applying your Terraform template, you can use the **Stop** button. Note that all resources that are already removed are not re-created. If a resource is currently deleting, {{site.data.keyword.bpshort}} waits for the deletion to complete, and then stops the creation, update, or deletion of any other resources in your Terraform template. 
    {: note}

10. Review the log files to ensure that no errors occurred during the deletion process. 
11. From the navigation, select **Resources** and verify that your resources are removed. 
12. Optional: After you removed all your resources, remove your workspace. 
    1. Open the [workspace dashboard](https://cloud.ibm.com/schematics/workspaces){: external} and find the workspace that you want to remove. 
    2. Click **Actions...** tab and select **Delete workspace** option. 
    3. Type your workspace name in **Type `workspace_name` to confirm** text box. 
    4. Click **Delete** button.

**To remove your resources from the {{site.data.keyword.bpshort}} console:**

1. From the [workspace dashboard](https://cloud.ibm.com/schematics/workspaces){: external}, find the workspace that includes the resources that you want to delete. 
2. Click **Actions...** tab and select **Destroy resources** option. 
3. Type your workspace name in **Type `workspace_name` to confirm** text box. Note that destroying resources will terminate the resource in your workspace. This action cannot be undone.
4. Click **Destroy** button.
5. From the navigation, select **Jobs** to review the logs for your resource deletion. Ensure that no errors occurred during the deletion process. 
6. From the navigation, select **Resources** and verify that your resources are removed. 

After the deletion of your resources is complete, the {{site.data.keyword.bpshort}} Workspaces is removed. 


## Deploying your resources through CLI
{: #deploy-resources-cli}
{: cli}

Run your infrastructure code to provision, or modify your {{site.data.keyword.cloud_notm}} resources with {{site.data.keyword.bpshort}}. 
{: shortdesc}

**Before you begin**: 
- [Create a workspace from CLI](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-new), [upload a workspace through CLI](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-update). 
- Make sure that you have the required [permissions](/docs/schematics?topic=schematics-access) to deploy the resources in {{site.data.keyword.cloud_notm}}. 

**To deploy your resources**: 

1. From your [command line interface](/docs/schematics?topic=schematics-setup-cli){: external} set up your CLI and {{site.data.keyword.bpshort}} plug-in.
2. List your workspace by using [`ibmcloud schematics workspace list`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-list) command.
3. Get your workspace by using [`ibmcloud schematics workspace get`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-get) command.
4. If you provided your Terraform template by uploading a tape archive file (`.tar`), you must use the [`ibmcloud schematics workspace upload`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-upload) command.
5. Create Terraform execution plan, by using [`ibmcloud schematics plan`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-plan) command.
6. Use your workspace ID to retrieve the logs by using [`ibmcloud schematics logs`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-logs) command.
7. When you are ready, execute [`ibmcloud schematics apply`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-apply) command.

    If you want to stop applying your Terraform template, you can use the [`ibmcloud schematics job delete`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-delete-job) command. Note that all resources that are already created are not removed. If a resource is currently provisioning, {{site.data.keyword.bpshort}} waits for the provisioning to complete, and then stops the creation, update, or deletion of any other resources in your Terraform template. 
    {: note}

8. Review the job log to ensure that no errors occurred during the provisioning, modification, or deletion process. 
9. From the [navigation pane](https://cloud.ibm.com/resources), select **Resources** to find a summary of {{site.data.keyword.cloud_notm}} resources that are available in your {{site.data.keyword.cloud_notm}} account.

## Updating your resources through CLI
{: #update-resources-cli}
{: cli}

To update {{site.data.keyword.cloud_notm}} resources, you must first change the infrastructure code in your Terraform template before you can run your code in {{site.data.keyword.bplong_notm}}.  
{: shortdesc}

Depending on how you change the configuration of an existing resources, {{site.data.keyword.bplong_notm}} might not be able to update your resource. Instead, {{site.data.keyword.bplong_notm}} might decide to apply the change, the resource must be removed, and a new resource must be created. If your resource must be removed, make sure that you do not interrupt a working environment, or delete data. 
{: note}

To update your resources: 

1. From your [command line interface](/docs/schematics?topic=schematics-setup-cli){: external} set up your CLI and {{site.data.keyword.bpshort}} plug-in.
2. List your workspace by using [`ibmcloud schematics workspace list`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-list) command.
3. Get your workspace by using [`ibmcloud schematics workspace get`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-get) command.
4. If you provided your Terraform template by uploading a tape archive file (`.tar`), you must use the [`ibmcloud schematics workspace upload`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-upload) command.
5. Create Terraform execution plan, by using [`ibmcloud schematics plan`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-plan) command.
6. Use your workspace ID to retrieve the logs by using [`ibmcloud schematics logs`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-logs) command.
7. When you are ready, execute [`ibmcloud schematics apply`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-apply) command.

    If you want to stop applying your Terraform template, you can use the [`ibmcloud schematics job delete`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-delete-job) command. Note that all resources that are already created are not removed. If a resource is currently provisioning, {{site.data.keyword.bpshort}} waits for the provisioning to complete, and then stops the creation, update, or deletion of any other resources in your Terraform template. 
    {: note}

8. Review the job log to ensure that no errors occurred during the provisioning, modification, or deletion process. 
9. From the [navigation pane](https://cloud.ibm.com/resources), select **Resources** to find a summary of {{site.data.keyword.cloud_notm}} resources that are available in your {{site.data.keyword.cloud_notm}} account.

## Managing drift between your cloud environment and Terraform configuration through CLI
{: #drift-report-cli}
{: cli}

Use Terraform-native capabilities to determine the differences between the infrastructure and platform services that you provisioned in {{site.data.keyword.cloud_notm}} and the resources that you specified in your Terraform configuration files. 
{: shortdesc}

Managing deviations between the real-world state of your cloud environment and your infrastructure code, also referred to as `drift`, is a key challenge when implementing infrastructure as code. Deviations can happen for many reasons, such as: 

- You added, updated, or removed resources in your Terraform configuration file without running your infrastructure code.
- You manually added, updated, or removed {{site.data.keyword.cloud_notm}} without Terraform.
- You used other automation tools, such as scripts to manipulate the state of your {{site.data.keyword.cloud_notm}} resources.
  
**To view deviations between the resources in your {{site.data.keyword.cloud_notm}} account and your Terraform configuration:** 

1. From your [command line interface](/docs/schematics?topic=schematics-setup-cli){: external} set up your CLI and {{site.data.keyword.bpshort}} plug-in.
2. List your workspace by using [`ibmcloud schematics workspace list`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-list) command.
3. Get your workspace by using [`ibmcloud schematics workspace get`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-get) command.
4. If you provided your Terraform template by uploading a tape archive file (`.tar`), you must use the [`ibmcloud schematics workspace upload`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-upload) command.
5. Create Terraform execution plan, by using [`ibmcloud schematics plan`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-plan) command.
6. Use your workspace ID to retrieve the logs by using [`ibmcloud schematics logs`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-logs) command.
7. When you are ready, execute [`ibmcloud schematics apply`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-apply) command.

## Reviewing resource and deployment details through CLI
{: #review-logs-cli}
{: cli}

View the details of the {{site.data.keyword.bplong_notm}} deployments and the {{site.data.keyword.cloud_notm}} resources that you currently manage with {{site.data.keyword.bplong_notm}}.
{: shortdesc}

1. From your [command line interface](/docs/schematics?topic=schematics-setup-cli){: external} set up your CLI and {{site.data.keyword.bpshort}} plug-in.
2. From the [navigation pane](https://cloud.ibm.com/resources), select **Resources** to find a summary of {{site.data.keyword.cloud_notm}} resources that are available in your {{site.data.keyword.cloud_notm}} account.
3. To review who made a change to your Terraform template, go to the source repository in GitHub that is linked to your workspace, and use the built-in capabilities such as the commit history and pull requests to review changes.
4. To review events that {{site.data.keyword.bpshort}} sent to {{site.data.keyword.at_full_notm}}, see [{{site.data.keyword.at_full_notm}} events](/docs/schematics?topic=schematics-at_events). 

## Removing your resources through CLI
{: #destroy-resources-cli}
{: cli}

To remove an {{site.data.keyword.cloud_notm}} resource that you provisioned with {{site.data.keyword.bplong_notm}}, you can either remove your resources with {{site.data.keyword.bpshort}}, delete your workspace, or remove the infrastructure code in the Terraform template. 
{: shortdesc}

Removing an {{site.data.keyword.cloud_notm}} resource cannot be undone. Make sure that you backed up your data before you remove a resource. If you choose to remove the infrastructure code, or comment out the resource in your Terraform configuration file, make sure to thoroughly review the log file of your execution plan to verify that all your resources are included in the removal.   
{: important}

**To remove your resources by deleting the infrastructure code from your Terraform template:**

1. Open the Terraform configuration file in your source repository in GitHub or on your local machine. 
2. Either remove the infrastructure code from the file, or comment out the resources that you want to remove by adding `#` to the beginning of each line. 

    **Example for commenting out a resource:**

    ```terraform
    ...
    #resource ibm_is_instance "vsi1" {
    #  name    = "${local.BASENAME}-vsi2"
    #  vpc     = ibm_is_vpc.vpc.id
    #  zone    = "${local.ZONE}"
    #  keys    = [data.ibm_is_ssh_key.ssh_key_id.id]
    #  image   = data.ibm_is_image.ubuntu.id
    #  profile = "cc1-2x4"

    #  primary_network_interface {
    #    subnet          = ibm_is_subnet.subnet1.id
    #    security_groups = [ibm_is_security_group.sg1.id]
    #  }
    #}
    ```
    {: codeblock}

3. Commit the change to your Terraform configuration file. 
4. From your [command line interface](/docs/schematics?topic=schematics-setup-cli){: external} set up your CLI and {{site.data.keyword.bpshort}} plug-in.
5. Get your workspace by using [`ibmcloud schematics workspace get`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-get) command.
6. If you provided your Terraform template by uploading a tape archive file (`.tar`), you must use the [`ibmcloud schematics workspace upload`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-upload) command.
7. Create Terraform execution plan, by using [`ibmcloud schematics plan`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-plan) command.
8. Use your workspace ID to retrieve the logs by using [`ibmcloud schematics logs`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-logs) command.
9. When you are ready, execute [`ibmcloud schematics apply`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-apply) command.

    If you want to stop applying your Terraform template, you can use the [`ibmcloud schematics job delete`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-delete-job) command. Note that all resources that are already created are not removed. If a resource is currently provisioning, {{site.data.keyword.bpshort}} waits for the provisioning to complete, and then stops the creation, update, or deletion of any other resources in your Terraform template. 
    {: note}

10. Review the job log to ensure that no errors occurred during the provisioning, modification, or deletion process. 
11. From the [navigation pane](https://cloud.ibm.com/resources), select **Resources** to find a summary of {{site.data.keyword.cloud_notm}} resources that are available in your {{site.data.keyword.cloud_notm}} account.
12. Optional: After you removed all your resources, remove your workspace by using [`ibmcloud schematics workspace delete`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-delete) command.


