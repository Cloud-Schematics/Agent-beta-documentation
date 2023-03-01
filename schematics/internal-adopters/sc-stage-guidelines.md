---

copyright:
  years: 2017, 2022
lastupdated: "2022-09-12"

keywords: stage schematics, schematics stage environment, infrastructure as code, terraform template, schematics workspace

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}

# Guidelines for using {{site.data.keyword.bpshort}} stage environment
{: #stage-guidelines-schematics} 

When planning to make {{site.data.keyword.bpshort}} service public. {{site.data.keyword.bpshort}} sets various features, fixes, and enhancement testing. {{site.data.keyword.bpshort}} sets guidelines and expectation for the stage users access staging environment.
{: shortdesc}

The following list states the guidelines for using the {{site.data.keyword.bpshort}} staging environment.

- Can be unstable due to continuous development, testing, and fixes.
- No Service Level Agreements (SLAs) for using {{site.data.keyword.bpshort}} staging environment.
- The {{site.data.keyword.bpshort}} staging environment testing must not be used in production environment.
- The {{site.data.keyword.bpshort}} staging environment must not be used in production workload, or automation.
- The data in {{site.data.keyword.bpshort}} staging environment is cleaned up with little or no notice.
- The content in the stage documentation is cleaned up with little or no notice


