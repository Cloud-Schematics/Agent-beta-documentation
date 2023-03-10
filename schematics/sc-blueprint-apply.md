---

copyright:
  years: 2017, 2022
lastupdated: "2022-12-22"

keywords: blueprint apply, apply blueprint, blueprint

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}

{{site.data.keyword.bpshort}} Blueprints is a [beta feature](/docs/schematics?topic=schematics-bp-beta-limitations) that is available for evaluation and testing purposes. It is not intended for production usage. Refer to the list of [limitations](/docs/schematics?topic=schematics-bp-beta-limitations) for the beta release.
{: beta}

# Apply blueprint config changes to an environment
{: #apply-blueprint}

Blueprint run apply is the second step to create, or update resources in a blueprint environment. This step runs the IaC automation code for each module. For each module, {{site.data.keyword.bpshort}} runs a Terraform Apply to create or configure the cloud resources defined by the Terraform module code. 
{: shortdesc}

## Running a blueprint apply through CLI  
{: #apply-blueprint-cli}
{: cli}

To deploy your blueprint environment through CLI, use the `ibmcloud schematics blueprint run apply` command. 
{: shortdesc}

Before your begin

- Install and log in to the [{{site.data.keyword.cloud_notm}} CLI](/docs/schematics?topic=schematics-setup-cli#install-schematics-cli).

The following command executes a `blueprint run apply` operation for the environment with the ID `eu-de.BLUEPRINT.Blueprint-Basic-Example.21735936`

For all the blueprint commands, syntax, and detailed option flags, refer to, [blueprint commands](/docs/schematics?topic=schematics-schematics-cli-reference#blueprints-cmd).
{: important}

Syntax

```sh
ibmcloud schematics blueprint run apply --id Blueprint_Basic.eaB.5cd9
```
{: pre}

On successful completion, the apply command returns `fullfilment_success`. 

### Verify blueprint run apply success 
{: #bp-verify-apply-cli}

Verify that the blueprint configuration change has been applied successfully. When you apply the configuration from CLI, the command displays the details of the modules being applied, and a continuously updating status of the progress of the {{site.data.keyword.bpshort}} jobs that run the IaC automation code. The command returns on completion.

```text
Modules to be applied
SNO Type Name Status
1 terraform basic-resource-group INACTIVE
2 terraform basic-cos-storage INACTIVE

Blueprint job running us-east.JOB.Blueprint_Basic.e4081308 
Waiting:0 Draft:0 Connecting:0 In Progress:0 Inactive:0 Active:2
Failed:0
Type Name Status Job ID
Blueprint Blueprint_Basic FULFILMENT_SUCCESS useast.JOB.Blueprint_Basic.e4081308
terraform basic-resource-group ACTIVE
terraform basic-cos-storage ACTIVE

Blueprint ID Blueprint_Basic.eaB.5cd9 fulfilment_success at 2022-08-03
21:24:26
OK
```
{: screen}

On successful completion the Apply command returns `fullfilment_success`.  

If the operation fails, refer to the [troubleshooting](/docs/schematics?topic=schematics-bp-apply-fails) section.

## Generate and apply blueprint environment through UI 
{: #apply-blueprint-ui}
{: ui}

You can follow these steps to generate a plan and apply a blueprint using {{site.data.keyword.cloud_notm}} console.

1. Log in to [{{site.data.keyword.cloud_notm}}](https://cloud.ibm.com/){: external}.
2. Click **Schematics** > **Blueprints**.
3. Click your blueprint that is listed in the [Blueprints dashboard](https://cloud.ibm.com/schematics/blueprints){: external} 
4. Click **Generate plan** to initialize the modules that are defined in the blueprint template
    
    Generate plan execution can take few a minutes to execute. Once generated check if the plan is correct. You can see the **Resource summary**, and **Jobs history** that displays the `blueprint_create_init` and the respective module job details. If **Generate plan** fails, review the job logs to identify the cause of the failure. As required to resolve the failure, modify the template and update the blueprint configuration with the revised template and any input values. Then re-run Generate Plan.
    {: note}

5. Click **Apply plan** to provision the resources configured in your modules. You can observe the `In progress` status.
    
    The apply plan execution takes a few minutes based on the resources. The execution jobs show the history of all blueprint, module activities, and the logs of the jobs. If **Apply plan** fails, review the module job logs for information relating to the Terraform execution errors. As required to resolve the failure, modify the template and update the blueprint configuration with the revised template and any input values. Then re-run Apply Plan.
    {: note}

### Verify blueprint apply operation through UI 
{: #bp-verify-apply-ui}

You can follow these steps to verify the {{site.data.keyword.bpshort}} Blueprints by using {{site.data.keyword.cloud_notm}} console.

1. From the [Blueprints dashboard](https://cloud.ibm.com/schematics/blueprints){: external}. Click your blueprint name to view the blueprint details.
2. Click **Overview** to view the blueprint summary, that includes `Modules status`, `Variables summary`, `Blueprint Details` and `Recent Job runs` of your blueprint. 
    - Optional: From the **Modules status** card, Click **View details** to navigate to the module details page.  
    - Optional: From **Variables summary** card, Click **View details** to navigate to the variable summary page.
3. Click **Modules** tab to see the list of blueprint modules and their current status. 
    - Optional: Click **Show details** to view more details about the blueprint module definition. 
    - Optional: Click **Name** that will take you to the modules related Schematics `Workspace` page. 
4. Click **Resources** tab to view the list of resources provisioned by the blueprint.
5. Click **Variables** tab to view the blueprint **Inputs** and **Outputs** variables and values. Optional: on this page you can edit the input variable values and save. 
6. Click **Jobs history** tab view the job logs of the blueprint and module jobs.
7. Click **Settings** tab to view and edit the configuration settings of the blueprint.

## Applying a blueprint using the API 
{: #apply-blueprint-api}
{: api}

Follow the [steps](/docs/schematics?topic=schematics-setup-api#cs_api) to retrieve your IAM access token and authenticate with {{site.data.keyword.bplong_notm}} by using the API. For more information, about Blueprint update, refer to, [Installing Blueprint](/apidocs/schematics/schematics#create-blueprint) by using API.

Blueprint installation API runs `blueprint_create_init`, and `blueprint_install` `APIs`, jobs to perform the create and install the modules using Blueprint operations.
{: important}

Create Blueprint Job Example:

```json
POST /v2/jobs HTTP/1.1
Host: schematics.cloud.ibm.com
Content-Type: application/json
Authorization: Bearer <auth_token> 
refresh_token: <refresh_token>

{
    "command_name": "blueprint_create_init",
    "command_object": "blueprint",
    "command_object_id": "Blueprint-Basic-Test.eaB.bbb9"
}
```
{: pre}

Install Blueprint Job Example:

```json
POST /v2/jobs HTTP/1.1
Host: schematics.cloud.ibm.com
Content-Type: application/json
Authorization: Bearer <auth_token> 
refresh_token: <refresh_token>

{
    "command_name": "blueprint_install",
    "command_object": "blueprint",
    "command_object_id": "Blueprint-Basic-Test.eaB.bbb9"
}
```
{: pre}

### Verify Blueprint apply job through API 
{: #bp-verify-apply-api}

Here the steps to verify the result of the blueprint apply job.
{: shortdesc}

Output

```text
{
    "command_object": "blueprint",
    "command_object_id": "Blueprint-Basic-Test-API.soB.347a",
    "command_name": "blueprint_create_init",
    "id": "us-south.JOB.Blueprint-Basic-Test-API.6a5ebf46",
    "name": "JOB.Blueprint-Basic-Test-API.blueprint_create_init.1669214059468",
    "description": "Deploys a simple two module blueprint",
    "location": "us-south",
    "resource_group": "aac37f57b20142dba1a435c70aeb12df",
    "submitted_at": "2022-11-23T14:34:19.468396362Z",
    "submitted_by": "test@in.ibm.com",
    "start_at": "2022-11-23T14:34:19.468393302Z",
    "end_at": "0001-01-01T00:00:00Z",
    "status": {
        "workspace_job_status": {
            "flow_status": {
                "updated_at": "0001-01-01T00:00:00Z"
            },
            "updated_at": "0001-01-01T00:00:00Z"
        },
        "action_job_status": {
            "action_name": "Blueprint Basic Test API",
            "status_code": "job_pending",
            "status_message": "Job created and pending to start",
            "updated_at": "2022-11-23T14:34:19.468399159Z"
        },
        "system_job_status": {
            "updated_at": "0001-01-01T00:00:00Z"
        },
        "flow_job_status": {
            "updated_at": "0001-01-01T00:00:00Z"
        }
    },
    "data": {
        "job_type": "",
        "workspace_job_data": {
            "updated_at": "0001-01-01T00:00:00Z"
        },
        "action_job_data": {
            "updated_at": "0001-01-01T00:00:00Z",
            "inventory_record": {
                "created_at": "0001-01-01T00:00:00Z",
                "updated_at": "0001-01-01T00:00:00Z"
            }
        },
        "system_job_data": {
            "updated_at": "0001-01-01T00:00:00Z"
        },
        "flow_job_data": {
            "workitems": [
                {
                    "command_object_name": "basic-resource-group",
                    "source": {
                        "source_type": "git_hub",
                        "git": {
                            "git_repo_url": "https://github.com/Cloud-Schematics/blueprint-example-modules/tree/main/IBM-DefaultResourceGroup",
                            "git_branch": "main"
                        },
                        "catalog": {},
                        "cos_bucket": {}
                    },
                    "outputs": [
                        {
                            "name": "resource_group_name",
                            "metadata": {}
                        },
                        {
                            "name": "resource_group_id",
                            "metadata": {}
                        }
                    ],
                    "last_job": {},
                    "updated_at": "0001-01-01T00:00:00Z"
                },
                {
                    "command_object_name": "basic-cos-storage",
                    "source": {
                        "source_type": "git_hub",
                        "git": {
                            "git_repo_url": "https://github.com/Cloud-Schematics/blueprint-example-modules/tree/main/IBM-Storage",
                            "git_branch": "main"
                        },
                        "catalog": {},
                        "cos_bucket": {}
                    },
                    "inputs": [
                        {
                            "name": "cos_instance_name",
                            "value": "$blueprint.cos_instance_name",
                            "metadata": {}
                        },
                        {
                            "name": "cos_storage_plan",
                            "value": "$blueprint.cos_storage_plan",
                            "metadata": {}
                        },
                        {
                            "name": "cos_single_site_loc",
                            "value": "ams03",
                            "metadata": {}
                        },
                        {
                            "name": "resource_group_id",
                            "value": "$module.basic-resource-group.outputs.resource_group_id",
                            "metadata": {}
                        }
                    ],
                    "outputs": [
                        {
                            "name": "cos_id",
                            "metadata": {}
                        },
                        {
                            "name": "cos_crn",
                            "metadata": {}
                        }
                    ],
                    "last_job": {},
                    "updated_at": "0001-01-01T00:00:00Z"
                }
            ],
            "updated_at": "0001-01-01T00:00:00Z"
        }
    },
    "bastion": {},
    "log_summary": {
        "log_start_at": "0001-01-01T00:00:00Z",
        "log_analyzed_till": "0001-01-01T00:00:00Z",
        "repo_download_job": {},
        "workspace_job": {},
        "flow_job": {},
        "action_job": {
            "recap": {}
        },
        "system_job": {}
    },
    "updated_at": "0001-01-01T00:00:00Z"
}
```
{: screen}


## Next steps
{: #bp-apply-nextsteps}

The environment and cloud resources are now deployed. The resources can be viewed on the `Resources` tab of the blueprint in the [Blueprints dashboard](https://cloud.ibm.com/schematics/blueprints){: external}, or using the [Resource list](https://cloud.ibm.com/resources){: external}. 
{: shortdesc}

The blueprint configuration and outputs can be reviewed by using the `blueprint get` command. See section [displaying blueprints](/docs/schematics?topic=schematics-schematics-cli-reference&interface=cli#schematics-blueprint-get). 

To destroy cloud resources and remove the blueprint environment, refer to, [destroy a blueprint environment](/docs/schematics?topic=schematics-destroy-blueprint&interface=cli), and [delete a blueprint config](/docs/schematics?topic=schematics-delete-blueprint&interface=cli#delete-blueprint-cli).

