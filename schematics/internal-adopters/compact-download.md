---

copyright:
  years: 2017, 2021
lastupdated: "2021-11-23"

keywords: compact, subdirectory, schematics, download, directory

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}

# Compact download for {{site.data.keyword.bpshort}} workspace
{: #compact-download}

{{site.data.keyword.bpshort}} workspaces act as a container of a Terraform template with the input data, output state, jobs, and job log files. The workspace uses the Git URL of the Terraform template. For example, the [Terraform template](https://github.com/terraform-ibm-modules/terraform-ibm-database/tree/main/examples/simple-etcd){: external} provided by an user is to download and securely store the template files. The default behaviour of the workspace is to download the whole Git repository and to save securely. Workspace assumes that the Terraform templates have relative references to template, modules, script, or data files that resides in the directory or subdirectory of the repository. 

Let's consider a scenario that the user is aware that the Terraform templates are isolated to a specific folder and its subdirectory, for example, `examples/simple-etcd` in the Git repository. Now the user wants the workspace to download, only the relevant files from the Git repository. This can be achieved using the **compact download** feature. The compact download feature fastens to download and process the files from the Git repository while creating, or updating the workspace.

## Location to active or deactive compact download
{: #compact-active}

You can activate **compact download** feature through `console` by deselecting the `Download entire repo` checkbox on the [Create a {{site.data.keyword.bpshort}} Workspace page](https://cloud.ibm.com/schematics/workspaces/create). By default, the checkbox is selected in order to download the full Git repository.

You can also activate **compact download** through the `API or CLI` by using `compact` field in the workspace [create](/apidocs/schematics/schematics#create-workspace), or [update](https://cloud.ibm.com/apidocs/schematics/schematics#replace-workspace) payload, as illustrated in the code block.
```text
{
        "name": "etcdCompactSan",
        "type": [
                "terraform_v0.13"
        ],
        "description": "terraform workspace",
        "tags": [
                "test:bbbranch"
        ],
        "template_repo": {
                "url": "https://github.com/terraform-ibm-modules/terraform-ibm-database/tree/main/examples/simple-etcd"
        },
        "template_data": [{
                "folder": ".",
                "compact": true,
                "type": "terraform_v0.13"
    }]
}
```

## Behaviour of the compact field
{: #compact-behaviour}

- In case the **compact** field is not specified in the workspace create request payload, the default behaviour is `full repository download` or `compact : false`.
- In case the **compact** field is absent in the workspace update request payload, the default behaviour uses the previous `compact` setting.
- Git repository URL is mandatory in both [create](/apidocs/schematics/schematics#create-workspace), or [update](https://cloud.ibm.com/apidocs/schematics/schematics#replace-workspace) request payload.  
- The [GET workspace](/apidocs/schematics/schematics#get-workspace) response includes the compact field, only if the **compact** download mode is `enabled`.
- If the Git repository URL is the root of the repository, as stated in [template](https://github.com/Cloud-Schematics/LEMP), the compact download and full download are the exact same thing. It doesn't matter if the compact checkbox is `selected` or `deselected`.

