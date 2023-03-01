---

copyright:
  years: 2017, 2022
lastupdated: "2022-11-29"

keywords: schematics relationship, relationship between workspace and blueprint, relationship, relations

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}

# Relating {{site.data.keyword.bpshort}} offerings
{: #sc-relationship}

{{site.data.keyword.bplong}} provides automation by offering declarative Terraform templates to ensure a desired provisioned cloud infrastructure. Native integration with {{site.data.keyword.redhat_openshift_full}} Ansible extends configuration, management and provisioning to software and applications, and integrates with other {{site.data.keyword.cloud}} services. The relationship between {{site.data.keyword.bpshort}} Workspaces, Blueprints, Agents, and Actions. 
{: shortdesc}



## {{site.data.keyword.bpshort}} Blueprints
{: #sc-blueprints}

Is an automation solution for large-scale cloud Infrastructure as Code (IaC) environments. It builds, manage, and operate a complex solution architecture from reusable IaC modules. The Terraform modules contain the group of Terraform templates that helps to create multiple {{site.data.keyword.bpshort}} Workspaces in a blueprint. For more information about Blueprint architecture and its features, see [{{site.data.keyword.bpshort}} Blueprints](/docs/schematics?topic=schematics-blueprint-intro).
{: shortdesc}

## {{site.data.keyword.bpshort}} Workspaces
{: #sc-workspaces}

Organize your Terraform templates and control the access to run infrastructure code in your {{site.data.keyword.cloud}} account. Before you create a workspace, make sure that you design the organizational structure of your Git repository, and workspaces. So that you can replicate and manage your configurations across multiple environments. For more information, see [{{site.data.keyword.bpshort}} Workspaces setup](/docs/schematics?topic=schematics-workspace-setup).
{: shortdesc}

## {{site.data.keyword.bpshort}} Actions
{: #sc-actions}

Acts as a container for artifacts and used to run your Ansible playbook in {{site.data.keyword.bpshort}}. The action points to your Ansible playbook in GitHub, or GitLab repository, the inventory to run the playbook, input variables, and environment variables are used to run the playbook. For more information about managing {{site.data.keyword.bpshort}} Actions and its features, see [managing Actions](/docs/schematics?topic=schematics-workspace-setup).
{: shortdesc}

## {{site.data.keyword.bpshort}} Agents
{: #sc-agents}

Extends and integrates the {{site.data.keyword.bpshort}} Workspaces that running in your private network to the {{site.data.keyword.bplong_notm}} service. Agents provisions, configure, and operate your private or on-premises cloud cluster resources without any time, network, or software restrictions. The {{site.data.keyword.bpshort}} Agents runtime uses `Terraform`, `Terraform CLI v1.0.11`, `Terraform CLI v1.1.5`, and `Micro-services`. For more information about architecture and features of Agents, see [{{site.data.keyword.bpshort}} Agents](/docs/schematics?topic=schematics-agents-intro).
{: shortdesc}

