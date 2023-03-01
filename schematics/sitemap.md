---

copyright:
  years: 2017, 2023
lastupdated: "2023-03-01"

keywords: schematics
subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}

# Site map
{: #sitemap}





## Getting started
{: #sitemap_getting_started}


[Getting started: {{site.data.keyword.bplong_notm}}](/docs/schematics?topic=schematics-getting-started#getting-started)

[Using Workspaces to deploy infrastructure and cloud services](/docs/schematics?topic=schematics-get-started-terraform#get-started-terraform)

* [Before you begin](/docs/schematics?topic=schematics-get-started-terraform#prereq)

* [Creating an {{site.data.keyword.cos_full_notm}} instance with {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-get-started-terraform#create-cos)

    * [Output](/docs/schematics?topic=schematics-get-started-terraform#create-cos-output)

* [What's next?](/docs/schematics?topic=schematics-get-started-terraform#whats-next-gs)

[Using Agents to perform configuration management](/docs/schematics?topic=schematics-getting-started-ansible#getting-started-ansible)

* [Before you begin](/docs/schematics?topic=schematics-getting-started-ansible#ansible-prereq)

* [Starting and stopping {{site.data.keyword.vsi_is_short}}](/docs/schematics?topic=schematics-getting-started-ansible#ansible-vsi)

* [What's next?](/docs/schematics?topic=schematics-getting-started-ansible#ansible-whats-next)

[Software deployment in {{site.data.keyword.bplong_notm}}](/docs/schematics?topic=schematics-get-started-software#get-started-software)

* [Before you begin](/docs/schematics?topic=schematics-get-started-software#vsi-postgres-prereq)

* [Setting up and configuring a classic VSI to run PostgreSQL with {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-get-started-software#vsi-postgres)

* [What's next?](/docs/schematics?topic=schematics-get-started-software#whats-next)

[Using Blueprints to deploy large-scale cloud environments](/docs/schematics?topic=schematics-get-started-blueprints#get-started-blueprints)

* [Deploy blueprint through UI](/docs/schematics?topic=schematics-get-started-blueprints#deploy-bp-ui)

    * [Creating a blueprint in {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-get-started-blueprints#get-started-blueprints-create-ui)

    * [Applying the blueprint configuration to create cloud resources](/docs/schematics?topic=schematics-get-started-blueprints#get-started-blueprints-apply-ui)

    * [Displaying the blueprint](/docs/schematics?topic=schematics-get-started-blueprints#get-started-bp-list-ui)

    * [Next steps](/docs/schematics?topic=schematics-get-started-blueprints#get-started-blueprints-nextsteps-ui)

* [Deploy a blueprint using the CLI](/docs/schematics?topic=schematics-get-started-blueprints#deploy-bp-cli)

    * [Before your begin](/docs/schematics?topic=schematics-get-started-blueprints#get-started-blueprints-prereq)

    * [Select a blueprint template](/docs/schematics?topic=schematics-get-started-blueprints#get-started-blueprints-select)

    * [Creating a blueprint in {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-get-started-blueprints#get-started-blueprints-create)

    * [Applying the blueprint to create cloud resources](/docs/schematics?topic=schematics-get-started-blueprints#get-started-blueprints-install)

    * [Next steps](/docs/schematics?topic=schematics-get-started-blueprints#get-started-blueprints-nextsteps)


## About
{: #sitemap_about}


[{{site.data.keyword.bpshort}} overview](/docs/schematics?topic=schematics-learn-about-schematics#learn-about-schematics)

* [IaC automation as-a-service](/docs/schematics?topic=schematics-learn-about-schematics#sc-IaCaas)

* [{{site.data.keyword.bpshort}} IaC offerings](/docs/schematics?topic=schematics-learn-about-schematics#sc-offerings)

    * [{{site.data.keyword.bpshort}} Blueprints](/docs/schematics?topic=schematics-learn-about-schematics#sc-blueprints)

    * [{{site.data.keyword.bpshort}} Workspaces](/docs/schematics?topic=schematics-learn-about-schematics#sc-workspaces)

    * [{{site.data.keyword.bpshort}} Actions](/docs/schematics?topic=schematics-learn-about-schematics#sc-actions)

    * [{{site.data.keyword.bpshort}} Agents](/docs/schematics?topic=schematics-learn-about-schematics#sc-agents)

* [Benefits of using Schematics](/docs/schematics?topic=schematics-learn-about-schematics#sc-benefits)

[What is Infrastructure as Code?](/docs/schematics?topic=schematics-infrastructure-as-code#infrastructure-as-code)

* [Benefits of Infrastructure as Code](/docs/schematics?topic=schematics-infrastructure-as-code#iac-benefits)

* [Best Practices](/docs/schematics?topic=schematics-infrastructure-as-code#iac-best-practices)

    * [Codifying everything in IaC](/docs/schematics?topic=schematics-infrastructure-as-code#iac-bp-codify)

    * [Minimize documentation](/docs/schematics?topic=schematics-infrastructure-as-code#iac-bp-docs)

    * [Testing](/docs/schematics?topic=schematics-infrastructure-as-code#iac-bp-testings)

    * [Modular Infrastructure](/docs/schematics?topic=schematics-infrastructure-as-code#iac-bp-modularity)

    * [Declarative versus imperative approaches to IaC](/docs/schematics?topic=schematics-infrastructure-as-code#iac-declarative)

    * [Declarative Terraform and lifecycle management](/docs/schematics?topic=schematics-infrastructure-as-code#iac-declarative-lifecycle)

    * [Idempotence](/docs/schematics?topic=schematics-infrastructure-as-code#iac-idempotence)

    * [Immutablity](/docs/schematics?topic=schematics-infrastructure-as-code#iac-immutability)

* [Next steps](/docs/schematics?topic=schematics-infrastructure-as-code#iac-nextsteps)

[Choosing your IaC tool](/docs/schematics?topic=schematics-schematics-open-projects#schematics-open-projects)

* [What is Provisioning?](/docs/schematics?topic=schematics-schematics-open-projects#sc-iac-provisioning)

* [What is Configuration Management?](/docs/schematics?topic=schematics-schematics-open-projects#sc-iac-cm)

* [How to choose your IaC tool](/docs/schematics?topic=schematics-schematics-open-projects#sc-iac-choosing)

    * [Understanding Schematics features and IaC tools](/docs/schematics?topic=schematics-schematics-open-projects#sc-iac-mapping)

* [Next steps](/docs/schematics?topic=schematics-schematics-open-projects#nextsteps-technologies)

[{{site.data.keyword.bpshort}} Workspaces](/docs/schematics?topic=schematics-sc-workspaces#sc-workspaces)

* [Architecture](/docs/schematics?topic=schematics-sc-workspaces#sch-wks-overview)

* [Features](/docs/schematics?topic=schematics-sc-workspaces#sc-wks-features)

* [Next steps](/docs/schematics?topic=schematics-sc-workspaces#sc-wks-nextsteps)

[{{site.data.keyword.bpshort}} Actions](/docs/schematics?topic=schematics-sc-actions#sc-actions)

* [Architecture](/docs/schematics?topic=schematics-sc-actions#sc-actions-overview)

* [Using Actions](/docs/schematics?topic=schematics-sc-actions#sc-actions-use)

* [Next steps](/docs/schematics?topic=schematics-sc-actions#sch-actions-nextsteps)

[{{site.data.keyword.bpshort}} Agents](/docs/schematics?topic=schematics-agents-intro#agents-intro)

* [Usage of an Agent](/docs/schematics?topic=schematics-agents-intro#agent-usage)

* [{{site.data.keyword.bpshort}} Agent architecture](/docs/schematics?topic=schematics-agents-intro#about-agents-architecture)

* [Augmenting {{site.data.keyword.bpshort}} with {{site.data.keyword.bpshort}} Agents](/docs/schematics?topic=schematics-agents-intro#agents-augmenting)

* [Setting up an Agent](/docs/schematics?topic=schematics-agents-intro#setting-agent)

* [Next steps](/docs/schematics?topic=schematics-agents-intro#nextsteps-agent-arch)

[{{site.data.keyword.bpshort}} Blueprints](/docs/schematics?topic=schematics-blueprint-intro#blueprint-intro)

* [Overview](/docs/schematics?topic=schematics-blueprint-intro#blueprint-overview)

* [Features](/docs/schematics?topic=schematics-blueprint-intro#blueprint-features)

* [Next steps](/docs/schematics?topic=schematics-blueprint-intro#nextsteps-bp-arch)

[Understanding {{site.data.keyword.bpshort}} use cases](/docs/schematics?topic=schematics-how-it-works#how-it-works)

* [Infrastructure deployment with {{site.data.keyword.bpshort}} Workspaces](/docs/schematics?topic=schematics-how-it-works#how-to-workspaces)

* [Configuration management with {{site.data.keyword.bpshort}} Actions](/docs/schematics?topic=schematics-how-it-works#how-to-actions)

* [Software deployments with IBM-provided templates](/docs/schematics?topic=schematics-how-it-works#how-to-software)

* [Next steps](/docs/schematics?topic=schematics-how-it-works#usecase-nextsteps)

[Your responsibilities when using {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-sc-responsibilities#sc-responsibilities)

* [Incident and operations management](/docs/schematics?topic=schematics-sc-responsibilities#incident-ops-mgt)

* [Change management](/docs/schematics?topic=schematics-sc-responsibilities#change-mgt)

* [Identity and access management](/docs/schematics?topic=schematics-sc-responsibilities#iam)

* [Security and regulation compliance](/docs/schematics?topic=schematics-sc-responsibilities#security-reg-compliance)

* [Disaster recovery](/docs/schematics?topic=schematics-sc-responsibilities#disaster-recovery)


## Understanding Blueprints
{: #sitemap_understanding_blueprints}


[Understanding blueprints and environments](/docs/schematics?topic=schematics-work-with-blueprints#work-with-blueprints)

* [Cloud infrastructure lifecycle](/docs/schematics?topic=schematics-work-with-blueprints#cloud-infra-lifecycle)

* [Working with environments and the blueprint lifecycle](/docs/schematics?topic=schematics-work-with-blueprints#bp-working-env)

    * [Defining blueprints](/docs/schematics?topic=schematics-work-with-blueprints#bp-define)

    * [Deploying blueprints](/docs/schematics?topic=schematics-work-with-blueprints#bp-deploy)

    * [Maintaining blueprints](/docs/schematics?topic=schematics-work-with-blueprints#bp-maintain)

    * [Deleting blueprints](/docs/schematics?topic=schematics-work-with-blueprints#bp-delete)

* [Next steps](/docs/schematics?topic=schematics-work-with-blueprints#working-bp-nextsteps)

[Scaling environments](/docs/schematics?topic=schematics-blueprint-scaling#blueprint-scaling)

* [Remote state data sources](/docs/schematics?topic=schematics-blueprint-scaling#blueprint-scaling-remotestate)

* [Orchestration and modules](/docs/schematics?topic=schematics-blueprint-scaling#blueprint-scaling-orchestration)

[Defining blueprints](/docs/schematics?topic=schematics-define-blueprints#define-blueprints)

* [Creating templates, inputs and configuration](/docs/schematics?topic=schematics-define-blueprints#define-templates-input)

* [Steps to define a blueprint](/docs/schematics?topic=schematics-define-blueprints#define-blueprint-steps)

* [Next steps](/docs/schematics?topic=schematics-define-blueprints#define-nextsteps)

[Deploying blueprints](/docs/schematics?topic=schematics-deploy-blueprints#deploy-blueprints)

* [Next steps](/docs/schematics?topic=schematics-deploy-blueprints#deploy-nextsteps)

[Maintaining blueprints](/docs/schematics?topic=schematics-update-op-blueprints#update-op-blueprints)

* [Updating blueprint environments](/docs/schematics?topic=schematics-update-op-blueprints#update-multistep)

* [Next steps](/docs/schematics?topic=schematics-update-op-blueprints#operate-nextsteps)

[Deleting blueprints](/docs/schematics?topic=schematics-delete-blueprints#delete-blueprints)

* [Next steps](/docs/schematics?topic=schematics-delete-blueprints#delete-nextsteps)


## Internal adopters
{: #sitemap_internal_adopters}


[Guidelines for using {{site.data.keyword.bpshort}} stage environment](/docs/schematics?topic=schematics-stage-guidelines-schematics#stage-guidelines-schematics)

[Enabling service to service authorization](/docs/schematics?topic=schematics-service-to-service-auth#service-to-service-auth)

[Embedded {{site.data.keyword.bplong_notm}}](/docs/schematics?topic=schematics-embedded-schematics-intro#embedded-schematics-intro)

* [Embedded {{site.data.keyword.bpshort}} `APIs`](/docs/schematics?topic=schematics-embedded-schematics-intro#embedded-schematics-api)

* [Comparing {{site.data.keyword.bpshort}} with the embedded {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-embedded-schematics-intro#comparsion)

* [Design flow](/docs/schematics?topic=schematics-embedded-schematics-intro#embedded-schematics-design)

* [Enhancements](/docs/schematics?topic=schematics-embedded-schematics-intro#embedded-schematics-enhancement)

[IBM Cloud Schematics internal_v1.0 API](https://test.cloud.ibm.com/apidocs/schematics){: external}


## Security and compliance
{: #sitemap_security_and_compliance}


[Security](/docs/schematics?topic=schematics-security#security)

* [Secure access control](/docs/schematics?topic=schematics-security#secure-access-control)

[Compliance](/docs/schematics?topic=schematics-compliance#compliance)

* [General Data Protection Regulation (GDPR) readiness](/docs/schematics?topic=schematics-compliance#compliance-gdpr)

* [Privacy shield](/docs/schematics?topic=schematics-compliance#compliance-privacy)

* [International Organization for Standardization (ISO)](/docs/schematics?topic=schematics-compliance#international-organization-for-standardization-iso)

* [SOC 2 Type 2 Certification](/docs/schematics?topic=schematics-compliance#soc-2-type-2-certification)

[Managing security and compliance with {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-manage-security-compliance#manage-security-compliance)

* [Monitoring security and compliance posture with {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-manage-security-compliance#monitor-schematics)

    * [Available goals for {{site.data.keyword.bplong_notm}}](/docs/schematics?topic=schematics-manage-security-compliance#schematics-available-goals)

[Protecting {{site.data.keyword.bpshort}} services with context-based restrictions](/docs/schematics?topic=schematics-access-control-cbr#access-control-cbr)

* [Managing CBR settings](/docs/schematics?topic=schematics-access-control-cbr#manage-cbr-settings)

* [Overview](/docs/schematics?topic=schematics-access-control-cbr#cbr-overview)

* [Understanding network zones](/docs/schematics?topic=schematics-access-control-cbr#cbr-network-zones)

    * [Creating network zones by using the CBR API](/docs/schematics?topic=schematics-access-control-cbr#cbr-create-zones-api)

    * [Creating network zones by using the CBR UI](/docs/schematics?topic=schematics-access-control-cbr#cbr-create-zone-ui)

* [Understanding network rules](/docs/schematics?topic=schematics-access-control-cbr#cbr-network-rules)

    * [Create network rules by using the CBR API](/docs/schematics?topic=schematics-access-control-cbr#cbr-create-rules-api)

    * [Creating network rules by using the CBR UI](/docs/schematics?topic=schematics-access-control-cbr#cbr-create-rules-ui)

* [Next steps](/docs/schematics?topic=schematics-access-control-cbr#cbr-next-steps)

[Data privacy and governance](/docs/schematics?topic=schematics-data-privacy-and-governance#data-privacy-and-governance)

[General Data Protection Regulation (GDPR)](/docs/schematics?topic=schematics-general-data-protection-regulation-gdpr#general-data-protection-regulation-gdpr)

* [How do you audit access to {{site.data.keyword.bpshort}}?](/docs/schematics?topic=schematics-general-data-protection-regulation-gdpr#how-do-i-audit-access-to-ibm-schematics)

* [Supporting classifications of personal data](/docs/schematics?topic=schematics-general-data-protection-regulation-gdpr#supported-classifications-of-personal-data)

* [About user data](/docs/schematics?topic=schematics-general-data-protection-regulation-gdpr#data-about-me)

* [Is the {{site.data.keyword.bpshort}} database encrypted?](/docs/schematics?topic=schematics-general-data-protection-regulation-gdpr#is-our-ibm-schematics-database-encrypted)

* [Data locations](/docs/schematics?topic=schematics-general-data-protection-regulation-gdpr#data-locations)

* [Service security](/docs/schematics?topic=schematics-general-data-protection-regulation-gdpr#service-security)

* [Deletion of data](/docs/schematics?topic=schematics-general-data-protection-regulation-gdpr#deletion-of-data)

[Best practices for securing the {{site.data.keyword.bpshort}} objects](/docs/schematics?topic=schematics-bp-secure-objects#bp-secure-objects)

* [Best practices for creating Terraform Templates or modules in Git repositories](/docs/schematics?topic=schematics-bp-secure-objects#bp-secure-repo)

    * [What are the best practices that you must follow in developing the Terraform templates, and publishing the same in the Git repositories?](/docs/schematics?topic=schematics-bp-secure-objects#bp-template-strategy)

    * [Can you create `tfvars` files with the {{site.data.keyword.cloud}} provider templates?](/docs/schematics?topic=schematics-bp-secure-objects#bp-security-tfvars)

    * [How can the Terraform developers ensure that the sensitive data is not leaked in the log files?](/docs/schematics?topic=schematics-bp-secure-objects#bp-security-leak)

* [Best practices of managing {{site.data.keyword.bpshort}} Workspaces](/docs/schematics?topic=schematics-bp-secure-objects#bp-workspaces)

    * [What are the best practices that you must follow in creating a workspace for the Terraform template?](/docs/schematics?topic=schematics-bp-secure-objects#bp-security-wks)

    * [How can you ensure that the sensitive data used by the Terraform automation, do not leak in the logs or outputs?](/docs/schematics?topic=schematics-bp-secure-objects#bp-security-leak-log)

    * [How can you protect the access to workspaces and its data?](/docs/schematics?topic=schematics-bp-secure-objects#bp-security-wks-data)

    * [How does {{site.data.keyword.bpshort}} protect the workspace data through Terraform state file, or log files?](/docs/schematics?topic=schematics-bp-secure-objects#bp-protect-data)

* [Best practices of managing {{site.data.keyword.bpshort}} Actions](/docs/schematics?topic=schematics-bp-secure-objects#bp-actions)

    * [What are the best practices that you must follow in creating an action for the Ansible template?](/docs/schematics?topic=schematics-bp-secure-objects#bp-security-ansible)

    * [How can you protect the access to actions and its data?](/docs/schematics?topic=schematics-bp-secure-objects#bp-security-action-data)

    * [How does {{site.data.keyword.bpshort}} protect the action data through input credentials state file, or log files?](/docs/schematics?topic=schematics-bp-secure-objects#bp-security-protect)

* [Protecting data of {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-bp-secure-objects#bp-protect)

    * [Access protection by using Identity and Access Management](/docs/schematics?topic=schematics-bp-secure-objects#bp-security-iam)

    * [Non-repudiation by using Activity tracker](/docs/schematics?topic=schematics-bp-secure-objects#bp-security-atracker)

    * [Data protection by using KMS](/docs/schematics?topic=schematics-bp-secure-objects#bp-security-data-protection)

* [Next steps](/docs/schematics?topic=schematics-bp-secure-objects#bp-security-next-steps)


## {{site.data.keyword.bpshort}} architecture
{: #sitemap__architecture}


[{{site.data.keyword.bpshort}} architecture](/docs/schematics?topic=schematics-compute-isolation#compute-isolation)

* [Architectural flow](/docs/schematics?topic=schematics-compute-isolation#basic-architecture)

* [Workload isolation](/docs/schematics?topic=schematics-compute-isolation#workload-isolation)

    * [How are API requests to the service isolated from other API requests?](/docs/schematics?topic=schematics-compute-isolation#workload-api-isolation)

    * [How is the information in {{site.data.keyword.cloudant}} and {{site.data.keyword.cos_full_notm}} isolated from other tenant data?](/docs/schematics?topic=schematics-compute-isolation#workload-info-isolation)

    * [How are cloud resources isolated from other tenants?](/docs/schematics?topic=schematics-compute-isolation#workload-tenant-isolation)


## Release notes
{: #sitemap_release_notes}


[Release notes](/docs/schematics?topic=schematics-schematics-relnotes#schematics-relnotes)

* [February 2023](/docs/schematics?topic=schematics-schematics-relnotes#schematics-feb23)

    * Review the release notes for February 2023.

    * [27 February 2023](/docs/schematics?topic=schematics-schematics-relnotes#schematics-feb2723)

        * {{site.data.keyword.bpshort}} Agents beta-1 release in production.

    * [16 February 2023](/docs/schematics?topic=schematics-schematics-relnotes#schematics-feb2023)

        * {{site.data.keyword.bpshort}} allowed IP address for `US`, `EU Central`, and `UK South` region are updated

    * [7 February 2023](/docs/schematics?topic=schematics-schematics-relnotes#schematics-feb0723)

        * Release {{site.data.keyword.bpshort}} command-line plug-in.

    * [3 February 2023](/docs/schematics?topic=schematics-schematics-relnotes#schematics-feb0323)

        * Enhancement in {{site.data.keyword.bpshort}} to protect its services with context-based restrictions

* [January 2023](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jan23)

    * Review the release notes for January 2023.

    * [30 January 2023](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jan3023)

        * Release {{site.data.keyword.bpshort}} command-line plug-in.

    * [27 January 2023](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jan2723)

        * Enhancement in {{site.data.keyword.bpshort}} protect its services with context-based restrictions

* [December 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-dec22)

    * Review the release notes for December 2022.

    * [13 December 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-dec1322)

        * Release {{site.data.keyword.bpshort}} Agents GitHub repository.

        * Release {{site.data.keyword.bpshort}} Blueprints bug fixes. Support for input values larger than 15,000 bytes.  

        * Release {{site.data.keyword.bpshort}} command-line plug-in.

* [November 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-nov22)

    * Review the release notes for November 2022.

    * [29 November 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-nov2922)

        * Enhance {{site.data.keyword.bpshort}} documentation

    * [18 November 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-nov1822)

        * Release {{site.data.keyword.bpshort}} Blueprints UI.

        * Release {{site.data.keyword.bpshort}} command-line plug-in.

    * [15 November 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-nov1522)

        * Release {{site.data.keyword.bpshort}} Agents GitHub repository.

    * [14 November 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-nov1422)

        * {{site.data.keyword.bpshort}} Blueprints template schema changes.

    * [03 November 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-nov0322)

        * Release {{site.data.keyword.bpshort}} command-line plug-in.

* [September 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-sept22)

    * {{site.data.keyword.bpshort}} deprecates `Python v3.6` and upgrades the {{site.data.keyword.bpshort}} Job image to use `Python v3.8` by mid of September 2022. For more information, see [{{site.data.keyword.bpshort}} announcement](https://cloud.ibm.com/status/announcement?component=schematics){: external} tools.

    * Review the release notes for September 2022.

    * [21 September 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-sept2222)

        * The {{site.data.keyword.bpshort}} Job image supports `Python v3.8` 

* [August 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-aug22)

    * Review the release notes for August 2022.

    * [16 August 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-aug1622)

        * {{site.data.keyword.bpshort}} runtime now supports Ansible v2.9.27

    * [11 August 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-aug1122)

        * Release {{site.data.keyword.bpshort}} command-line plug-in 

    * [04 August 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-aug2022)

        * {{site.data.keyword.bpshort}} allowed IP address for `US`, `EU Central`, and `UK South` region are updated

* [July 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-july22)

    * Review the release notes for July 2022.

    * [26 July 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jul2622)

        * Release {{site.data.keyword.bpshort}} command-line plug-in 

    * [20 July 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-july2022)

        * {{site.data.keyword.bpshort}} allowed IP address for `US` region is updated

    * [11 July 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-july1122)

        * {{site.data.keyword.bpshort}} Agents beta release in production.

        * Release {{site.data.keyword.bpshort}} command-line plug-in 

    * [8 July 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-july0822)

        * {{site.data.keyword.bpshort}} Blueprints beta release in production.

        * Release {{site.data.keyword.bpshort}} command-line plug-in 

* [June 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-june22)

    * Review the release notes for June 2022.

    * [22 June 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-june2222)

        * {{site.data.keyword.bpshort}} Agents beta release

        * {{site.data.keyword.bpshort}} Blueprints beta release

        * Enhanced FAQ documentation

    * [6 June 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-june0622)

        * Enhance {{site.data.keyword.bpshort}} getting started section

* [May 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-may22)

    * Review the release notes for May 2022.

    * [12 May 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-may1222)

        * Enhance documentation with the security and compliance section

        * Enhance documentation with the best practices 

    * [5 May 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-may0522)

        * Release {{site.data.keyword.bpshort}} command-line plug-in 

* [April 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-apr22)

    * Review the release notes for April 2022.

    * [30 April 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-apr3022)

        * Support detecting drift

        * Support stopping or terminating the running job

        * Support more frequently asked questions (FAQs) 

        * Support enhanced {{site.data.keyword.bpshort}} resource view

    * [26 April 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-apr2622)

        * Release {{site.data.keyword.bpshort}} command-line plug-in 

    * [17 April 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-apr2722)

        * Release {{site.data.keyword.bpshort}} command-line plug-in 

    * [18 April 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-apr1822)

        * Support array of injectable Terraform blocks in create workspace API

        * Release {{site.data.keyword.bpshort}} command-line plug-in 

    * [12 April 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-apr3122)

        * {{site.data.keyword.bpshort}} command-line supports private {{site.data.keyword.bpshort}} endpoint

        * Support `.JSON` and `.tfvars` file extension for {{site.data.keyword.bpshort}} plan and apply commands

        * Enhance resources tabular data view for resources.

        * Deprecate and warning message when using `ibmcloud terraform` command.

        * Release {{site.data.keyword.bpshort}} command-line plug-in 

* [March 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-mar22)

    * Review the release notes for March 2022.

    * [31 March 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-mar3122)

        * Support deleting {{site.data.keyword.bpshort}} data objects 

        * Fixes related to {{site.data.keyword.bpshort}} Actions and workspace

        * Get job files API supports `plan_json` file type

    * [15 March 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-mar1522)

        * Support `__netrc__` environment values in private Git repository

    * [4 March 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-mar422)

        * Support `Terraform v1.1` in {{site.data.keyword.bpshort}} 

        * Release {{site.data.keyword.bpshort}} command-line plug-in 

* [February 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-feb22)

    * Review the release notes for February 2022.

    * [16 February 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-feb1622)

        * Release {{site.data.keyword.bpshort}} command-line plug-in 

        * Supports installer for Linux&trade; arm64 and Mac OS arm64 binaries 

    * [11 February 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-feb1122)

        * Release {{site.data.keyword.bpshort}} command-line plug-in 

* [January 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jan22)

    * Review the release notes for January 2022.

    * [31 January 2022](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jan3122)

        * Release {{site.data.keyword.bpshort}} command-line plug-in 

        * Supports installer for PowerLinux&trade; and System/390 Linux&trade; 

* [December 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-dec21)

    * Review the release notes for December 2021.

    * [30 December 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-dec3021)

        * Release {{site.data.keyword.bpshort}} command-line plug-in 

* [November 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-nov21)

    * Review the release notes for November 2021.

    * [30 November 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-nov302021)

        * Centrally manage access tags for {{site.data.keyword.bpshort}} Workspaces in your account

        * Support `WinRM` in user interface

        * Global catalog settings for {{site.data.keyword.bpshort}} Workspaces location

        * About `compact` download

        * About {{site.data.keyword.bpshort}} Job files

        * ResourceQuery attribute deprecated 

* [October 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-oct21)

    * Review the release notes for October 2021.

    * [22 October 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-oct2021)

        * Onboarding Terraform templates to private catalog

        * Sample templates to deploy into {{site.data.keyword.cloud_notm}}

        * Support `WinRM` in command line

        * Documentation lists the Command-line version change log history

* [September 2021](/docs/schematics?topic=schematics-schematics-relnotes#sept30-2021)

    * Review the release notes for September 2021.

    * [30 September 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-sept302021)

        * Inventory target feature support in {{site.data.keyword.bpshort}} Actions API

        * Bastion host enhancement in {{site.data.keyword.bpshort}} Actions API

        * {{site.data.keyword.bpshort}} Actions API enhancement to support bastion host connection with non-root user

        * {{site.data.keyword.bplong_notm}} job queue process

        * {{site.data.keyword.bpshort}} Actions `APIs` enhances the credentials parameter

        * {{site.data.keyword.bpshort}} introduces compact flag in the workspace create and update API

        * Importance of location and URL endpoint in workspace creation

* [August 2021](/docs/schematics?topic=schematics-schematics-relnotes#aug-2021)

    * Review the release notes for August 2021.

    * [27 August 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-aug272021)

        * Workspace update command enhancement

        * Terraform v1.0 support

        * {{site.data.keyword.bplong_notm}} support job queue logs enhancement

    * [11 August 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-aug112021)

        * {{site.data.keyword.bplong_notm}} deprecates older version of Terraform

* [July 2021](/docs/schematics?topic=schematics-schematics-relnotes#july-2021)

    * Review the release notes for July 2021.

    * [30 July 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jul302021)

        * {{site.data.keyword.bplong_notm}} deprecates Terraform v0.11

        * Terraform v0.15 support

        * Ansible v2.9.23 API and command-line support

    * [19 July 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jul192021)

        * Support parallelism and other environment variables in {{site.data.keyword.bplong_notm}}

* [June 2021](/docs/schematics?topic=schematics-schematics-relnotes#june-2021)

    * Review the release notes for June 2021.

    * [30 June 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jun302021)

        * Support taint and untaint feature enhancement in {{site.data.keyword.bplong_notm}}

        * Documentation support to deploy resources in specific region or across multiple region

        * Documentation support to create workspace by using {{site.data.keyword.bplong_notm}} resources

        * One page view to create workspace by using `UI`, `CLI`, `API`, and `Terraform` switcher documentation

        * Temporarily {{site.data.keyword.bplong_notm}} Workspaces stop activity API is deactivated

* [May 2021](/docs/schematics?topic=schematics-schematics-relnotes#may-2021)

    * Review the release notes for May 2021.

    * [26 May 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-may262021)

        * Version constraints support in {{site.data.keyword.bplong_notm}}

        * Troubleshooting guide support

        * {{site.data.keyword.bpshort}} supports sample solutions

* [April 2021](/docs/schematics?topic=schematics-schematics-relnotes#april-2021)

    * Review the release notes for April 2021.

    * [14 April 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-apri142021)

        * Ansible support in {{site.data.keyword.bplong_notm}} is now generally available

* [March 2021](/docs/schematics?topic=schematics-schematics-relnotes#march-2021)

    * Review the release notes for March 2021.

    * [29 March 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-mar142021)

        * Terraform v0.14 support

* [February 2021](/docs/schematics?topic=schematics-schematics-relnotes#feb-2021)

    * Review the release notes for February 2021.

    * [25 February 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-feb252021)

        * {{site.data.keyword.bpshort}} supports the ability to store the user-defined file

        * Allowed file extensions in {{site.data.keyword.bpshort}}

        * {{site.data.keyword.bpshort}} CLI plug-in and commands support in CLI documentation

    * [12 February 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-feb122021)

        * Ansible open beta release

* [January 2021](/docs/schematics?topic=schematics-schematics-relnotes#jan-2021)

    * Review the release notes for January 2021.

    * [29 January 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jan292021)

        * Virtual Private Endpoint Gateways support

    * [20 January 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jan202021)

        * Terraform commands API support

        * Terraform commands command-line support

        * command-line Commands

    * [7 January 2021](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jan072021)

        * Multiple SDK support

* [December 2020](/docs/schematics?topic=schematics-schematics-relnotes#dec-2020)

    * Review the release notes for December 2020.

    * [9 December 2020](/docs/schematics?topic=schematics-schematics-relnotes#schematics-dec92020)

        * Ansible beta release

        * Beta

* [November 2020](/docs/schematics?topic=schematics-schematics-relnotes#nov-2020)

    * Review the release notes for November 2020.

    * [25 November 2020](/docs/schematics?topic=schematics-schematics-relnotes#schematics-dec252020)

        * Terraform v0.13 support

* [October 2020](/docs/schematics?topic=schematics-schematics-relnotes#oct-2020)

    * Review the release notes for October 2020.

    * [16 October 2020](/docs/schematics?topic=schematics-schematics-relnotes#schematics-oct162020)

        * Monitoring

        * Files and resources for your workspace actions

        * Creating a deploy to {{site.data.keyword.bplong_notm}} link

* [September 2020](/docs/schematics?topic=schematics-schematics-relnotes#sept-2020)

    * Review the release notes for September 2020.

    * [11 September 2020](/docs/schematics?topic=schematics-schematics-relnotes#schematics-sept112020)

        * `Bitbucket` supports private repository

        * Support to override the default variable

* [August 2020](/docs/schematics?topic=schematics-schematics-relnotes#aug-2020)

    * Review the release notes for August 2020.

    * [14 August 2020](/docs/schematics?topic=schematics-schematics-relnotes#schematics-aug142020)

        * Support for multiple Terraform provider

        * Time out set for local-exec and remote-exec users

        * `Bitbucket` is used as a template repository source

* [July 2020](/docs/schematics?topic=schematics-schematics-relnotes#jul-2020)

    * Review the release notes for July 2020.

    * [9 July 2020](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jul92020)

        * Stop apply support

        * New {{site.data.keyword.bpshort}} locations

* [June 2020](/docs/schematics?topic=schematics-schematics-relnotes#jun-2020)

    * Review the release notes for June 2020.

    * [26 June 2020](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jun262020)

        * Ansible provisioner support

    * [25 June 2020](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jun252020)

        * Version 1.8.0 of the {{site.data.keyword.cloud_notm}} Provider plug-in available

    * [22 June 2020](/docs/schematics?topic=schematics-schematics-relnotes#schematics-jun222020)

        * Upload Terraform templates as TAR files

* [May 2020](/docs/schematics?topic=schematics-schematics-relnotes#may-2020)

    * Review the release notes for May 2020.

    * [8 May 2020](/docs/schematics?topic=schematics-schematics-relnotes#schematics-may82020)

        * New EU API endpoint

* [April 2020](/docs/schematics?topic=schematics-schematics-relnotes#april-2020)

    * Review the release notes for April 2020.

    * [17 April 2020](/docs/schematics?topic=schematics-schematics-relnotes#schematics-apr172020)

        * Terraform v0.12 support

        * New workspace creation flow


## Setting up the CLI and API
{: #sitemap_setting_up_the_cli_and_api}


[Setting up the CLI](/docs/schematics?topic=schematics-setup-cli#setup-cli)

* [Installing the {{site.data.keyword.cloud_notm}} command-line](/docs/schematics?topic=schematics-setup-cli#install-schematics-cli)

* [Installing the {{site.data.keyword.bplong_notm}} command-line plug-in](/docs/schematics?topic=schematics-setup-cli#install-schematics-plugin)

* [Updating the CLI](/docs/schematics?topic=schematics-setup-cli#schematics-cli-update)

* [Uninstalling the {{site.data.keyword.bplong_notm}} command-line plug-in](/docs/schematics?topic=schematics-setup-cli#uninstall-schematics-plugin)

[Setting up the API](/docs/schematics?topic=schematics-setup-api#setup-api)

* [Automating deployments with the API](/docs/schematics?topic=schematics-setup-api#cs_api)

* [Refreshing {{site.data.keyword.cloud_notm}} IAM access tokens and obtaining new refresh tokens with the API](/docs/schematics?topic=schematics-setup-api#api_refresh)

* [Table1](/docs/schematics?topic=schematics-setup-api#table1)


## Managing Blueprints
{: #sitemap_managing_blueprints}


[Understanding blueprint templates and configuration](/docs/schematics?topic=schematics-blueprint-templates#blueprint-templates)

* [Blueprint configuration](/docs/schematics?topic=schematics-blueprint-templates#blueprint-temp-config)

* [Blueprint template overview](/docs/schematics?topic=schematics-blueprint-templates#template-overview)

    * [Blueprint template YAML file](/docs/schematics?topic=schematics-blueprint-templates#blueprint-yaml-file)

    * [Template inputs](/docs/schematics?topic=schematics-blueprint-templates#blueprint-input-statements)

    * [Template outputs](/docs/schematics?topic=schematics-blueprint-templates#blueprint-output)

    * [Module definitions](/docs/schematics?topic=schematics-blueprint-templates#blueprint-module)

* [Input files](/docs/schematics?topic=schematics-blueprint-templates#blueprint-input-file)

* [Dynamic inputs](/docs/schematics?topic=schematics-blueprint-templates#blueprint-dynamic-input)

* [What's next?](/docs/schematics?topic=schematics-blueprint-templates#bp-def-whatsnext)

[Using Terraform modules with blueprint templates](/docs/schematics?topic=schematics-blueprint-terraform#blueprint-terraform)

* [Root modules and Terraform configurations](/docs/schematics?topic=schematics-blueprint-terraform#blueprint-root-module-config)

* [Child and reusable shared modules](/docs/schematics?topic=schematics-blueprint-terraform#blueprint-reusable-module)

* [Blueprints provider injection](/docs/schematics?topic=schematics-blueprint-terraform#bp-provider-injection)

    * [Templating Terraform language statements](/docs/schematics?topic=schematics-blueprint-terraform#blueprint-template-statement)

    * [Configuring provider injection](/docs/schematics?topic=schematics-blueprint-terraform#blueprint-provider-injection)

* [Next steps](/docs/schematics?topic=schematics-blueprint-terraform#bp-terraform-nextsteps)

[Reuse and customization](/docs/schematics?topic=schematics-blueprint-reuse#blueprint-reuse)

* [Reuse across environments](/docs/schematics?topic=schematics-blueprint-reuse#blueprint-reuse-env)

    * [Deployment pipelines](/docs/schematics?topic=schematics-blueprint-reuse#blueprint-pipelines)

* [Customization best practice](/docs/schematics?topic=schematics-blueprint-reuse#blueprint-customization-bp)

    * [Blueprint customization](/docs/schematics?topic=schematics-blueprint-reuse#blueprint-customization)

* [Customizing environments with inputs](/docs/schematics?topic=schematics-blueprint-reuse#blueprint-customization-layers)

* [Using versioned inputs](/docs/schematics?topic=schematics-blueprint-reuse#bp-version-input)

* [Blueprint input value precedence](/docs/schematics?topic=schematics-blueprint-reuse#blueprint-input-precedence)

    * [No value](/docs/schematics?topic=schematics-blueprint-reuse#bp-precedence-novalue)

    * [Default value](/docs/schematics?topic=schematics-blueprint-reuse#bp-precedence-defaultvalue)

    * [Specified value](/docs/schematics?topic=schematics-blueprint-reuse#bp-precedence-specifiedvalue)

[Versioning blueprint environments](/docs/schematics?topic=schematics-blueprint-versioning#blueprint-versioning)

* [Relaxed versioning](/docs/schematics?topic=schematics-blueprint-versioning#update-blueprint-relaxed)

    * [Creating environments using relaxed versioning](/docs/schematics?topic=schematics-blueprint-versioning#bp-relaxed-version)

    * [Updating an un-versioned environment](/docs/schematics?topic=schematics-blueprint-versioning#bp-un-versioned-env)

    * [Migrating to a versioned configuration](/docs/schematics?topic=schematics-blueprint-versioning#bp-versioned-env)

* [Explicit versioning](/docs/schematics?topic=schematics-blueprint-versioning#update-blueprint-strict)

    * [Specifying versioning at create time](/docs/schematics?topic=schematics-blueprint-versioning#bp-version-create-time)

    * [Specifying versions at update time](/docs/schematics?topic=schematics-blueprint-versioning#bp-version-update-time)

[Editing blueprint templates](/docs/schematics?topic=schematics-edit-blueprints#edit-blueprints)

* [Configure your VSCode environment](/docs/schematics?topic=schematics-edit-blueprints#bp-config-vscode)

* [Sourcing a blueprint template](/docs/schematics?topic=schematics-edit-blueprints#bp-select-template)

* [Clone source template repo in Git](/docs/schematics?topic=schematics-edit-blueprints#bp-clone-repo)

* [Clone repo to local machine](/docs/schematics?topic=schematics-edit-blueprints#bp-clone-repo-local)

* [Editing in VSCode](/docs/schematics?topic=schematics-edit-blueprints#bp-edit-vscode)

    * [Blueprint usage and configuration documentation](/docs/schematics?topic=schematics-edit-blueprints#bp-usage-config-doc)

    * [Push edited template](/docs/schematics?topic=schematics-edit-blueprints#bp-push-template)

* [Next steps](/docs/schematics?topic=schematics-edit-blueprints#bp-edit-nextsteps)

[Create a blueprint configuration](/docs/schematics?topic=schematics-create-blueprint-config#create-blueprint-config)

* [Creating a blueprint configuration through the CLI](/docs/schematics?topic=schematics-create-blueprint-config#create-blueprint-cli)

    * [Verifying blueprint config creation](/docs/schematics?topic=schematics-create-blueprint-config#verify-blueprint-create-cli)

* [Creating a blueprint configuration using the UI](/docs/schematics?topic=schematics-create-blueprint-config#bp-ui-create)

    * [Verifying blueprint config creation using the UI](/docs/schematics?topic=schematics-create-blueprint-config#verify-blueprint-create-ui)

* [Creating a blueprint configuration using the API](/docs/schematics?topic=schematics-create-blueprint-config#create-blueprint-api)

    * [Verifying blueprint create using the API](/docs/schematics?topic=schematics-create-blueprint-config#verify-bp-create-api)

* [Next steps](/docs/schematics?topic=schematics-create-blueprint-config#bp-create-nextsteps)

[Update a blueprint configuration](/docs/schematics?topic=schematics-update-blueprint#update-blueprint)

* [Update process](/docs/schematics?topic=schematics-update-blueprint#update-blueprint-process)

* [Updating a blueprint through CLI](/docs/schematics?topic=schematics-update-blueprint#update-blueprint-cli)

    * [Verifying blueprint update](/docs/schematics?topic=schematics-update-blueprint#verify-update)

* [Updating a blueprint environment using the UI](/docs/schematics?topic=schematics-update-blueprint#update-blueprint-ui)

    * [Verify blueprint update using the UI](/docs/schematics?topic=schematics-update-blueprint#verify-bp-update-ui)

* [Updating a blueprint using the API](/docs/schematics?topic=schematics-update-blueprint#update-blueprint-api)

    * [Verify blueprint create using the API](/docs/schematics?topic=schematics-update-blueprint#verify-bp-update-api)

* [Next steps](/docs/schematics?topic=schematics-update-blueprint#bp-update-nextsteps)

[Apply blueprint config changes to an environment](/docs/schematics?topic=schematics-apply-blueprint#apply-blueprint)

* [Running a blueprint apply through CLI](/docs/schematics?topic=schematics-apply-blueprint#apply-blueprint-cli)

    * [Verify blueprint run apply success](/docs/schematics?topic=schematics-apply-blueprint#bp-verify-apply-cli)

* [Generate and apply blueprint environment through UI](/docs/schematics?topic=schematics-apply-blueprint#apply-blueprint-ui)

    * [Verify blueprint apply operation through UI](/docs/schematics?topic=schematics-apply-blueprint#bp-verify-apply-ui)

* [Applying a blueprint using the API](/docs/schematics?topic=schematics-apply-blueprint#apply-blueprint-api)

    * [Verify Blueprint apply job through API](/docs/schematics?topic=schematics-apply-blueprint#bp-verify-apply-api)

* [Next steps](/docs/schematics?topic=schematics-apply-blueprint#bp-apply-nextsteps)

[Displaying blueprints](/docs/schematics?topic=schematics-list-blueprint#list-blueprint)

* [Displaying blueprints using the UI](/docs/schematics?topic=schematics-list-blueprint#display-blueprint-ui)

* [Displaying blueprints using the CLI](/docs/schematics?topic=schematics-list-blueprint#listing-bp-cli)

    * [Displaying blueprint details](/docs/schematics?topic=schematics-list-blueprint#display-blueprint-cli)

    * [Get blueprint summary](/docs/schematics?topic=schematics-list-blueprint#display-blueprint-summary)

    * [Get blueprint outputs](/docs/schematics?topic=schematics-list-blueprint#display-blueprint-outputs-cli)

    * [Get blueprint module details](/docs/schematics?topic=schematics-list-blueprint#display-blueprint-summary-cli)

* [Displaying blueprint using the API](/docs/schematics?topic=schematics-list-blueprint#display-blueprint-api)

* [Next steps](/docs/schematics?topic=schematics-list-blueprint#bp-display-nextsteps)

[Displaying blueprint jobs](/docs/schematics?topic=schematics-list-blueprint-jobs#list-blueprint-jobs)

* [Viewing blueprint job results using the UI](/docs/schematics?topic=schematics-list-blueprint-jobs#blueprint-job-get-ui)

* [Listing blueprint jobs using the CLI](/docs/schematics?topic=schematics-list-blueprint-jobs#list-blueprint-cli)

* [Viewing blueprint job results using the CLI](/docs/schematics?topic=schematics-list-blueprint-jobs#view-blueprint-job-get-cli)

    * [Blueprint job get](/docs/schematics?topic=schematics-list-blueprint-jobs#blueprint-job-get-cli)

    * [Blueprint job get summary log](/docs/schematics?topic=schematics-list-blueprint-jobs#blueprint-job-get-drilldown-cli)

    * [Viewing blueprint job logs](/docs/schematics?topic=schematics-list-blueprint-jobs#blueprint-job-log-cli)

* [List blueprint jobs using the UI](/docs/schematics?topic=schematics-list-blueprint-jobs#list-blueprint-jobs-ui)

* [Listing blueprints using the API](/docs/schematics?topic=schematics-list-blueprint-jobs#list-blueprint-api)

    * [Verifying blueprint job results using the API](/docs/schematics?topic=schematics-list-blueprint-jobs#bp-verify-jobs-api)

* [Next steps](/docs/schematics?topic=schematics-list-blueprint-jobs#bp-job-nextsteps)

[Destroy a blueprint environment](/docs/schematics?topic=schematics-destroy-blueprint#destroy-blueprint)

* [Destroying a blueprint environment using the UI](/docs/schematics?topic=schematics-destroy-blueprint#destroy-blueprint-ui)

    * [Verifying blueprint environment destroy](/docs/schematics?topic=schematics-destroy-blueprint#verify-bp-destroy-ui)

* [Destroying a blueprint environment using the CLI](/docs/schematics?topic=schematics-destroy-blueprint#destroy-blueprint-cli)

    * [Verifying blueprint destroy success](/docs/schematics?topic=schematics-destroy-blueprint#verify-bp-destroy-cli)

* [Destroying blueprint environment using the API](/docs/schematics?topic=schematics-destroy-blueprint#destroy-blueprint-api)

    * [Verifying blueprint destroy using the API](/docs/schematics?topic=schematics-destroy-blueprint#bp-verify-display-api)

* [Next steps](/docs/schematics?topic=schematics-destroy-blueprint#bp-destroy-nextsteps)

[Delete a blueprint configuration](/docs/schematics?topic=schematics-delete-blueprint#delete-blueprint)

* [Deleting a blueprint config using the CLI](/docs/schematics?topic=schematics-delete-blueprint#delete-blueprint-cli)

    * [Verifying blueprint config deletion](/docs/schematics?topic=schematics-delete-blueprint#verify-bp-delete-cli)

* [Deleting a blueprint config using the UI](/docs/schematics?topic=schematics-delete-blueprint#delete-blueprint-ui)

    * [Verifying blueprint config deletion](/docs/schematics?topic=schematics-delete-blueprint#verify-bp-deletion-ui)

* [Deleting a blueprint config using the API](/docs/schematics?topic=schematics-delete-blueprint#delete-blueprint-api)

    * [Verifying blueprint delete using the API](/docs/schematics?topic=schematics-delete-blueprint#verify-bp-delete-api)

* [Next steps](/docs/schematics?topic=schematics-delete-blueprint#bp-delete-nextsteps)

[Creating blueprints via the CLI using a config file](/docs/schematics?topic=schematics-create-blueprint-file#create-blueprint-file)

* [Using a config file](/docs/schematics?topic=schematics-create-blueprint-file#bp-create-config)

* [Defining a JSON config file](/docs/schematics?topic=schematics-create-blueprint-file#bp-create-configJSON)

[Using environment variables with blueprints](/docs/schematics?topic=schematics-bp-env-vars#bp-env-vars)

* [Blueprints usage](/docs/schematics?topic=schematics-bp-env-vars#usage)


## Managing Workspaces New
{: #sitemap_managing_workspaces_new}



### Creating workspace
{: #sitemap_creating_workspace}


[Creating workspaces and importing your Terraform template](/docs/schematics?topic=schematics-sch-create-wks#sch-create-wks)

* [Before you begin](/docs/schematics?topic=schematics-sch-create-wks#prerequisites-create)

* [Creating the workspace through UI](/docs/schematics?topic=schematics-sch-create-wks#create-wks-ui)

* [Creating the workspace through CLI](/docs/schematics?topic=schematics-sch-create-wks#create-wks-cli)

* [Creating the workspace through API](/docs/schematics?topic=schematics-sch-create-wks#create-wks-api)

* [Creating the workspace with Terraform](/docs/schematics?topic=schematics-sch-create-wks#create-wks-terraform)

* [Next steps](/docs/schematics?topic=schematics-sch-create-wks#sch-create-wks-nextsteps)

[Creating Terraform templates](/docs/schematics?topic=schematics-create-tf-config#create-tf-config)

* [Configuring the `provider` block](/docs/schematics?topic=schematics-create-tf-config#configure-provider)

* [Adding {{site.data.keyword.cloud_notm}} resources to the `resource` block](/docs/schematics?topic=schematics-create-tf-config#configure-resources)

    * [Referencing resources in other resource blocks](/docs/schematics?topic=schematics-create-tf-config#reference-resource-info)

* [Managing resources in other account](/docs/schematics?topic=schematics-create-tf-config#manage-resource-account)

* [Using `variable` blocks to customize resources](/docs/schematics?topic=schematics-create-tf-config#configure-variables)

    * [Referencing variables](/docs/schematics?topic=schematics-create-tf-config#reference-variables)

* [Providing values to {{site.data.keyword.bplong_notm}} for the declared variables](/docs/schematics?topic=schematics-create-tf-config#declare-variable)

    * [Example for list of Strings](/docs/schematics?topic=schematics-create-tf-config#example-list-strings)

    * [Example for list of Objects](/docs/schematics?topic=schematics-create-tf-config#example-list-object)

* [Storing your Terraform templates](/docs/schematics?topic=schematics-create-tf-config#store-template)

[Planning workspace](/docs/schematics?topic=schematics-sch-plan-wks#sch-plan-wks)

* [Before you begin](/docs/schematics?topic=schematics-sch-plan-wks#display-prerequisites)

* [Generate the workspace plan through UI](/docs/schematics?topic=schematics-sch-plan-wks#plan-wks-ui)

    * [Verifying workspace plan](/docs/schematics?topic=schematics-sch-plan-wks#verify-wks-plan-ui)

* [Generate the workspace plan through CLI](/docs/schematics?topic=schematics-sch-plan-wks#plan-wks-cli)

    * [Verifying workspace plan](/docs/schematics?topic=schematics-sch-plan-wks#verify-wks-plan-cli)

* [Generate the workspace plan through API](/docs/schematics?topic=schematics-sch-plan-wks#plan-wks-api)

    * [Verifying workspace plan:](/docs/schematics?topic=schematics-sch-plan-wks#verify-wks-plan-api)

* [Generate the workspace plan with Terraform](/docs/schematics?topic=schematics-sch-plan-wks#plan-wks-terraform)

* [Next steps](/docs/schematics?topic=schematics-sch-plan-wks#sch-plan-wks-nextsteps)

[Deploying workspace](/docs/schematics?topic=schematics-sch-deploy-wks#sch-deploy-wks)

* [Before you begin](/docs/schematics?topic=schematics-sch-deploy-wks#display-prerequisites)

* [Generate the workspace deployment through UI](/docs/schematics?topic=schematics-sch-deploy-wks#deploy-wks-ui)

    * [Verifying workspace deployment](/docs/schematics?topic=schematics-sch-deploy-wks#verify-wks-list-ui)

* [Generate the workspace deployment through CLI](/docs/schematics?topic=schematics-sch-deploy-wks#deploy-wks-cli)

    * [Verifying workspace deploy](/docs/schematics?topic=schematics-sch-deploy-wks#verify-wks-deploy-cli)

* [Generate the workspace deploy through API](/docs/schematics?topic=schematics-sch-deploy-wks#deploy-wks-api)

    * [Verifying workspace deploy](/docs/schematics?topic=schematics-sch-deploy-wks#verify-wks-deploy-api)

* [Generate the workspace deploy with Terraform](/docs/schematics?topic=schematics-sch-deploy-wks#deploy-wks-terraform)

* [Next steps](/docs/schematics?topic=schematics-sch-deploy-wks#sch-deploy-wks-nextsteps)

[Updating workspace](/docs/schematics?topic=schematics-sch-update-wks#sch-update-wks)

* [Before you begin](/docs/schematics?topic=schematics-sch-update-wks#update-prerequisites)

* [Updating the workspace through UI](/docs/schematics?topic=schematics-sch-update-wks#update-wks-ui)

    * [Verifying workspace update](/docs/schematics?topic=schematics-sch-update-wks#verify-wks-update-ui)

* [Updating the workspace through CLI](/docs/schematics?topic=schematics-sch-update-wks#update-wks-cli)

    * [Verifying workspace update](/docs/schematics?topic=schematics-sch-update-wks#verify-wks-update-cli)

* [Updating the workspace through API](/docs/schematics?topic=schematics-sch-update-wks#update-wks-api)

    * [Verifying workspace update](/docs/schematics?topic=schematics-sch-update-wks#verify-wks-update-api)

* [Updating the workspace with Terraform](/docs/schematics?topic=schematics-sch-update-wks#update-wks-terraform)

* [Next steps](/docs/schematics?topic=schematics-sch-update-wks#sch-update-wks-nextsteps)

[Displaying workspace](/docs/schematics?topic=schematics-sch-display-wks#sch-display-wks)

* [Before you begin](/docs/schematics?topic=schematics-sch-display-wks#display-prerequisites)

* [Displaying the workspace through UI](/docs/schematics?topic=schematics-sch-display-wks#list-wks-ui)

    * [Verifying workspace display](/docs/schematics?topic=schematics-sch-display-wks#verify-wks-list-ui)

* [Displaying the workspace through CLI](/docs/schematics?topic=schematics-sch-display-wks#list-wks-cli)

    * [Verifying workspace list](/docs/schematics?topic=schematics-sch-display-wks#verify-wks-list-cli)

* [Displaying the workspace list through API](/docs/schematics?topic=schematics-sch-display-wks#list-wks-api)

    * [verifying workspace update:](/docs/schematics?topic=schematics-sch-display-wks#verify-wks-list-api)

* [Displaying the workspace list with Terraform](/docs/schematics?topic=schematics-sch-display-wks#list-wks-terraform)

* [Next steps](/docs/schematics?topic=schematics-sch-display-wks#sch-list-wks-nextsteps)

[Destroying workspace](/docs/schematics?topic=schematics-sch-destroy-wks#sch-destroy-wks)

* [Before you begin](/docs/schematics?topic=schematics-sch-destroy-wks#prerequisites-destroy)

* [Destroying the workspace through UI](/docs/schematics?topic=schematics-sch-destroy-wks#destroy-wks-ui)

    * [Verifying blueprint environment destroy](/docs/schematics?topic=schematics-sch-destroy-wks#verify-wks-destroy-ui)

* [Destroying the workspace through CLI](/docs/schematics?topic=schematics-sch-destroy-wks#destroy-wks-cli)

    * [Verifying workspace destroy](/docs/schematics?topic=schematics-sch-destroy-wks#verify-workspace-destroy-cli)

* [Destroying the workspace through API](/docs/schematics?topic=schematics-sch-destroy-wks#destroy-wks-api)

    * [Verifying workspace destroy](/docs/schematics?topic=schematics-sch-destroy-wks#verify-workspace-destroy-api)

* [destroying the workspace with Terraform](/docs/schematics?topic=schematics-sch-destroy-wks#destroy-wks-terraform)

* [Next steps](/docs/schematics?topic=schematics-sch-destroy-wks#sch-destroy-wks-nextsteps)

[Deleting workspace](/docs/schematics?topic=schematics-sch-delete-wks#sch-delete-wks)

* [Before you begin](/docs/schematics?topic=schematics-sch-delete-wks#prerequisites-delete)

* [Deleting the workspace through UI](/docs/schematics?topic=schematics-sch-delete-wks#delete-wks-ui)

    * [Verifying workspace delete](/docs/schematics?topic=schematics-sch-delete-wks#verify-wks-delete-ui)

* [Deleting the workspace through CLI](/docs/schematics?topic=schematics-sch-delete-wks#delete-wks-cli)

    * [Verifying workspace delete](/docs/schematics?topic=schematics-sch-delete-wks#verify-wks-delete-cli)

* [Deleting the workspace through API](/docs/schematics?topic=schematics-sch-delete-wks#delete-wks-api)

    * [Verifying workspace delete](/docs/schematics?topic=schematics-sch-delete-wks#verify-wks-delete-api)

* [Deleting the workspace with Terraform](/docs/schematics?topic=schematics-sch-delete-wks#delete-wks-terraform)

* [Next steps](/docs/schematics?topic=schematics-sch-delete-wks#sch-delete-wks-nextsteps)


### Managing workspace resources
{: #sitemap_managing_workspace_resources}


[Detecting drift in workspaces](/docs/schematics?topic=schematics-drift-note#drift-note)

* [Example drift scenario](/docs/schematics?topic=schematics-drift-note#drift-scenario)

* [Drift detection in {{site.data.keyword.cloud_notm}}](/docs/schematics?topic=schematics-drift-note#drift-in-ibm)

* [Drift detection through {{site.data.keyword.bpshort}} UI](/docs/schematics?topic=schematics-drift-note#drift-ui)

    * [Viewing detect drift through UI](/docs/schematics?topic=schematics-drift-note#drift-view-ui)

* [Drift detection through {{site.data.keyword.bpshort}} CLI](/docs/schematics?topic=schematics-drift-note#drift-cli)

    * [Creating and viewing the detect drift through CLI](/docs/schematics?topic=schematics-drift-note#drift-view-cli)

* [Creating and viewing the detect drift through API](/docs/schematics?topic=schematics-drift-note#drift-api)

[Remote state and cross-workspace access](/docs/schematics?topic=schematics-remote-state#remote-state)

* [Accessing workspace state and outputs](/docs/schematics?topic=schematics-remote-state#data-sources)


## Managing Workspaces
{: #sitemap_managing_workspaces}


[Creating Terraform templates](/docs/schematics?topic=schematics-create-tf-config#create-tf-config)

* [Configuring the `provider` block](/docs/schematics?topic=schematics-create-tf-config#configure-provider)

* [Adding {{site.data.keyword.cloud_notm}} resources to the `resource` block](/docs/schematics?topic=schematics-create-tf-config#configure-resources)

    * [Referencing resources in other resource blocks](/docs/schematics?topic=schematics-create-tf-config#reference-resource-info)

* [Managing resources in other account](/docs/schematics?topic=schematics-create-tf-config#manage-resource-account)

* [Using `variable` blocks to customize resources](/docs/schematics?topic=schematics-create-tf-config#configure-variables)

    * [Referencing variables](/docs/schematics?topic=schematics-create-tf-config#reference-variables)

* [Providing values to {{site.data.keyword.bplong_notm}} for the declared variables](/docs/schematics?topic=schematics-create-tf-config#declare-variable)

    * [Example for list of Strings](/docs/schematics?topic=schematics-create-tf-config#example-list-strings)

    * [Example for list of Objects](/docs/schematics?topic=schematics-create-tf-config#example-list-object)

* [Storing your Terraform templates](/docs/schematics?topic=schematics-create-tf-config#store-template)

[Setting up workspaces](/docs/schematics?topic=schematics-workspace-setup#workspace-setup)

* [Creating workspaces and importing your Terraform template](/docs/schematics?topic=schematics-workspace-setup#create-workspace)

    * [Before you begin](/docs/schematics?topic=schematics-workspace-setup#prerequisites)

    * [Creating the workspace from the console](/docs/schematics?topic=schematics-workspace-setup#create-workspace_ui)

    * [Creating the workspace through CLI](/docs/schematics?topic=schematics-workspace-setup#create-workspace-cli)

    * [Creating the workspace through API](/docs/schematics?topic=schematics-workspace-setup#create-workspace-api)

    * [Creating the workspace with Terraform](/docs/schematics?topic=schematics-workspace-setup#create-workspace-terraform)

    * [Importing your Terraform template](/docs/schematics?topic=schematics-workspace-setup#import-template)

    * [Running your Terraform template in {{site.data.keyword.cloud_notm}}](/docs/schematics?topic=schematics-workspace-setup#run-template)

* [Freezing and unfreezing workspaces](/docs/schematics?topic=schematics-workspace-setup#lock-workspace)

* [Deleting a workspace](/docs/schematics?topic=schematics-workspace-setup#del-workspace)

* [Planning your workspace](/docs/schematics?topic=schematics-workspace-setup#workspaces-plan)

    * [Designing your workspace and Git repository structure](/docs/schematics?topic=schematics-workspace-setup#structure-workspace)

    * [How many workspaces do I need?](/docs/schematics?topic=schematics-workspace-setup#plan-number-of-workspaces)

    * [How do I structure my Git repository to map my workspaces?](/docs/schematics?topic=schematics-workspace-setup#plan-github-structure)

    * [How can I reuse configuration files across environments and workspaces?](/docs/schematics?topic=schematics-workspace-setup#plan-reuse)

    * [How do I control access to my workspaces?](/docs/schematics?topic=schematics-workspace-setup#plan-workspace-access)

    * [What do I need to be aware of when I have a repository that I managed with native Terraform?](/docs/schematics?topic=schematics-workspace-setup#plan-terraform-migration)

* [Setting up a continuous delivery toolchain for your workspace](/docs/schematics?topic=schematics-workspace-setup#continuous-delivery)

* [Workspace states](/docs/schematics?topic=schematics-workspace-setup#wks-state)

    * [Workspace state overview](/docs/schematics?topic=schematics-workspace-setup#states-overview)

    * [Workspace state diagram and manipulative job](/docs/schematics?topic=schematics-workspace-setup#workspace-state-diagram)

* [Creating an auto deployment to the {{site.data.keyword.bplong_notm}}](/docs/schematics?topic=schematics-workspace-setup#create-deploy-to-schematics)

* [Reviewing the {{site.data.keyword.bpshort}} job details](/docs/schematics?topic=schematics-workspace-setup#job-logs)

[Using shared data sets for workspace variables](/docs/schematics?topic=schematics-shared-dataset#shared-dataset)

* [Creating shared data sets](/docs/schematics?topic=schematics-shared-dataset#create-shared-data)

* [Updating shared data sets](/docs/schematics?topic=schematics-shared-dataset#update-shared-data)

* [Deleting shared data sets](/docs/schematics?topic=schematics-shared-dataset#delete-shared-data)

* [Using shared data sets in a workspace](/docs/schematics?topic=schematics-shared-dataset#using-shared-data)

[Using environment variables with workspaces](/docs/schematics?topic=schematics-set-parallelism#set-parallelism)

* [Usage](/docs/schematics?topic=schematics-set-parallelism#parelleism-usage)

    * [Passing TF_CLI_ARGS](/docs/schematics?topic=schematics-set-parallelism#passing-cli-args)

    * [Example setting parallelism or TF_LOGS](/docs/schematics?topic=schematics-set-parallelism#parallelism-example)

* [List of Terraform environment variables](/docs/schematics?topic=schematics-set-parallelism#list-special-env-vars)

[Detecting drift in workspaces](/docs/schematics?topic=schematics-drift-note#drift-note)

* [Example drift scenario](/docs/schematics?topic=schematics-drift-note#drift-scenario)

* [Drift detection in {{site.data.keyword.cloud_notm}}](/docs/schematics?topic=schematics-drift-note#drift-in-ibm)

* [Drift detection through {{site.data.keyword.bpshort}} UI](/docs/schematics?topic=schematics-drift-note#drift-ui)

    * [Viewing detect drift through UI](/docs/schematics?topic=schematics-drift-note#drift-view-ui)

* [Drift detection through {{site.data.keyword.bpshort}} CLI](/docs/schematics?topic=schematics-drift-note#drift-cli)

    * [Creating and viewing the detect drift through CLI](/docs/schematics?topic=schematics-drift-note#drift-view-cli)

* [Creating and viewing the detect drift through API](/docs/schematics?topic=schematics-drift-note#drift-api)

[Using private repos for modules](/docs/schematics?topic=schematics-download-modules-pvt-git#download-modules-pvt-git)

* [Usage of private module template](/docs/schematics?topic=schematics-download-modules-pvt-git#netrc-example)

[Managing resources with {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-manage-lifecycle#manage-lifecycle)

* [Supporting features](/docs/schematics?topic=schematics-manage-lifecycle#resource-features)

* [Deploying your resources](/docs/schematics?topic=schematics-manage-lifecycle#deploy-resources)

* [Updating your resources](/docs/schematics?topic=schematics-manage-lifecycle#update-resources)

* [Managing drift between your cloud environment and Terraform configuration](/docs/schematics?topic=schematics-manage-lifecycle#drift-report)

* [Reviewing resource and deployment details](/docs/schematics?topic=schematics-manage-lifecycle#review-logs)

* [Removing your resources](/docs/schematics?topic=schematics-manage-lifecycle#destroy-resources)

* [Deploying your resources through CLI](/docs/schematics?topic=schematics-manage-lifecycle#deploy-resources-cli)

* [Updating your resources through CLI](/docs/schematics?topic=schematics-manage-lifecycle#update-resources-cli)

* [Managing drift between your cloud environment and Terraform configuration through CLI](/docs/schematics?topic=schematics-manage-lifecycle#drift-report-cli)

* [Reviewing resource and deployment details through CLI](/docs/schematics?topic=schematics-manage-lifecycle#review-logs-cli)

* [Removing your resources through CLI](/docs/schematics?topic=schematics-manage-lifecycle#destroy-resources-cli)

[Deploying {{site.data.keyword.cloud_notm}} resources in a specific region or across multiple regions](/docs/schematics?topic=schematics-multi-region-deployment#multi-region-deployment)

* [Deploying services in a specific region](/docs/schematics?topic=schematics-multi-region-deployment#single-region)

* [Deploying services across regions](/docs/schematics?topic=schematics-multi-region-deployment#across-regions)

[Deprecating Terraform versions](/docs/schematics?topic=schematics-deprecate-tf-version#deprecate-tf-version)

* [Phases](/docs/schematics?topic=schematics-deprecate-tf-version#deprecate-phase)

* [Schedule](/docs/schematics?topic=schematics-deprecate-tf-version#deprecate-timeline)

* [User actions](/docs/schematics?topic=schematics-deprecate-tf-version#user-action)

[Updating Terraform version](/docs/schematics?topic=schematics-migrating-terraform-version#migrating-terraform-version)

* [Upgrading the Terraform template version 1.x and above](/docs/schematics?topic=schematics-migrating-terraform-version#terraform-version-upgrade1x)

    * [Updating the Workspace Terraform 1.x version](/docs/schematics?topic=schematics-migrating-terraform-version#terraform-version-upgrade1x-process)

* [Upgrading the Terraform template version 0.x to 1.x](/docs/schematics?topic=schematics-migrating-terraform-version#terraform-version-upgrade0x)

* [Upgrading a Terraform v0.12 Workspace to v0.13](/docs/schematics?topic=schematics-migrating-terraform-version#migrate-steps12)

* [Upgrade Terraform template from `v0.13` and higher to `v1.0`](/docs/schematics?topic=schematics-migrating-terraform-version#upgrade-13-to10)

[Remote state and cross-workspace access](/docs/schematics?topic=schematics-remote-state#remote-state)

* [Accessing workspace state and outputs](/docs/schematics?topic=schematics-remote-state#data-sources)

[Sample Terraform solutions](/docs/schematics?topic=schematics-sol-overview#sol-overview)

[Compact config repo download](/docs/schematics?topic=schematics-compact-download#compact-download)

* [Using compact download](/docs/schematics?topic=schematics-compact-download#compact-active)

* [Note](/docs/schematics?topic=schematics-compact-download#compact-note)

[Downloading workspace job files](/docs/schematics?topic=schematics-job-download#job-download)

* [Workspace job execution](/docs/schematics?topic=schematics-job-download#wks-job-execution)

* [Note](/docs/schematics?topic=schematics-job-download#job-note)

[Stopping or terminating running jobs](/docs/schematics?topic=schematics-interrupt-job#interrupt-job)

* [Stopping job types](/docs/schematics?topic=schematics-interrupt-job#interrupt-types)

* [Canceling a job](/docs/schematics?topic=schematics-interrupt-job#cancelling)

* [Stopping a running job through UI](/docs/schematics?topic=schematics-interrupt-job#stop-job-ui)

* [Stopping a running job through CLI](/docs/schematics?topic=schematics-interrupt-job#stop-job-cli)

* [Stopping a running job through API](/docs/schematics?topic=schematics-interrupt-job#stop-job-api)

    * [Syntax to stop running jobs](/docs/schematics?topic=schematics-interrupt-job#stop-jobs-api)


## Managing Actions
{: #sitemap_managing_actions}


[Creating Ansible roles and galaxy](/docs/schematics?topic=schematics-ansible-roles-galaxy#ansible-roles-galaxy)

* [Creating your own roles in Ansible](/docs/schematics?topic=schematics-ansible-roles-galaxy#main-file)

* [Installing roles from Ansible Galaxy](/docs/schematics?topic=schematics-ansible-roles-galaxy#requirements-file)

[Working with {{site.data.keyword.bpshort}} Actions](/docs/schematics?topic=schematics-action-working#action-working)

* [Creating and running a {{site.data.keyword.bpshort}} action](/docs/schematics?topic=schematics-action-working#create-action)

    * [Prerequisites](/docs/schematics?topic=schematics-action-working#action-working-prereq)

    * [To create an action](/docs/schematics?topic=schematics-action-working#create-action-working)

* [Editing the {{site.data.keyword.bpshort}} Actions settings](/docs/schematics?topic=schematics-action-working#action-settings)

* [Deleting an action](/docs/schematics?topic=schematics-action-working#delete-ansible-actions)

* [Action state](/docs/schematics?topic=schematics-action-working#action-state-diagram)

    * [State diagram flow](/docs/schematics?topic=schematics-action-working#state-diagram-flow)

* [Reviewing Actions job details](/docs/schematics?topic=schematics-action-working#action-jobs)

[Creating an Ansible playbook](/docs/schematics?topic=schematics-create-playbook#create-playbook)

* [Referencing Ansible collections in your playbook](/docs/schematics?topic=schematics-create-playbook#schematics-collections)

* [Preparing your Ansible playbook to run in {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-create-playbook#plan-ansible-playbook)

[Sample Ansible playbook templates for {{site.data.keyword.bpshort}} Actions](/docs/schematics?topic=schematics-sample_actiontemplates#sample_actiontemplates)

* [Running cloud operations on {{site.data.keyword.vsi_is_short}}](/docs/schematics?topic=schematics-sample_actiontemplates#ansible-vpc)

* [Provisioning a LAMP stack on {{site.data.keyword.vsi_is_short}}](/docs/schematics?topic=schematics-sample_actiontemplates#ansible-lamp-stack)

* [Configuring {{site.data.keyword.databases-for-postgresql_full_notm}} with WAL2JSON plug-in](/docs/schematics?topic=schematics-sample_actiontemplates#ansible-databases)

* [Automating app deployments in {{site.data.keyword.containerfull_notm}}](/docs/schematics?topic=schematics-sample_actiontemplates#ansible-iks-deploy)

* [Installing `kubectl` on {{site.data.keyword.vsi_is_short}}](/docs/schematics?topic=schematics-sample_actiontemplates#ansible-kubectl)

[Creating an auto deploy button for {{site.data.keyword.bpshort}} Actions](/docs/schematics?topic=schematics-auto-deploy-url#auto-deploy-url)

* [Creating the deployment URL](/docs/schematics?topic=schematics-auto-deploy-url#create-url)

* [Adding the button to a website or page](/docs/schematics?topic=schematics-auto-deploy-url#add_an_image)

    * [Adding the button in HTML](/docs/schematics?topic=schematics-auto-deploy-url#add-button-html)

    * [Adding the button in Markdown](/docs/schematics?topic=schematics-auto-deploy-url#add-button-markdown)

* [Next steps](/docs/schematics?topic=schematics-auto-deploy-url#sample-actions-nextsteps)

[Onboarding Terraform templates into {{site.data.keyword.cloud_notm}} private catalog](/docs/schematics?topic=schematics-onboard-pvt-catalog#onboard-pvt-catalog)

* [About {{site.data.keyword.bpshort}} Actions](/docs/schematics?topic=schematics-onboard-pvt-catalog#abt-bulkonbaord-action)

* [About {{site.data.keyword.bpshort}} Actions playbook](/docs/schematics?topic=schematics-onboard-pvt-catalog#abt-bulkonboard-playbook)

* [About automation script](/docs/schematics?topic=schematics-onboard-pvt-catalog#abt-bulkonboard-script)

* [About clickable button](/docs/schematics?topic=schematics-onboard-pvt-catalog#abt-button)

* [Running bulk onboard of Terraform templates into {{site.data.keyword.cloud_notm}} private catalog](/docs/schematics?topic=schematics-onboard-pvt-catalog#ansible-bulkonboarding)


## Managing Inventories
{: #sitemap_managing_inventories}


[Creating resource inventories for {{site.data.keyword.bpshort}} Actions](/docs/schematics?topic=schematics-inventories-setup#inventories-setup)

* [Creating static inventory files](/docs/schematics?topic=schematics-inventories-setup#static-inv)

    * [File format](/docs/schematics?topic=schematics-inventories-setup#inv-file-format)

    * [Limitations](/docs/schematics?topic=schematics-inventories-setup#inv-file-limitation)

* [Dynamically building resource inventories from {{site.data.keyword.bpshort}} Workspaces](/docs/schematics?topic=schematics-inventories-setup#dynamic-inv)

    * [Supported resource queries](/docs/schematics?topic=schematics-inventories-setup#supported-queries)

    * [Limitations](/docs/schematics?topic=schematics-inventories-setup#dynamic-inv-limitation)


## Managing Integrations
{: #sitemap_managing_integrations}


[Logging integration](/docs/schematics?topic=schematics-logging-integration#logging-integration)

* [Launching logging](/docs/schematics?topic=schematics-logging-integration#logging-ui)

[{{site.data.keyword.monitoringshort_notm}} integration](/docs/schematics?topic=schematics-monitoring-integration#monitoring-integration)

* [Launching monitoring](/docs/schematics?topic=schematics-monitoring-integration#monitoring-ui)

[Activity tracking integration](/docs/schematics?topic=schematics-at-integration#at-integration)

* [Launching activity tracking](/docs/schematics?topic=schematics-at-integration#audit-ui)

[KMS integration for BYOK or KYOK](/docs/schematics?topic=schematics-kms-integration#kms-integration)

* [Launching key management](/docs/schematics?topic=schematics-kms-integration#key-mgt-ui)

    * [Prerequisites](/docs/schematics?topic=schematics-kms-integration#kms-key-prerequisites)

    * [Enabling {{site.data.keyword.keymanagementservicelong_notm}} through UI](/docs/schematics?topic=schematics-kms-integration#integrate-byok-ui)

    * [Enabling {{site.data.keyword.keymanagementservicelong_notm}} through CLI](/docs/schematics?topic=schematics-kms-integration#integrate-byok-cli)


## Managing Agents Beta
{: #sitemap_managing_agents_beta}


[Installing {{site.data.keyword.bpshort}} Agent](/docs/schematics?topic=schematics-agents-setup#agents-setup)

* [Prerequisites](/docs/schematics?topic=schematics-agents-setup#agents-setup-prereq)

* [Provision the Agent infrastructure through UI](/docs/schematics?topic=schematics-agents-setup#agents-setup-infra-ui)

    * [Expected outcome](/docs/schematics?topic=schematics-agents-setup#agents-setup-infra-output)

    * [Deploying the Agent services](/docs/schematics?topic=schematics-agents-setup#agents-setup-svc)

* [Provision the Agent infrastructure through CLI](/docs/schematics?topic=schematics-agents-setup#agents-setup-infra-cli)

    * [Deploying the Agent services through CLI](/docs/schematics?topic=schematics-agents-setup#agents-setup-svc-cli)

* [Provision the Agent infrastructure through API](/docs/schematics?topic=schematics-agents-setup#agents-setup-infra-api)

    * [Deploying the Agent services](/docs/schematics?topic=schematics-agents-setup#agents-setup-svc-api)

* [Next steps](/docs/schematics?topic=schematics-agents-setup#nextsteps-agentsetup)

[Connecting {{site.data.keyword.bpshort}} Agent](/docs/schematics?topic=schematics-register-agent#register-agent)

* [Connecting Agent through UI](/docs/schematics?topic=schematics-register-agent#register-ui)

* [Connecting Agent through API](/docs/schematics?topic=schematics-register-agent#register-api)

* [Next steps](/docs/schematics?topic=schematics-register-agent#connect-nextsteps)

[Using {{site.data.keyword.bpshort}} Agent](/docs/schematics?topic=schematics-using-agent#using-agent)

* [Steps to Bind an existing workspace to the Agent](/docs/schematics?topic=schematics-using-agent#steps-bind-exist-wks)

* [Steps to Bind a new workspace to the Agent](/docs/schematics?topic=schematics-using-agent#steps-bind-new-wks)

* [Validate the Job execution by the Agent](/docs/schematics?topic=schematics-using-agent#validate-agent-job)

* [Next steps](/docs/schematics?topic=schematics-using-agent#agent-using-nextsteps)

[Uninstalling {{site.data.keyword.bpshort}} Agents](/docs/schematics?topic=schematics-uninstall-agent#uninstall-agent)

* [Clean up Agent infrastructure](/docs/schematics?topic=schematics-uninstall-agent#cleanup-agent-infra)

* [Clean up Agent service](/docs/schematics?topic=schematics-uninstall-agent#cleanup-agent-service)


### Customizing Agents
{: #sitemap_customizing_agents}


[Managing network policies](/docs/schematics?topic=schematics-agent-networkpolicy#agent-networkpolicy)

* [Restricting properties](/docs/schematics?topic=schematics-agent-networkpolicy#networkpolicy-restrict)

* [Default network policies](/docs/schematics?topic=schematics-agent-networkpolicy#networkpolicy-default)


## Logging and monitoring
{: #sitemap_logging_and_monitoring}


[Monitoring {{site.data.keyword.bpshort}} services by using {{site.data.keyword.mon_full_notm}}](/docs/schematics?topic=schematics-monitoring-instances#monitoring-instances)

* [Launching Monitoring UI from the {{site.data.keyword.cloud_notm}}](/docs/schematics?topic=schematics-monitoring-instances#launch-dashboard)

* [Launching monitor by using {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-monitoring-instances#monitor-using-schematics)

* [Creating service instance](/docs/schematics?topic=schematics-monitoring-instances#create-instance)

* [Creating custom dashboard](/docs/schematics?topic=schematics-monitoring-instances#create-dashboard)

* [{{site.data.keyword.bplong_notm}} metrics details](/docs/schematics?topic=schematics-monitoring-instances#metrics-details)

    * [`ibm_schematics_workspace_count`](/docs/schematics?topic=schematics-monitoring-instances#wkspace-count)

    * [`ibm_schematics_workspace_actions_count`](/docs/schematics?topic=schematics-monitoring-instances#wkspace-actions-count)

    * [`ibm_schematics_vulnerability_count`](/docs/schematics?topic=schematics-monitoring-instances#wkspace-vulnerability-count)

[Auditing events](/docs/schematics?topic=schematics-at_events#at_events)

* [{{site.data.keyword.bpshort}} events](/docs/schematics?topic=schematics-at_events#schematics-events)

    * [Workspace events](/docs/schematics?topic=schematics-at_events#schematics-wks-events)

    * [Action events](/docs/schematics?topic=schematics-at_events#schematics-action-events)

    * [Job events](/docs/schematics?topic=schematics-at_events#schematics-job-events)

    * [`Shareddata` events](/docs/schematics?topic=schematics-at_events#schematics-shareddata-events)

    * [Other events](/docs/schematics?topic=schematics-at_events#schematics-otherevents)

* [Viewing events](/docs/schematics?topic=schematics-at_events#at_ui)

* [Analyzing events](/docs/schematics?topic=schematics-at_events#at_analyze)

    * [Creating a workspace](/docs/schematics?topic=schematics-at_events#at_analyze_1)


## Location based access
{: #sitemap_location_based_access}


[Location based access](/docs/schematics?topic=schematics-access-ibm-cloud-catalog#access-ibm-cloud-catalog)

* [Manage location settings in catalog](/docs/schematics?topic=schematics-access-ibm-cloud-catalog#configure-location)


## Job queuing in {{site.data.keyword.bpshort}}
{: #sitemap_job_queuing_in_}


[Job queuing in {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-job-queue-process#job-queue-process)

* [About the {{site.data.keyword.bpshort}} job queue](/docs/schematics?topic=schematics-job-queue-process#about-job-queue)

* [Functioning of job queue](/docs/schematics?topic=schematics-job-queue-process#functions-job-queue)

* [When does the job enter into the pending queue?](/docs/schematics?topic=schematics-job-queue-process#pending-job-queue)

* [Timeout](/docs/schematics?topic=schematics-job-queue-process#job-queue-timeout)


## Deleting {{site.data.keyword.bpshort}} data
{: #sitemap_deleting__data}


[Deleting {{site.data.keyword.bpshort}} data](/docs/schematics?topic=schematics-delete-schematics-data-intro#delete-schematics-data-intro)

* [Scope](/docs/schematics?topic=schematics-delete-schematics-data-intro#delete-schematics-data-scope)

* [Deleting {{site.data.keyword.bpshort}} objects from UI](/docs/schematics?topic=schematics-delete-schematics-data-intro#delete-schematics-data-ui)

    * [Workspaces](/docs/schematics?topic=schematics-delete-schematics-data-intro#delete-schematics-data-wkscategory)

    * [Actions](/docs/schematics?topic=schematics-delete-schematics-data-intro#delete-schematics-data-actionscategory)

    * [Inventories](/docs/schematics?topic=schematics-delete-schematics-data-intro#delete-schematics-data-invcategory)

* [Deleting {{site.data.keyword.bpshort}} objects from CLI](/docs/schematics?topic=schematics-delete-schematics-data-intro#delete-schematics-data-cli)

    * [Workspaces](/docs/schematics?topic=schematics-delete-schematics-data-intro#delete-schematics-data-cliwks)

    * [Actions](/docs/schematics?topic=schematics-delete-schematics-data-intro#delete-schematics-data-cliactions)

    * [Inventories](/docs/schematics?topic=schematics-delete-schematics-data-intro#delete-schematics-data-cliinvcategory)

* [Deleting {{site.data.keyword.bpshort}} objects from API](/docs/schematics?topic=schematics-delete-schematics-data-intro#delete-schematics-data-api)

    * [Workspaces](/docs/schematics?topic=schematics-delete-schematics-data-intro#delete-schematics-data-apiwks)

    * [Actions](/docs/schematics?topic=schematics-delete-schematics-data-intro#delete-schematics-data-apiactions)

    * [Inventories](/docs/schematics?topic=schematics-delete-schematics-data-intro#delete-schematics-data-apicategory)


## Specifying version constraints
{: #sitemap_specifying_version_constraints}


[Specifying version constraints](/docs/schematics?topic=schematics-version-constraints#version-constraints)

* [Overview of {{site.data.keyword.bpshort}} images and packaged Terraform providers](/docs/schematics?topic=schematics-version-constraints#schematics-image-ov)

* [Specifying version constraints for the Terraform CLI and Terraform providers](/docs/schematics?topic=schematics-version-constraints#version-constraints-terraform)

    * [Version constraints for the Terraform CLI](/docs/schematics?topic=schematics-version-constraints#tf-version-constraint)

    * [Version constraints for Terraform providers](/docs/schematics?topic=schematics-version-constraints#provider-version-contraint)

* [Specifying version constraints in Ansible](/docs/schematics?topic=schematics-version-constraints#version-constraints-ansible)


## Using Terraform to configure {{site.data.keyword.bpshort}}
{: #sitemap_using_terraform_to_configure_}


[Using Terraform to configure {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-terraform-setup#terraform-setup)

* [Example: Creating the {{site.data.keyword.bpshort}} Workspaces by using Terraform](/docs/schematics?topic=schematics-terraform-setup#workspace-resource)

* [What's next?](/docs/schematics?topic=schematics-terraform-setup#terraform-setup-next)


## Enhancing security for Schematics
{: #sitemap_enhancing_security_for_schematics}


[Managing user access](/docs/schematics?topic=schematics-access#access)

* [Overview of {{site.data.keyword.bpshort}} service access roles and required permissions](/docs/schematics?topic=schematics-access#access-roles)

    * [Workspace permissions](/docs/schematics?topic=schematics-access#workspace-permissions)

    * [Action permissions](/docs/schematics?topic=schematics-access#action-permissions)

    * [Agent permissions](/docs/schematics?topic=schematics-access#agent-permissions)

    * [Blueprint permissions](/docs/schematics?topic=schematics-access#blueprint-permissions)

    * [KMS permissions](/docs/schematics?topic=schematics-access#kms-permissions)

* [Setting up access for your users](/docs/schematics?topic=schematics-access#access-setup)

* [Manage access tag in your account](/docs/schematics?topic=schematics-access#access-tag)

[User responsibilities by using {{site.data.keyword.bplong_notm}}](/docs/schematics?topic=schematics-responsibilities#responsibilities)

[Understanding high availability and disaster recovery for {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-high-availability#high-availability)

[Managing backups](/docs/schematics?topic=schematics-manage-backups#manage-backups)

* [Restoring a backup](/docs/schematics?topic=schematics-manage-backups#restoring-backups)

* [Steps to restore](/docs/schematics?topic=schematics-manage-backups#steps-to-restore)

[Using private endpoints](/docs/schematics?topic=schematics-private-endpoints#private-endpoints)

* [Private service endpoints in {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-private-endpoints#private-cse)

    * [Enable VRF and service endpoints for your account](/docs/schematics?topic=schematics-private-endpoints#private-network-prereqs)

    * [Connect to the {{site.data.keyword.bpshort}} private service endpoint](/docs/schematics?topic=schematics-private-endpoints#configure-private-network)

* [Virtual Private Endpoints Gateways for {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-private-endpoints#endpoint-setup)

    * [Before you begin](/docs/schematics?topic=schematics-private-endpoints#endpoint-prereq)

    * [Adding Virtual Private Endpoint Gateways for {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-private-endpoints#endpoint-add)

[Securing your data with encryption](/docs/schematics?topic=schematics-secure-data#secure-data)

* [How your data is stored and encrypted in {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-secure-data#data-storage)

    * [Key deletion or disable](/docs/schematics?topic=schematics-secure-data#key-delete)

    * [Key enable or restore](/docs/schematics?topic=schematics-secure-data#key-enable)

* [What technical information is stored in {{site.data.keyword.bpshort}}?](/docs/schematics?topic=schematics-secure-data#ti-data)

* [Where is my information stored?](/docs/schematics?topic=schematics-secure-data#pi-location)

* [How is my information encrypted?](/docs/schematics?topic=schematics-secure-data#pi-encrypt)

* [How can I delete my information?](/docs/schematics?topic=schematics-secure-data#delete-data)

[Opening needed IP addresses for {{site.data.keyword.bpfull_notm}} in your firewall](/docs/schematics?topic=schematics-allowed-ipaddresses#allowed-ipaddresses)


## Creating an {{site.data.keyword.containerlong_notm}} cluster on VPC infrastructure
{: #sitemap_creating_an__cluster_on_vpc_infrastructure}


[Creating an {{site.data.keyword.containerlong_notm}} cluster on VPC infrastructure](/docs/schematics?topic=schematics-provisioning-terraform-template#provisioning-terraform-template)

* [Description](/docs/schematics?topic=schematics-provisioning-terraform-template#provisioning-desc)

* [Objectives](/docs/schematics?topic=schematics-provisioning-terraform-template#provisioning-tut-obj)

* [Time required](/docs/schematics?topic=schematics-provisioning-terraform-template#provisioning-timereq)

* [Audience](/docs/schematics?topic=schematics-provisioning-terraform-template#provisioning-tut-audience)

* [Prerequisites](/docs/schematics?topic=schematics-provisioning-terraform-template#provisioning-tut-prereq)

* [Creating your {{site.data.keyword.bpshort}} Workspace](/docs/schematics?topic=schematics-provisioning-terraform-template#create-wkspace-for-cluster)

* [Creating your {{site.data.keyword.bplong_notm}} Workspace](/docs/schematics?topic=schematics-provisioning-terraform-template#create-tut-wks)

* [Planning and applying the Terraform template](/docs/schematics?topic=schematics-provisioning-terraform-template#tut-plan-wks)

* [What's next?](/docs/schematics?topic=schematics-provisioning-terraform-template#tut_whats_next)


## Setting up continuous deployment with {{site.data.keyword.bpshort}} and DevOps toolchain
{: #sitemap_setting_up_continuous_deployment_with__and_devops_toolchain}


[Setting up continuous deployment with {{site.data.keyword.bpshort}} and DevOps toolchain](/docs/schematics?topic=schematics-workspace-continuous-deployment#workspace-continuous-deployment)

* [Description](/docs/schematics?topic=schematics-workspace-continuous-deployment#workspace-desc)

* [Objectives](/docs/schematics?topic=schematics-workspace-continuous-deployment#workspace-obj)

* [Time needed](/docs/schematics?topic=schematics-workspace-continuous-deployment#workspace-timereq)

* [Audience](/docs/schematics?topic=schematics-workspace-continuous-deployment#workspace-tut-audience)

* [Prerequisites](/docs/schematics?topic=schematics-workspace-continuous-deployment#workspace-prereq)

* [Accessing the {{site.data.keyword.cloud_notm}} and GitHub](/docs/schematics?topic=schematics-workspace-continuous-deployment#access-automate-template)

* [Creating your {{site.data.keyword.bplong_notm}} Workspace](/docs/schematics?topic=schematics-workspace-continuous-deployment#create-wkspace)

* [Configuring variables](/docs/schematics?topic=schematics-workspace-continuous-deployment#configure-the-variables)

* [Automating the continuous deployment process](/docs/schematics?topic=schematics-workspace-continuous-deployment#continuous-deployment)

* [Analyzing the pipeline execution process](/docs/schematics?topic=schematics-workspace-continuous-deployment#analyze-deployment)

* [Analyzing the {{site.data.keyword.bpshort}} Workspace](/docs/schematics?topic=schematics-workspace-continuous-deployment#analyze-workspace-process)

* [What's next?](/docs/schematics?topic=schematics-workspace-continuous-deployment#automate-what-next)


## Importing {{site.data.keyword.bpshort}} templates into the {{site.data.keyword.cloud_notm}} catalog
{: #sitemap_importing__templates_into_the__catalog}


[Importing {{site.data.keyword.bpshort}} templates into the {{site.data.keyword.cloud_notm}} catalog](/docs/schematics?topic=schematics-private-catalog#private-catalog)

* [Objectives](/docs/schematics?topic=schematics-private-catalog#private-tut-obj)

* [Time required](/docs/schematics?topic=schematics-private-catalog#private-timereq)

* [Audience](/docs/schematics?topic=schematics-private-catalog#private-tut-audience)

* [Prerequisites](/docs/schematics?topic=schematics-private-catalog#private-prerequisites)

* [Prepare your Terraform template for the private catalog](/docs/schematics?topic=schematics-private-catalog#prepare-tf-templates)

* [Creating a release](/docs/schematics?topic=schematics-private-catalog#create-release)

* [Create a private catalog and add your Terraform template as a product](/docs/schematics?topic=schematics-private-catalog#create-private-catalog)

* [What's next?](/docs/schematics?topic=schematics-private-catalog#private_what's_next)


## Deploying a {{site.data.keyword.bpshort}} blueprint using the command line
{: #sitemap_deploying_a__blueprint_using_the_command_line}


[Deploying a {{site.data.keyword.bpshort}} blueprint using the command line](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#deploy-schematics-blueprint-cli)

* [Select a blueprint template](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#select-schematics-blueprint-cli)

* [Create the blueprint configuration](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#create-schematics-blueprint-cli)

    * [Syntax](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#step1-syntax)

    * [Output](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#step1-output)

* [Apply blueprint to deploy environment](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#install-schematics-blueprint-cli)

    * [Output](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#step3-output)

* [View blueprint job logs](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#view-schematics-blueprint-cli)

    * [Output](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#viewing-output)

* [Access and test the blueprint environment resources](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#review-schematics-blueprint)

    * [Using the cloud UI](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#review-schematics-blueprint-ui)

    * [Using the CLI](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#review-schematics-blueprint-cli)

* [Destroy blueprint cloud resources](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#destroy-schematics-blueprint-cli)

    * [Output](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#step5-output)

* [Delete the blueprint](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#delete-schematics-blueprint-cli)

    * [Output](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#step6-output)

* [Next steps](/docs/schematics?topic=schematics-deploy-schematics-blueprint-cli#nextsteps-schematics-blueprint-cli)


## Deploying a VPC environment with bastion host on IBM Cloud
{: #sitemap_deploying-a-vpc-environment-with-bastion-host-on-ibm-cloud}

[Deploying a VPC environment with bastion host on IBM Cloud](https://developer.ibm.com/articles/secure-vpc-access-with-a-bastion-host-and-terraform/){: external}


## Deploying a multitiered VPC with bastion host on IBM Cloud
{: #sitemap_deploying-a-multitiered-vpc-with-bastion-host-on-ibm-cloud}

[Deploying a multitiered VPC with bastion host on IBM Cloud](https://github.com/Cloud-Schematics/multitier-vpc-bastion-host/blob/master/README.md){: external}


## CLI reference
{: #sitemap_cli_reference}


[{{site.data.keyword.bplong_notm}} CLI](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-cli-reference)

* [Prerequisites](/docs/schematics?topic=schematics-schematics-cli-reference#cli-prerequisites)

* [Actions commands](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-action-commands)

    * [Inventory host groups](/docs/schematics?topic=schematics-schematics-cli-reference#inventory-host-grps)

    * [`ibmcloud schematics action create`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-create-action)

    * [`ibmcloud schematics action update`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-update-action)

    * [`ibmcloud schematics action get`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-get-action)

    * [`ibmcloud schematics action list`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-list-action)

    * [`ibmcloud schematics action delete`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-delete-action)

    * [`ibmcloud schematics action upload`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-upload-action)

* [Agent commands](/docs/schematics?topic=schematics-schematics-cli-reference#agent-cmd)

    * [`ibmcloud schematics agent apply`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-agent-apply)

    * [`ibmcloud schematics agent create`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-agent-create)

    * [`ibmcloud schematics agent get`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-agents-get)

    * [`ibmcloud schematics agent list`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-agent-list)

    * [`ibmcloud schematics agent plan`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-agent-plan)

* [Agents commands](/docs/schematics?topic=schematics-schematics-cli-reference#agents-cmd)

    * [`ibmcloud schematics agents bind-workspaces`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-agents-bind-wks)

    * [`ibmcloud schematics agents get`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-agents-get)

    * [`ibmcloud schematics agents list`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-agents-list)

    * [`ibmcloud schematics agent register`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-agent-register)

    * [`ibmcloud schematics agents unregister`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-agents-unregister)

    * [`ibmcloud schematics agents update`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-agent-update)

    * [`ibmcloud schematics workspace new with Agent`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-agent-new)

    * [`ibmcloud schematics workspace get with Agent`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-agent-get)

* [Blueprint commands](/docs/schematics?topic=schematics-schematics-cli-reference#blueprints-cmd)

    * [`ibmcloud schematics blueprint create`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-blueprint-create)

    * [`ibmcloud schematics blueprint apply`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-blueprint-apply)

    * [`ibmcloud schematics blueprint update`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-blueprint-update)

    * [`ibmcloud schematics blueprint get`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-blueprint-get)

    * [`ibmcloud schematics blueprint list`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-blueprint-list)

    * [`ibmcloud schematics blueprint destroy`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-blueprint-destroy)

    * [`ibmcloud schematics blueprint delete`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-blueprint-delete)

    * [`ibmcloud schematics blueprint job get`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-blueprint-job-get)

    * [`ibmcloud schematics blueprint job list`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-blueprint-job-list)

    * [`ibmcloud schematics blueprint job logs`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-blueprint-job-logs)

* [Policy commands](/docs/schematics?topic=schematics-schematics-cli-reference#policy-cmd)

    * [`ibmcloud schematics policy create`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-policy-create)

    * [`ibmcloud schematics policy get`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-policy-get)

    * [`ibmcloud schematics policy list`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-policy-list)

    * [`ibmcloud schematics policy update`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-policy-update)

    * [`ibmcloud schematics policy delete`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-policy-delete)

* [Enable BYOK or KYOK commands](/docs/schematics?topic=schematics-schematics-cli-reference#kms-commands)

    * [Prerequisites](/docs/schematics?topic=schematics-schematics-cli-reference#key-prerequisites)

    * [`ibmcloud schematics kms instance ls`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-kms-list)

    * [`ibmcloud schematics kms enable`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-kms-enable)

    * [`ibmcloud schematics kms info`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-kms-info)

* [General commands](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-general-commands)

    * [`ibmcloud schematics help`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-help-cmd)

    * [`ibmcloud schematics version`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-version)

* [Inventories commands](/docs/schematics?topic=schematics-schematics-cli-reference#inv-commands)

    * [`ibmcloud schematics inventory create`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-create-inv)

    * [`ibmcloud schematics inventory delete`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-delete-inventory)

    * [`ibmcloud schematics inventory get`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-get-inv)

    * [`ibmcloud schematics inventory list`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-list-inv)

    * [`ibmcloud schematics inventory update`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-update-inv)

* [Job commands](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-job-commands)

    * [`ibmcloud schematics job run`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-run-job)

    * [`ibmcloud schematics job update`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-update-job)

    * [`ibmcloud schematics job get`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-get-job)

    * [`ibmcloud schematics job list`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-list-job)

    * [`ibmcloud schematics job logs`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-logs-job)

    * [`ibmcloud schematics job delete`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-delete-job)

* [Resource management commands](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-resource-commands)

    * [`ibmcloud schematics apply`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-apply)

    * [`ibmcloud schematics destroy`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-destroy)

    * [`ibmcloud schematics logs`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-logs)

    * [`ibmcloud schematics output`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-output2)

    * [`ibmcloud schematics plan`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-plan)

* [Resource query commands](/docs/schematics?topic=schematics-schematics-cli-reference#rq-commands)

    * [`ibmcloud schematics resource query create`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-create-rq)

    * [`ibmcloud schematics resource query delete`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-delete-resource-query)

    * [`ibmcloud schematics resource query get`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-get-rq)

    * [`ibmcloud schematics resource query list`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-list-rq)

    * [`ibmcloud schematics resource query update`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-update-rq)

* [Stop commands](/docs/schematics?topic=schematics-schematics-cli-reference#stop-cmds)

    * [`ibmcloud schematics workspace job stop`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-stop-job)

* [Terraform commands](/docs/schematics?topic=schematics-schematics-cli-reference#tf-cmds)

    * [Commands](/docs/schematics?topic=schematics-schematics-cli-reference#cmds)

* [Terraform state file commands](/docs/schematics?topic=schematics-schematics-cli-reference#state-file-cmds)

    * [`ibmcloud schematics state pull`](/docs/schematics?topic=schematics-schematics-cli-reference#state-pull)

    * [`ibmcloud schematics workspace state show`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-show)

    * [`ibmcloud schematics workspace state mv`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-wks_statemv)

    * [`ibmcloud schematics workspace state rm`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-wks_staterm)

* [Workspaces commands](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-commands)

    * [`ibmcloud schematics workspace action`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-action)

    * [`ibmcloud schematics workspace delete`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-delete)

    * [`ibmcloud schematics workspace get`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-get)

    * [`ibmcloud schematics workspace import`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-import)

    * [`ibmcloud schematics workspace list`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-list)

    * [`ibmcloud schematics workspace new`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-new)

    * [`ibmcloud schematics refresh`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-refresh)

    * [`ibmcloud schematics state list`](/docs/schematics?topic=schematics-schematics-cli-reference#state-list)

    * [`ibmcloud schematics workspace taint`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-taint)

    * [`ibmcloud schematics workspace untaint`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-untaint)

    * [`ibmcloud schematics workspace update`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-update)

    * [`ibmcloud schematics workspace upload`](/docs/schematics?topic=schematics-schematics-cli-reference#schematics-workspace-upload)

[CLI version history](/docs/schematics?topic=schematics-cli_version-releases#cli_version-releases)


## API reference
{: #sitemap_api_reference}


[IBM Cloud Schematics API](https://cloud.ibm.com/apidocs/schematics){: external}


## Blueprint template reference
{: #sitemap_blueprint_template_reference}


[Blueprint template YAML schema](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-template-schema-yaml)

* [Global preface](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-parameters)

    * [name](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-name)

    * [type](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-type)

    * [schema_version](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-schema-version)

    * [description](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-description)

    * [tags](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-tags)

    * [inputs](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-inputs)

    * [outputs](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-outputs)

    * [settings](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-settings)

* [Module parameters](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-schema)

    * [modules.name](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-name)

    * [modules.module_type](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-moduletype)

    * [modules.source options](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-sourceoptions)

    * [modules.source.source_type](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-source-type)

    * [modules.source.git.git_repo_url](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-git-repo-url)

    * [modules.source.git.git_branch](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-git-branch)

    * [modules.source.git.git_release](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-git-release)

    * [modules.source.git.git_token](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-git-token)

    * [modules.settings](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-settings)

    * [modules.inputs options](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-inputs-options)

    * [modules.inputs.name](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-inputs-name)

    * [modules.inputs.type](/docs/schematics?topic=schematics-bp-template-schema-yaml#module-inputs-type)

    * [modules.inputs.value](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-inputs-value)

    * [module.outputs](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-module-outputs)

    * [module.injectors options](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-injector)

    * [module.injectors.tft_git_url](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-module-tft-git-url)

    * [module.injectors.tft_name](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-module-tft-name)

    * [module.injectors.injection_type](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-module-injection-type)

    * [module.injectors.tft_parameters](/docs/schematics?topic=schematics-bp-template-schema-yaml#bp-modules-tft-parameters)

[Blueprints input file YAML Schema](/docs/schematics?topic=schematics-bp-input-schema-yaml#bp-input-schema-yaml)

* [Defining input values](/docs/schematics?topic=schematics-bp-input-schema-yaml#define-input-value)

* [Complex input values](/docs/schematics?topic=schematics-bp-input-schema-yaml#complex-input-value)


## Beta code for {{site.data.keyword.bpshort}} Agents
{: #sitemap_beta_code_for__agents}


[Beta code for {{site.data.keyword.bpshort}} Agents](/docs/schematics?topic=schematics-agent-beta-limitations#agent-beta-limitations)

* [Beta release limitations for Agent](/docs/schematics?topic=schematics-agent-beta-limitations#sc-agent-beta-limitation)

* [Joining public slack channel](/docs/schematics?topic=schematics-agent-beta-limitations#sc-agent-join-public-slack)

    * [Steps to join public slack](/docs/schematics?topic=schematics-agent-beta-limitations#sc-agent-join-slack)


## Beta code for {{site.data.keyword.bpshort}} Blueprints
{: #sitemap_beta_code_for__blueprints}


[Beta code for {{site.data.keyword.bpshort}} Blueprints](/docs/schematics?topic=schematics-bp-beta-limitations#bp-beta-limitations)

* [Beta changes October 2022](/docs/schematics?topic=schematics-bp-beta-limitations#bp-beta-changes-oct)

* [Beta release limitations](/docs/schematics?topic=schematics-bp-beta-limitations#sc-bp-beta-limitation)

* [Beta release known issues](/docs/schematics?topic=schematics-bp-beta-limitations#sc-bp-beta-knownissues)

* [Joining public slack channel](/docs/schematics?topic=schematics-bp-beta-limitations#sc-bp-join-public-slack)

    * [Steps to join public slack](/docs/schematics?topic=schematics-bp-beta-limitations#sc-bp-join-slack)


## Runtime environment tools
{: #sitemap_runtime_environment_tools}


[Runtime environment tools](/docs/schematics?topic=schematics-sch-utilities#sch-utilities)

* [Terraform-runtime-job image used by {{site.data.keyword.bpshort}} Workspaces](/docs/schematics?topic=schematics-sch-utilities#terraform-runtime-job)

* [Terraform-runtime-agent-job image used by {{site.data.keyword.bpshort}} Agents](/docs/schematics?topic=schematics-sch-utilities#terraform-runtime-agent-job)

* [Ansible-runtime-job image used by {{site.data.keyword.bpshort}} Actions](/docs/schematics?topic=schematics-sch-utilities#Ansible-runtime-job)


## {{site.data.keyword.bpshort}} SDKs
{: #sitemap__sdks}


[{{site.data.keyword.bpshort}} SDKs](/docs/schematics?topic=schematics-schematics-sdks#schematics-sdks)


## Service locations and endpoints
{: #sitemap_service_locations_and_endpoints}


[Service locations and endpoints](/docs/schematics?topic=schematics-locations#locations)

* [Where can I create and run {{site.data.keyword.bpshort}} Workspaces?](/docs/schematics?topic=schematics-locations#where-wks-created)

* [Where do my {{site.data.keyword.bpshort}} Actions run?](/docs/schematics?topic=schematics-locations#where-do-locations-run)

* [Where is my {{site.data.keyword.bpshort}} and template data stored?](/docs/schematics?topic=schematics-locations#where-is-data-stored)

* [Where are my {{site.data.keyword.cloud_notm}} resources provisioned?](/docs/schematics?topic=schematics-locations#where-are-resources-provisioned)


## Service limitations
{: #sitemap_service_limitations}


[Service limitations](/docs/schematics?topic=schematics-schematics-limitations#schematics-limitations)

* [Differences to native Terraform](/docs/schematics?topic=schematics-schematics-limitations#terraform-vs-schematics)

    * [Do I need to provide an {{site.data.keyword.cloud_notm}} API key in the `provider` block?](/docs/schematics?topic=schematics-schematics-limitations#provider-block)

    * [Can I use my local `terraform.tfvars` file?](/docs/schematics?topic=schematics-schematics-limitations#terraformtfvars)

    * [Is Terraform remote state supported in {{site.data.keyword.bpshort}}?](/docs/schematics?topic=schematics-schematics-limitations#tf-remote-state)

    * [Why is my local-exec and remote-exec provisioner in {{site.data.keyword.bplong_notm}} fails?](/docs/schematics?topic=schematics-schematics-limitations#local-remote-exec)

* [What is the use of refresh token header?](/docs/schematics?topic=schematics-schematics-limitations#refresh-token)


## Glossary
{: #sitemap_glossary}


[Glossary](/docs/schematics?topic=schematics-glossary#glossary)

* [Actions](/docs/schematics?topic=schematics-glossary#glossary-actions)

* [Agents](/docs/schematics?topic=schematics-glossary#glossary-agents)

    * [Agent](/docs/schematics?topic=schematics-glossary#agentsa1)

    * [Agent service](/docs/schematics?topic=schematics-glossary#agentsa2)

    * [Agent Infrastructure](/docs/schematics?topic=schematics-glossary#agentsa3)

* [Blueprints](/docs/schematics?topic=schematics-glossary#glossary-blueprint)

    * [Blueprint](/docs/schematics?topic=schematics-glossary#bpb1)

    * [Blueprint template](/docs/schematics?topic=schematics-glossary#bpb2)

    * [Blueprint configuration](/docs/schematics?topic=schematics-glossary#bpb3)

    * [Blueprint environment](/docs/schematics?topic=schematics-glossary#bpb4)

    * [Blueprint modules](/docs/schematics?topic=schematics-glossary#bpb5)

    * [Blueprint inputs](/docs/schematics?topic=schematics-glossary#bpi1)

    * [Blueprint input files](/docs/schematics?topic=schematics-glossary#bpi2)

    * [Blueprint jobs](/docs/schematics?topic=schematics-glossary#bpj1)

    * [Blueprint lifecycle](/docs/schematics?topic=schematics-glossary#bpl1)

* [Catalog](/docs/schematics?topic=schematics-glossary#glossa-catalog)

* [Inventories](/docs/schematics?topic=schematics-glossary#glossa-inventory)

    * [Resource inventory](/docs/schematics?topic=schematics-glossary#rir1)

* [Jobs](/docs/schematics?topic=schematics-glossary#glossary-job)

* [Templates or Modules](/docs/schematics?topic=schematics-glossary#glossary-template)

* [Workspaces](/docs/schematics?topic=schematics-glossary#glossary-workspace)

    * [{{site.data.keyword.bpshort}} Workspaces](/docs/schematics?topic=schematics-glossary#wkss1)

    * [Jobs](/docs/schematics?topic=schematics-glossary#wksj1)

    * [Resources](/docs/schematics?topic=schematics-glossary#wksr1)

    * [Readme file](/docs/schematics?topic=schematics-glossary#wksr2)

    * [Settings](/docs/schematics?topic=schematics-glossary#wkss2)

    * [Workspace](/docs/schematics?topic=schematics-glossary#wksw1)


## Notices and information
{: #sitemap_notices_and_information}


[Notices and information](/docs/schematics?topic=schematics-schematics-notices#schematics-notices)

* [Creative Commons Attribution 3.0](/docs/schematics?topic=schematics-schematics-notices#CC-BY-3.0)

* [Creative Commons Attribution 4.0](/docs/schematics?topic=schematics-schematics-notices#CC-BY-4.0)

* [Creative Commons Attribution Share Alike 1.0 Generic](/docs/schematics?topic=schematics-schematics-notices#CC-BY-SA-1.0)

* [Creative Commons Attributions Share Alike 2.0 Generic](/docs/schematics?topic=schematics-schematics-notices#CC-BY-SA-2.0)

* [Creative Commons Attribution 2.5 Generic](/docs/schematics?topic=schematics-schematics-notices#CC-BY-SA-2.5)

* [Creative Commons Attribution Share Alike 3.0 Generic](/docs/schematics?topic=schematics-schematics-notices#CC-BY-SA-3.0)

* [Creative Commons Attribution Share Alike 4.0 Generic](/docs/schematics?topic=schematics-schematics-notices#CC-BY-SA-4.0)


## Create `profile_id` for Agents
{: #sitemap_create_profile_id_for_agents}


[Create `profile_id` for Agents](/docs/schematics?topic=schematics-agent-trusted-profile#agent-trusted-profile)

* [Next Step](/docs/schematics?topic=schematics-agent-trusted-profile#agent-profile-id-nextstep)


## Related links
{: #sitemap_related_links}



### Terraform
{: #sitemap_terraform}



### Ansible
{: #sitemap_ansible}



## FAQs
{: #sitemap_faqs}


[Actions](/docs/schematics?topic=schematics-actions-faq#actions-faq)

* [Why is my success action job execution displays DEPRECATION WARNING message?](/docs/schematics?topic=schematics-actions-faq#deprecation-warn-faq)

* [How can I resolve that might not run action error while provisioning `WinRM` by using {{site.data.keyword.bpshort}} action?](/docs/schematics?topic=schematics-actions-faq#winrm-faq)

* [When are the new Terraform and Ansible versions added to {{site.data.keyword.bpshort}}?](/docs/schematics?topic=schematics-actions-faq#new-versions)

* [Can I run Ansible playbooks with {{site.data.keyword.bpshort}}?](/docs/schematics?topic=schematics-actions-faq#ansible-playbooks)

[Agent](/docs/schematics?topic=schematics-faqs-agent#faqs-agent)

* [What are the new updates in the agent beta-1 release?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-update)

* [What is the cost of installing the {{site.data.keyword.bpshort}} Agent?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-cost)

* [Can I install more than one {{site.data.keyword.bpshort}} Agent on a cluster?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-install)

* [What type of Schematics jobs can I run in my Agent?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-jobs)

* [How can I see the {{site.data.keyword.bpshort}} job results and logs, for the workloads running on an agent?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-workload)

* [How many {{site.data.keyword.bpshort}} jobs can run in parallel in the Agent?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-parallel)

* [What is the minimum cluster configuration required in Agent release?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-min-cluster)

* [How many workspaces can be assigned to an agent?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-min-wks)

* [How many jobs can run in parallel on an agent?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-min-job)

* [What is the default polling interval for an agent?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-poll-interval)

* [What is the difference between agent-location and location input variable flag in Agent service?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-diff-location)

* [Can an agent run {{site.data.keyword.bpshort}} Job from different resource group?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-diff-rg)

* [Can an agent run {{site.data.keyword.bpshort}} Job from different region?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-diff-region)

* [Can I register one agent with multiple accounts?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-register)

* [Can jobs of an existing workspace configured to run on an agent?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-conf)

* [What are the identity and permissions are needed to deploy an agent?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-permission)

* [When my agent is deployed in a private network. How can I configure mirror site for the Terraform plug-ins?](/docs/schematics?topic=schematics-faqs-agent#faqs-agent-pvt-network)

[Blueprints](/docs/schematics?topic=schematics-blueprints-faq#blueprints-faq)

* [What are the Git repositories that are supported by Blueprints?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-repos)

* [Are variable operators and functions supported in blueprint templates?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-values)

* [How are blueprint module dependencies and execution order determined?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-dependencies)

* [How do I edit and validate blueprint templates?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-editing)

* [Why do blueprints get the error 'Length for variable `variable name` greater than the given length'?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-length)

* [Why do blueprint operations require a `blueprint ID`?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-install)

* [What URL format is used for referencing blueprint templates and input files?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-url)

* [How is resource provisioning performed?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-resource)

* [How do you view the blueprint provisioned resources in your cloud account?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-results)

* [How do you securely pass input variables?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-secure-inputs)

* [Why does the blueprint template, basic example, fail in the apply step?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-basic-example)

* [What is the time taken to create an IBM Kubernetes Service cluster and other resources?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-time)

* [How do you configure the version of Terraform to used?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-tf-version)

* [Is it possible to specify the CLI parameters as a file?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-cli-file)

* [When you create a blueprint config in the `us-south` target region, why is the blueprint job ID indicating `us-east`?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-target-region)

* [Is it possible to delete the {{site.data.keyword.bpshort}} service instance by using the Resource Controller API or CLI?](/docs/schematics?topic=schematics-blueprints-faq#faqs-bp-schematics-instance)

[General](/docs/schematics?topic=schematics-general-faq#general-faq)

* [What is {{site.data.keyword.bplong_notm}} and how does it work?](/docs/schematics?topic=schematics-general-faq#what-is-schematics)

* [What is Infrastructure as Code?](/docs/schematics?topic=schematics-general-faq#what-is-iac)

* [What am I charged for when I use {{site.data.keyword.bpshort}}?](/docs/schematics?topic=schematics-general-faq#charges)

* [Does {{site.data.keyword.bpfull_notm}} support multiple Terraform provider versions?](/docs/schematics?topic=schematics-general-faq#provider-versions)

* [How do I generate IAM access token, if client ID `bx` is used?](/docs/schematics?topic=schematics-general-faq#createworkspace-generate-tokens)

* [How do I rectify 'Failed to clone Git repository, might not find remote ref `refs/heads/master` (most likely invalid branch name is passed)'?](/docs/schematics?topic=schematics-general-faq#template-errors)

* [Can I increase the timeout for null-exec and remote-exec resource?](/docs/schematics?topic=schematics-general-faq#timeout-null-resource)

* [How can I save user-defined files that are generated by the Terraform modules and use them across multiple Terraform plan, apply, destroy, refresh, or import commands?](/docs/schematics?topic=schematics-general-faq#persist-file)

* [How do I identify the best way to synchronize a deleted resource with the Terraform state?](/docs/schematics?topic=schematics-general-faq#sync-delresource-terraform)

* [How do I overcome the request exceeds the Cluster resource quota of '100' for the account in any region?](/docs/schematics?topic=schematics-general-faq#clusterquota-warn-faq)

* [While creating Red Hat OpenShift or Kubernetes resources, can I tune 90 minutes time out to higher?](/docs/schematics?topic=schematics-general-faq#resourcetimeout-warn-faq)

* [How can I rectify the 403 Error while validating the location in the account. Verify you have permission to the location in the global catalog settings?](/docs/schematics?topic=schematics-general-faq#global-setting-location)

* [Can I start or stop the {{site.data.keyword.vsi_is_short}} based on tags and through scheduler or cron job?](/docs/schematics?topic=schematics-general-faq#vm-tags-faq)

* [Might I create a worker node in an existing worker node pool?](/docs/schematics?topic=schematics-general-faq#workernode-kubernetes-faq)

* [Where can I view the list of public and private allowed IP addresses of `us-south`, `us-east`, `eu-gb`, and `eu-de` regions?](/docs/schematics?topic=schematics-general-faq#privateip-workspace-faq)

* [Can I manually add, or remove a resource from the service dashboard directly?](/docs/schematics?topic=schematics-general-faq#add-remove-resource-faq)

* [What changes can I make to my resources?](/docs/schematics?topic=schematics-general-faq#resource-faq)

* [How can I compare the required state of my cloud resources against the actual state of my resources?](/docs/schematics?topic=schematics-general-faq#required-resource-state-faq)

* [What are the deviations that cannot be detected?](/docs/schematics?topic=schematics-general-faq#edit-resource-faq)

* [How must I remove resources with {{site.data.keyword.bplong_notm}}?](/docs/schematics?topic=schematics-general-faq#remove-resource-faq)

* [What happens if I choose to delete my resource directly from the resource dashboard?](/docs/schematics?topic=schematics-general-faq#delete-resource-directly-faq)

* [Does {{site.data.keyword.bpshort}} supports `ibmcloud terraform` command?](/docs/schematics?topic=schematics-general-faq#ibmcloud-terraform-cmd-faq)

* [Can I access private network through {{site.data.keyword.bpshort}}?](/docs/schematics?topic=schematics-general-faq#private-endpoint-faq)

* [How can I resolve the error message when connecting to Bastion host IP addresses through {{site.data.keyword.bplong_notm}}?](/docs/schematics?topic=schematics-general-faq#bastion-ipaddress-faq)

* [How do I create a cluster by using Terraform on {{site.data.keyword.cloud_notm}} environment?](/docs/schematics?topic=schematics-general-faq#newcluster-workspace-faq)

* [Can I always set Terraform to use the current or default version?](/docs/schematics?topic=schematics-general-faq#terraform-defaultversion-faq)

* [If I set `"type”: = “terraform_v1.0"` in the JSON file as shown in the code block, will `Terraform version 1.0 continue to use even if Terraform version 2.0 or higher` are released?](/docs/schematics?topic=schematics-general-faq#terraform-type-faq)

* [Can I specify only the provider version in the `version` parameter? Or is it mandatory to provide the `required_version` parameter in the `versions.tf` file?](/docs/schematics?topic=schematics-general-faq#terraform-reqparam-faq)

* [What is the difference between delete, and destroy in {{site.data.keyword.bpshort}}?](/docs/schematics?topic=schematics-general-faq#faq-delete-destroy)

* [Can I delete and destroy operation as one step?](/docs/schematics?topic=schematics-general-faq#faq-delete-destroy-operation)

[Workspaces](/docs/schematics?topic=schematics-workspaces-faq#workspaces-faq)

* [How do you overcome the authentication error when {{site.data.keyword.bpshort}} Workspaces is created by using API?](/docs/schematics?topic=schematics-workspaces-faq#createworkspace-authentication-error)

* [How do {{site.data.keyword.bpshort}} decide to remove the files from the Terraform, or Ansible templates?](/docs/schematics?topic=schematics-workspaces-faq#clone-file-extension)

* [How do you upgrade the Terraform versions in {{site.data.keyword.bpshort}}? or Can I update the version during workspace recreation?](/docs/schematics?topic=schematics-workspaces-faq#migrate-terraform-v11)

* [How do I overcome the downtime updating the workspace activities?](/docs/schematics?topic=schematics-workspaces-faq#impact-downtime-workspace)

* [Why do the jobs delay in a queue when plan is generated?](/docs/schematics?topic=schematics-workspaces-faq#job-queue-faq)

* [How do I `pull latest` code from the workspace through command line?](/docs/schematics?topic=schematics-workspaces-faq#latestcode-workspace-commandline)

* [What are the development tools and utilities used in the {{site.data.keyword.bpshort}}?](/docs/schematics?topic=schematics-workspaces-faq#schematics-tools)

* [How can I create workspace from command-line by using Git repositories and personal access token with full permission?](/docs/schematics?topic=schematics-workspaces-faq#create-workspace-cli-tokens)

* [How do you overcome the authorization issue when create or update a workspace or a template?](/docs/schematics?topic=schematics-workspaces-faq#workspace-auth)

* [How can I access the {{site.data.keyword.bpshort}} services for test ID?](/docs/schematics?topic=schematics-workspaces-faq#global-catalog-faq)

* [How can you download `subfolder`s from the Git repositories through {{site.data.keyword.bpshort}}](/docs/schematics?topic=schematics-workspaces-faq#compact-faq)

* [How do I resolve issue while trying to delete a workspace that was created for a cluster that no longer exists, deletion fails because of the cluster not found?](/docs/schematics?topic=schematics-workspaces-faq#clusterdeletion-warn-faq)

* [What is the best way to deploy a Helm chart to an existing cluster by using {{site.data.keyword.bpshort}} keeping credentials or secrets?](/docs/schematics?topic=schematics-workspaces-faq#gherepo-warn-faq)

* [How do you set the release tag through {{site.data.keyword.bpshort}}?](/docs/schematics?topic=schematics-workspaces-faq#releasetag-warn-faq)

* [Why you are getting 403 error instead of 404 error when providing an invalid workspace ID?](/docs/schematics?topic=schematics-workspaces-faq#invalidwspid-warn-faq)

* [How can you enable Terraform debug through the `ibmcloud schematics` command line?](/docs/schematics?topic=schematics-workspaces-faq#terraform-debug-ibmcli)

* [How can I generate {{site.data.keyword.bpshort}} Workspaces import from CLI?](/docs/schematics?topic=schematics-workspaces-faq#workspace-import-ibmcli)

* [Can I download the {{site.data.keyword.bpshort}} Job files?](/docs/schematics?topic=schematics-workspaces-faq#download-jobfile)

* [Can I set TF_CLI_ARGS environment variable in the {{site.data.keyword.bpshort}} Workspaces console without using catalog service or {{site.data.keyword.bpshort}} command line?](/docs/schematics?topic=schematics-workspaces-faq#terraformcli-arguments-faq)

* [Does {{site.data.keyword.bpshort}} support to download the Terraform modules template from the private repository?](/docs/schematics?topic=schematics-workspaces-faq#download-module-netrc-faq)

* [Can I edit all the variables in the {{site.data.keyword.bpshort}} console instead of editing individually?](/docs/schematics?topic=schematics-workspaces-faq#edit-variables-faq)

* [Can I set or manage keys for `ibm_kms_key` resource when {{site.data.keyword.bpshort}} Workspaces imports Terraform?](/docs/schematics?topic=schematics-workspaces-faq#kmskey-value-faq)

* [Can you enable the TRACE to help DEBUG {{site.data.keyword.bpshort}} API while running workspace list command?](/docs/schematics?topic=schematics-workspaces-faq#traces-api-faq)

* [How do I overcome the `Error while retrieving {{site.data.keyword.bpshort}} Instance for the given account` to fetch {{site.data.keyword.bpshort}} Workspaces?](/docs/schematics?topic=schematics-workspaces-faq#badstatus-workspace-faq)

* [How can I configure private (IBM) GitLab repository in {{site.data.keyword.bpshort}} Workspace?](/docs/schematics?topic=schematics-workspaces-faq#gitlab-workspace-faq)

* [Does {{site.data.keyword.cloud_notm}} provider support manages IAM access groups in {{site.data.keyword.bpshort}}?](/docs/schematics?topic=schematics-workspaces-faq#manageaccessgrp-iam-faq)

* [Might I create {{site.data.keyword.bpshort}} Workspaces in {{site.data.keyword.cloud_notm}} source account and run Terraform providing resources in {{site.data.keyword.cloud_notm}} target account to provision?](/docs/schematics?topic=schematics-workspaces-faq#account-resource-faq)

* [Does `North America` location indicate `us-south`, `us-east`, or `both` during the {{site.data.keyword.bpshort}} Workspaces creation?](/docs/schematics?topic=schematics-workspaces-faq#location-faq)

* [What are the port used to communicate with {{site.data.keyword.bpshort}} and resources, such as VPC services?](/docs/schematics?topic=schematics-workspaces-faq#port-faq)

* [When do I use {{site.data.keyword.bplong_notm}} versus the individual resource dashboards?](/docs/schematics?topic=schematics-workspaces-faq#schematics-vs-cloud-resource-faq)

* [When I change my configuration file in GitHub, is my change automatically available in the next execution plan?](/docs/schematics?topic=schematics-workspaces-faq#edit-resource-confg-faq)

* [Where does {{site.data.keyword.bpshort}} store the state of the cloud resources?](/docs/schematics?topic=schematics-workspaces-faq#resource-state-faq)

* [Are the resources removed when remove the workspace is run?](/docs/schematics?topic=schematics-workspaces-faq#delete-resource-wks-faq)

* [How can I update a workspace that is created through payload in command line to resolve invalid payload issue?](/docs/schematics?topic=schematics-workspaces-faq#invalid-paylaod-cli)

* [Is the drift detection an automatic in the {{site.data.keyword.bplong_notm}}?](/docs/schematics?topic=schematics-workspaces-faq#drift-automatic-faq)

* [Can I initiate the drift detection?](/docs/schematics?topic=schematics-workspaces-faq#drift-initiate-faq)

* [Where can I see the status of the drift detection? Or How can I know whether the workspace is in drift?](/docs/schematics?topic=schematics-workspaces-faq#drift-status-faq)

* [Can I `interrupt`, `force-stop`, or `terminate` the provisioning resources or a running job in {{site.data.keyword.bpshort}}?](/docs/schematics?topic=schematics-workspaces-faq#stopping-job-faq)

* [How can I `POST` Cart API with a location as `eu-de` region and resolve `Incorrect Location Input` error?](/docs/schematics?topic=schematics-workspaces-faq#postcartapi-job-faq)

* [What CLI command is used to view the resources as in the {{site.data.keyword.bpshort}} Workspace resources?](/docs/schematics?topic=schematics-workspaces-faq#clicmdresource-job-faq)

* [How do I fix the `CreateworkspaceWithContext failed Bad request` error in creating {{site.data.keyword.bpshort}} resource to `eu-de` region by using Terraform?](/docs/schematics?topic=schematics-workspaces-faq#locationres-job-faq)

* [How can I encrypt sensitive value in Terraform state file when using {{site.data.keyword.bpshort}}?](/docs/schematics?topic=schematics-workspaces-faq#encrypt-state-file)

* [Why is {{site.data.keyword.bpshort}} workspace list variable defined by using CLI throws 400 error?](/docs/schematics?topic=schematics-workspaces-faq#wks-list-var)

* [Why is the Terraform version (`TF_VERSION`) updated through `JSON` file is not working?](/docs/schematics?topic=schematics-workspaces-faq#tf-version-update)

* [In each workspace job trigger the previously created resources gets force replaced with the new values. Can I reset or start with the new Terraform state file with each trigger?](/docs/schematics?topic=schematics-workspaces-faq#wks-job-trigger)

* [Can I bootstrap a {{site.data.keyword.bpshort}} Workspace with an existing Terraform state that are created elsewhere?](/docs/schematics?topic=schematics-workspaces-faq#tf-state-argument)

* [What is the maximum length of characters that the {{site.data.keyword.bpshort}} Workspace name variable supports?](/docs/schematics?topic=schematics-workspaces-faq#wks-name-maxlength)


## Troubleshooting
{: #sitemap_troubleshooting}



### Troubleshooting Schematics apply errors
{: #sitemap_troubleshooting_schematics_apply_errors}


[How can you find the root cause of why {{site.data.keyword.bpshort}} apply is failing?](/docs/schematics?topic=schematics-nullresource-errors#nullresource-errors)

[Why can't {{site.data.keyword.bpshort}} find your resource group?](/docs/schematics?topic=schematics-rg-not-found#rg-not-found)

[Why are you getting 5xx HTTP errors?](/docs/schematics?topic=schematics-server-errors#server-errors)


### Troubleshooting Schematics create errors
{: #sitemap_troubleshooting_schematics_create_errors}


[Why do {{site.data.keyword.bpshort}} Workspaces create using the API/UI/CLI fails?](/docs/schematics?topic=schematics-wks-create-api#wks-create-api)


### Troubleshooting blueprints
{: #sitemap_troubleshooting_blueprints}


[Blueprint create fails](/docs/schematics?topic=schematics-bp-create-fails#bp-create-fails)

* [Blueprint create fails with an invalid blueprint template: failed to clone Git repository error](/docs/schematics?topic=schematics-bp-create-fails#bp-create-fails1)

* [Blueprint create fails with an invalid blueprint template: unable to find file error](/docs/schematics?topic=schematics-bp-create-fails#bp-create-fails2)

* [Blueprint create fails with the requested resource group as invalid](/docs/schematics?topic=schematics-bp-create-fails#bp-create-fails3)

* [Blueprint create fails with the error blueprint JSON validation failed: field missing or invalid in config](/docs/schematics?topic=schematics-bp-create-fails#bp-create-fails4)

* [Blueprint create fails with the error blueprint JSON validation failed - field missing or invalid](/docs/schematics?topic=schematics-bp-create-fails#bp-create-fails5)

[blueprint create fails in the create_init step](/docs/schematics?topic=schematics-bp-create-init-fails#bp-create-init-fails)

[blueprint apply fails](/docs/schematics?topic=schematics-bp-apply-fails#bp-apply-fails)

* [blueprint apply fails with message "Install of module Failed"](/docs/schematics?topic=schematics-bp-apply-fails#bp-apply-fails1)

* [blueprint apply failure due to Terraform config coding error](/docs/schematics?topic=schematics-bp-apply-fails#bp-apply-fails2)

* [blueprint apply failure due to Terraform timeouts or transient failures](/docs/schematics?topic=schematics-bp-apply-fails#bp-apply-fails3)

* [blueprint apply failures that require changes to values in input files](/docs/schematics?topic=schematics-bp-apply-fails#bp-apply-fails4)

* [blueprint apply failures that require changes to dynamic inputs](/docs/schematics?topic=schematics-bp-apply-fails#bp-apply-fails5)


### Troubleshooting Agents
{: #sitemap_troubleshooting_agents}


[How can you provide value to `schematics_resource_crn` variable?](/docs/schematics?topic=schematics-agent-crn-not-found#agent-crn-not-found)

[Why are your getting create endpoint gateway that is failed with wrong number of segments in CRN?](/docs/schematics?topic=schematics-agent-endpoint-error#agent-endpoint-error)

[Troubleshooting errors](/docs/schematics?topic=schematics-handling-error#handling-error)

* [Action error messages](/docs/schematics?topic=schematics-handling-error#action-errmsg)

    * [Parameter error](/docs/schematics?topic=schematics-handling-error#param-error)

    * [Service error](/docs/schematics?topic=schematics-handling-error#svc-error)

    * [State error](/docs/schematics?topic=schematics-handling-error#state-error)

    * [Job error](/docs/schematics?topic=schematics-handling-error#job-error)


## Getting help and support
{: #sitemap_getting_help_and_support}


[Getting help and support](/docs/schematics?topic=schematics-schematics-help#schematics-help)

