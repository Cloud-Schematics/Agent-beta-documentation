---

copyright:
  years: 2017, 2022
lastupdated: "2022-06-13"

keywords: schematics remote agents, remote agents, terraform template to set up remote agents

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}

# {{site.data.keyword.bplong_notm}} Agent
{: #agents-intro}

The {{site.data.keyword.bpshort}} agent feature is currently in beta and should not be used for production workloads.
{: beta}

{{site.data.keyword.bplong}} agent is a feature that allows you to run a automation workloads for Terraform, or Ansible on your {{site.data.keyword.cloud_notm}} infrastructure to provide more flexibility and control. This feature needs a multi-step configuration to set up.
{: shortdesc}

## {{site.data.keyword.bplong_notm}} agent feature
{: #agents-features}

Following are the primary drivers to create the {{site.data.keyword.bplong_notm}} agent feature.

- You need to use {{site.data.keyword.bpshort}} and {{site.data.keyword.satellitelong}} to deploy and configure hybrid cloud resources such as private cloud resources, private data center resources, and other public cloud resources.
- You need {{site.data.keyword.bpshort}} to securely connect and manage hybrid cloud infrastructure by using Terraform, Ansible, and other automation tools to perform the deployment, configurations, and the operations.
- You need to reduce your wait time in a shared {{site.data.keyword.bpshort}} queue to run your automation.
- You need a dedicated infrastructure to run your automation and the ability to scale up or scale down the capacity depending on your automation workloads.
- You need to fine tune the network policies such as ingress or egress rules that are used by {{site.data.keyword.bpshort}} to connect to hybrid cloud infrastructure.
- You need a flexibility to use your softwares and versions in conjunction with automation engine provided by the {{site.data.keyword.bpshort}} runtime.


