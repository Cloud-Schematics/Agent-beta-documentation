---

copyright:
  years: 2017, 2022
lastupdated: "2022-11-14"

keywords: terraform template guidelines, terraform config file guidelines, sample terraform files, terraform provider, terraform variables, terraform input variables, terraform template

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}

# Using shared data sets for workspace variables
{: #shared-dataset}

Shared data sets provide a way to define the variables globally in {{site.data.keyword.bplong_notm}} and scope across the {{site.data.keyword.bplong_notm}} Workspaces. Let's learn how to create and use the shared data sets.
{: shortdesc}

## Creating shared data sets
{: #create-shared-data}

Create a shared data set and specify all the variables that you want to add to your data set.
{: shortdesc}

To create a shared data set in your workspace:
1. From the {{site.data.keyword.bpfull_notm}} [shared data dashboard](https://cloud.ibm.com/schematics){: external}, click **Create shared data set**.
2. Enter a name for your shared data set and select the resource group where you want to create the shared data set.
3. Enter an optional description for your shared data set.
4. Select **Add your own**, to enter the variables that you want to add to your shared data set.
    a. Enter the name and a default value for your variable.
    b. Select if the variable value is sensitive, such as for credentials. Sensitive variables values are not shown in the console. 
    {: note}

    c. Select if the variable value is immutable. If you select this option, users cannot overwrite the default value in the console later.
    d. Click the **Advanced data options** option to specify a variable value range or to select the variable value type.
    e. To add more variables, click **Add data**.
    f. To save your shared data set, click Create.
Use the shared data in your workspace and then link out to the topic that describes in the workspace.

## Updating shared data sets
{: #update-shared-data}

If you want to add or remove variables from your shared data set, or if you want to change the default variable values, you can update your shared data set.
{: shortdesc}

To update a shared data set in your workspace:
1. From the {{site.data.keyword.bpfull_notm}} [shared data dashboard](https://cloud.ibm.com/schematics){: external}, find the shared data set that you want to update.
2. Search the **Workspace** and select **Settings** to update the shared data set.
3. Scroll to the **Variables** section to select shared data set name you need to update.
4. Click the Actions menu to view the **Edit** and **Delete** options.
5. Edit the **Override value** parameters and click the link object to link the value to the shared data set.
6. Click **Update** and click **Save Changes**.

Select the variable values you need to update and remain linked to the shared data set and all others will be unlinked. Unlinked variable values is manually managed and stay filled with the last relevant data.
You can update share data set in batch or bulk mode.
{: note}


## Deleting shared data sets
{: #delete-shared-data}

If you do not need your shared data set anymore, you can remove all the data permanently.
{: shortdesc}

To delete a shared data set in your workspace:
1. From the {{site.data.keyword.bpfull_notm}} [shared data dashboard](https://cloud.ibm.com/schematics){: external}, find the shared data set that you want to delete.
2. Click the Actions menu to view the `Edit`, and `Delete` options.
3. From the Actions menu, click **Delete**.
4. Type the shared data set that you need to delete.
5. Click **Delete**.

Make sure to back up all required shared data set. Once shared data set is deleted you cannot undo.
{: note}

## Using shared data sets in a workspace
{: #using-shared-data}

1. From the {{site.data.keyword.bpfull_notm}} [shared data dashboard](https://cloud.ibm.com/schematics){: external} open an existing workspace or create a new workspace, see [Creating workspaces](/docs/schematics?topic=schematics-workspace-setup#create-workspace). 
2. From your existing or new workspace page, click **Settings**.
3. From the **Variables** section to select the **Shared data set**.
4. From the **Shared data set** drop down list to link the variable and value to the resources.
5. Click **Save changes** to view the successful message of the value linked to your shared data set.
6. Click **Apply plan**.

To manage shared data sets, click Unlink button to edit shared data set by using **Manage** option in staging or prod and click **Save changes**.
{: note}




