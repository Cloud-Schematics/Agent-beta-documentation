---

copyright:
  years: 2017, 2022
lastupdated: "2022-06-13"

keywords: schematics agents register, register agents, register

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}

# Registering an agent
{: #register-agent}

The {{site.data.keyword.bpshort}} agent feature is currently in beta and should not be used for production workloads.
{: beta}

Once you have set up the {{site.data.keyword.bpshort}} agents infrastructure workspace and {{site.data.keyword.bpshort}} agents runtime services workspace. The next step is to register your agent on your infrastructure by running your workspaces. You can register an agent by using `UI`, `CLI`, or `API`.
{: shortdesc}

## Registering an agent through UI
{: #register-ui}
{: ui}

Here are the steps to register an agent through {{site.data.keyword.cloud_notm}} console.

1. Login to your [{{site.data.keyword.cloud_notm}}](https://cloud.ibm.com/){: external} account by using your credentials. 
2. From the {{site.data.keyword.cloud_notm}} page, select **Navigation menu** > **{{site.data.keyword.bpshort}}**.
3. Select **Integration** in the side navigation pane.
4. Click **Register** from the Agents panel.
5. In the **Register an Agent** page, enter the input value.
    - Name - Enter the unique name.
    - Agent ID - You can find the agent ID is available in the agent infrastructure workspace.
    - Profile - Create a trusted ID and link the profile to the trusted ID. For more information, about creating trusted profile, see [establishing trust with compute resources](/docs/account?topic=account-create-trusted-profile&interface=ui#create-profile-compute).
    - Resource Group - Select your resource group and specific resources where you need to register.
    - Location - Select the location, where you need to register.
6. Click **Save** to view the registered instance in the **Integrations** page.
7. Optional: From your registered agent instance you can click the three dots to **Edit Agent** to edit the agent configuration, **Assign Agent** to the workspace, **Disconnect Agent** to deactive the agent.

