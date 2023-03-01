---

copyright:
  years: 2017, 2022
lastupdated: "2022-09-13"

keywords: service to service authorization, catalog management, private catalog, schematics

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}

# Enabling service to service authorization 
{: #service-to-service-auth}

{{site.data.keyword.bplong}} supports IAM service to service authorization between {{site.data.keyword.bplong_notm}} and other Catalog Management services.

When you use CART `APIs` with the private catalog, you can enable service to service communication between {{site.data.keyword.bpshort}} and Catalog Management services in the account where the private catalog is on boarded.
Then, {{site.data.keyword.bpshort}} communicates with the private catalog in the account and fetches the  details such as the offering type, versions, and repository URLs. 
{: shortdesc}

You need to have access to the target service to create an authorization between services. You can grant only the level of access that you have as a user for the target service. For example, if you have viewer access on the target service, you can assign only the viewer role for the authorization.
{: note}

Follow these steps to provide access to the private catalog in your account for {{site.data.keyword.bpshort}} by using the console

- In the {{site.data.keyword.cloud_notm}} console, click **Manage** > **Access (IAM)**, and select **Authorizations**.
- Click **Create**.
- Select **{{site.data.keyword.bpshort}}** as a source service, and specify whether you want the authorization for all instances, only a specific instance, or instances in a certain resource group in the account.
-	Select **Catalog Management** as a target service and specify whether you want the authorization to be for all instances, only a specific instance, or instances only in a certain resource group in the account. This option is displayed only if the source service has dependent services. By selecting this option, policies are automatically created by the source service for the dependent services.
-	Select the **Viewer** as a role to assign access for the source service to access the target service.
- Click **Authorize**.





