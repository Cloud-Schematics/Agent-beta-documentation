---

copyright:
  years: 2017, 2022
lastupdated: "2022-06-13"

keywords: agent tar file, terraform template to set up remote agents, agent terraform templates

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}

# Reusing an agent templates
{: #agents-templates}

The {{site.data.keyword.bpshort}} agent feature is currently in beta and should not be used for production workloads.
{: beta}

The two pre-defined method speeds up the {{site.data.keyword.bpshort}} agent infrastructure and {{site.data.keyword.bpshort}} agent runtime service set up. 
- Using an agent Terraform templates and modules
- Using an archived configuration file
{: shortdesc}

## Using an agent Terraform templates and modules
{: #agents-tf-template}

You can access the {{site.data.keyword.bpshort}} agent related [Terraform template](https://github.ibm.com/schematics-solution/schematics-remote-agents/tree/master/templates) to create the following workspaces. 

- [`{{site.data.keyword.bpshort}} agents infrastructure workspace`](https://github.ibm.com/schematics-solution/schematics-remote-agents/tree/master/templates/infrastructure) to provision the {{site.data.keyword.cloud_notm}} resources such as VPC Gen2, COS, LogDNA, VPC Kubernetes cluster, subnets, and public gateways in your region.
- [`{{site.data.keyword.bpshort}} agents runtime services workspace`](https://github.ibm.com/schematics-solution/schematics-remote-agents/tree/master/templates/service) sets the namespaces, deployments, daemonsets, secrets, configmaps, job-runner service account, and cluster role and bindings in your {{site.data.keyword.containerlong_notm}} cluster.

## Using an archived configuration file
{: #agents-tf-tar}

You need to set up your {{site.data.keyword.cloud_notm}} account and resources and then deploy {{site.data.keyword.bpshort}} agent on the infrastructure created by using Terraform templates in TAR file format. Following are the two `tar` files used to create the `agents infrastructure` and deploy `agents runtime services` workspaces.
1. remoteagent-infrastructure-templates.tar
2. remoteagent-service-templates.tar

For more information, about the steps to use the `tar` files, refer to, [{{site.data.keyword.bpshort}} agents infrastructure and runtime set up by using `tar` readme file](https://github.ibm.com/schematics-solution/schematics-remote-agents/blob/master/docs/04-remoteagent-workspaces-using-tar-templates.md).

