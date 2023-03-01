---

copyright:
  years: 2017, 2023
lastupdated: "2023-02-03"

keywords: action templates, schematics template, terraform template, onboard private catalog, bulk onboard private catalog

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}

# Onboarding Terraform templates into {{site.data.keyword.cloud_notm}} private catalog 
{: #onboard-pvt-catalog}

Administering your Terraform template repositories in the {{site.data.keyword.cloud}} public repositories and perform bulk onboard into {{site.data.keyword.cloud_notm}} private catalog.
{: shortdesc}

## About {{site.data.keyword.bpshort}} Actions
{: #abt-bulkonbaord-action}

{{site.data.keyword.bplong_notm}} allows to build, update, scale, and remove multitiered apps and app runtime environments by using Ansible playbooks. You can also use Ansible to set up continuous deployment pipelines for your apps or automate cloud resource operations. For more information about {{site.data.keyword.bplong_notm}} action, see [Getting Started with configuration management](/docs/schematics?topic=schematics-getting-started-ansible).
{: shortdesc}

## About {{site.data.keyword.bpshort}} Actions playbook
{: #abt-bulkonboard-playbook}

You can now use {{site.data.keyword.bpshort}} Actions to install bulk onboarding Terraform templates into {{site.data.keyword.cloud_notm}} private catalog. This action contains the playbook that runs the python script to run bulk onboard of Terraform templates that are existing in [Cloud-{{site.data.keyword.bpshort}}](https://github.com/Cloud-Schematics) repository into {{site.data.keyword.cloud_notm}} private catalog. This onboard lead to higher visibility of your templates in the form of products for {{site.data.keyword.cloud_notm}} users to explore and enhance your templates and their provisioning in minimal time.
{: shortdesc}

## About automation script
{: #abt-bulkonboard-script}

The script starts your `BASE_URL` and fetches the `.tgz` file by using your credentials and validates the releases artifacts, vulnerability check. Then, create the catalog and uploads all the Terraform templates into {{site.data.keyword.cloud_notm}}
private catalog offerings. Also, the script validates the duplication of catalog name, and updates your offerings by maintaining the version control.
{: shortdesc}

**Prerequisites:**

The following environment variables need to be exported with your values. 

```sh
export BASE_URL=<https://github.com/Cloud-Schematics>
export CATALOG_MANAGEMENT_AUTH_TYPE=<iam>
export CATALOG_MANAGEMENT_APIKEY=<{xxxxxx}>
export CATALOG_NAME=<bulkonboard-terraform-templates>
export GITHUB_TOKEN=<xxxxxxx>
```
{: codeblock}

## About clickable button
{: #abt-button}

`View GitHub repo`: Click this link to view the Git repository where the template is stored. You can review the file structure, the Ansible playbook instructions, and the `README` file that contains the steps to use the template in {{site.data.keyword.bpshort}}.
`Deploy to {{site.data.keyword.cloud_notm}}`: This link points you to the **Create an action** page with the pre-populated values for **GitHub repository URL** and the **Action name** parameters. 


## Running bulk onboard of Terraform templates into {{site.data.keyword.cloud_notm}} private catalog
{: #ansible-bulkonboarding}

Description
:    Use `bulkonboard-terraform-templates` Ansible playbook to run bulk onboard of your Terraform templates that are bundled in a <code>.tgz</code> format. To configure and run the {{site.data.keyword.bpshort}} Actions by using the console, see the template [readme file](https://github.ibm.com/Tanya-Shanker/catalog-automation/blob/master/README.md){: external}.

Access
:   <img src="images/viewgithubrepo.png" alt="View GitHub repository" usemap="#viewgithubimage_maptgz1">
<map name="viewgithubimage_maptgz1">
    <area alt="View GitHub repo" title="View GitHub repo" href="https://github.ibm.com/Tanya-Shanker/catalog-automation" target="_blank" coords="3,1,140,20" shape="rect">
</map>

Deploy
:   <img usemap="#deploybutton_maptgz1" alt="Auto deployment button" src="https://cloud.ibm.com/media/docs/images/icons/Deploy_to_cloud.svg"><map name="deploybutton_maptgz1" alt="This image leads to create an action.">
    <area alt="Deploy to {{site.data.keyword.cloud_notm}}" title="Deploy to {{site.data.keyword.cloud_notm}}" href="https://cloud.ibm.com/schematics/actions/create?name=bulkonboard-terraform-templates&repository=https://github.com/Cloud-Schematics/bulkonboard-terraform-templates" target="_blank" coords="1,3,139,20" shape="rect">
</map>



