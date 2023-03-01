---

copyright:
  years: 2017, 2022
lastupdated: "2022-12-22"

keywords: create blueprint, blueprint

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}

{{site.data.keyword.bpshort}} Blueprints is a [beta feature](/docs/schematics?topic=schematics-bp-beta-limitations) that is available for evaluation and testing purposes. It is not intended for production usage. Refer to the list of [limitations](/docs/schematics?topic=schematics-bp-beta-limitations#sc-bp-beta-limitation) for the beta release.
{: beta}

# Blueprints UI flow
{: #bp-ui}

## Creating a blueprint
{: #bp-ui-create}

You can follow these steps to create a blueprint using {{site.data.keyword.cloud_notm}} console.

1. Log in to [{{site.data.keyword.cloud_notm}}](https://cloud.ibm.com/){: external}.
2. Click **Schematics** > **Blueprints** > **Create Blueprint**.
    - In **Blueprint Details** section:
        - **Name** `<Provide unique name for your blueprint>`.
        - **Location** as `North America` or other [region](/docs/schematics?topic=schematics-multi-region-deployment) for this blueprint.
        - **Resource group** as `Default` or other resource group for this blueprint. For more information, see [Creating a resource group](/docs/account?topic=account-rgs). Ensure you have right access permission for the resource group.
        - **Tags** as `<Provide the tag name for your blueprint>`.
        - **Description** for the blueprint. Supports maximum character range from `0 - 2048`.
        - Click **Next**.
    - In **Blueprint URL** section:
        - **Repository URL** - `<Provide your valid GitHub, GitLab or Bitbucket repository URL that hosts your blueprint configuration file>`. For example, `https://github.com/Cloud-Schematics/blueprint-basic-example`.
        - **Personal access token** - `<Provide your Git personal access token, only for private Git repos>`.
        - Check the information that is entered are correct to create a blueprint.
        - Click **Next and save as draft**. Observe that a blueprint is created with a Blueprint ID and is in `Draft` Status.
           Validation takes a few seconds to fetch the template details from the Git repo. 
           {: note}

    - In **Input Variables** section:
        - Select **Import input file** drop down only when you want to import the new `inputs` YAML file for the blueprint.
            - In **Import input file (Optional)** section:
               -  **Input file GIT URL** - `<Provide your valid GitHub, GitLab or Bitbucket repository URL that hosts your blueprint configuration file>`. For example, `https://github.com/Cloud-Schematics/blueprint-basic-example/blob/main/basic-blueprint.yaml`.
               - **Source name** - Used to display from which source name the value is imported.
               - **Personal access token** - `<Provide your Git personal access token, only for private Git repos>`.
               - Click **Import values**.
        - Observe that the input variables from the `inputs.yaml` file are imported. Optionally, you can edit the variables.
           Enter variable values into the table by typing them in or by importing them. Prefilled default values, if any, were pulled from the blueprint template, but can be changed. If there is a dropdown, select a value from the dropdown.
           {: important}

        - Click **Done editing**, if the editing is done.
        - Click **Save draft** only if you need to save the draft to continue edit the input variables again later.
3. Click **Create Blueprint** that redirects to your blueprint page. 

## Updating a blueprint
{: #bp-ui-update}

1. Log in to [{{site.data.keyword.cloud_notm}}](https://cloud.ibm.com/){: external}.
2. Click **Schematics** > **Blueprints**.
3. Select your `<Blueprint_ID>`.

You can follow these steps to update the {{site.data.keyword.bpshort}} Blueprints by using {{site.data.keyword.cloud_notm}} console.

1. From the [{{site.data.keyword.cloud_notm}} Blueprints dashboard](https://cloud.ibm.com/schematics/blueprints){: external}. 
2. Click the **Name** of the blueprint **Name** that you want to edit.
3. Click the **Variables** tab to view your inputs on the **Inputs** tab.
4. Click **Edit** option in **Inputs Source**:
    - **Input file GIT URL**  - `<Edit the GIT URL>`.
    - **Personal access token (private repositories only)** - `<Provide your Git personal access token, only for private Git repos>`.
    - Click **Update**.
5. Click **Settings** tab.
    - In **Details** section, click **Edit**.
       - **Name** - Edit the blueprint name.
       - **Description** - Edit the description.
       - Click **Update**.
    - In **Blueprint Source** section, click **Edit**.
       - **Respository URL** - `<Edit the GIT URL>`.
       - **Personal access token (private repositories only)** - `<Provide your Git personal access token, only for private Git repos>`.
    - Click **Update**.
6. Click **Apply** to initiate the blueprint.

## Generating plan and apply blueprint
{: #bp-ui-plan}

You can follow these steps to generate plan and apply a blueprint using {{site.data.keyword.cloud_notm}} console.

1. Log in to [{{site.data.keyword.cloud_notm}}](https://cloud.ibm.com/){: external}.
2. Click **Schematics** > **Blueprints**.
3. Select your `<Blueprint_ID>`.
4. Click **Generate plan** to initiate the modules that are configured in the blueprint.

    Generate plan execution takes few seconds. Once generated check if the plan is correct. You can see the **Resource summary**, and **Jobs history** that displays the `blueprint_create_init` and the respective module job details. If **Generate plan** fails, you can update the blueprint.
     {: note}

5. Click **Apply plan** to provision the resources configured in your modules. You can observe the `In progress` staus.

    The apply plan exection takes few minutes based on the resources. The execution jobs show history of all blueprint, module activities, and the logs of the jobs. If **Apply plan** fails, you can update the blueprint.
    {: note}

## Destroying a blueprint
{: #bp-ui-destroy}

You can follow these steps to destroy a blueprint using {{site.data.keyword.cloud_notm}} console.

1. From the [{{site.data.keyword.cloud_notm}} Blueprints dashboard](https://cloud.ibm.com/schematics/blueprints){: external}. Click the blueprint name that you want to destroy.
2. Select the **Actions** drop down list.
3. Select **Destroy resources** to delete the resources associated with this blueprint.
4. Type the resource name in **Destroy resources** text box.
5. Click **Destroy** button.

## Deleting a blueprint
{: #bp-ui-delete}

You can follow these steps to delete a blueprints using {{site.data.keyword.cloud_notm}} console.

1. From the [{{site.data.keyword.cloud_notm}} Blueprints dashboard](https://cloud.ibm.com/schematics/blueprints){: external}. Click the blueprint name that you want to delete.
2. Select the **Actions** drop down list.
3. Select **Delete blueprint** option.
4. Type your blueprint name in **Delete blueprint** text box.
5. Click **Delete blueprint** button.

## Listing blueprints
{: #bp-ui-list}

You can follow these steps to list blueprints using {{site.data.keyword.cloud_notm}} console.

1. From the [{{site.data.keyword.cloud_notm}} console](https://cloud.ibm.com/schematics/blueprints){: external}. Click your blueprint name to view the blueprint details.
2. Click **Overview** to view the blueprint summary, that includes `Modules status`, `Variables summary`, `Blueprint Details` and `Recent Job runs` of your blueprint. 
    - Optional: From **Modules status** section, Click **View details** to view the module details.
    - Optional: From **Variables summary** section, Click **View details** to view the variable summary.
3. Click **Modules** tab to see the list of modules and their current status. 
    - Optional: Click **Show details** to view the module details.
    - Optional: Click **Name** that takes to the modules `Workspace` page. 
4. Click **Resources** tab to view the list of resources provisioned status by the blueprint.
5. Click **Variables** tab to view your **Inputs** and **Outputs** variables and values. Optional: you can edit the input variable and click **Save variables**.
6. Click **Jobs history** tab view the job logs of the blueprint and module activities.
7. Click **Settings** tab to view the configuration settings of the blueprint.


