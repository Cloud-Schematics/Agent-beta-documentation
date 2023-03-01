---

copyright:
  years: 2017, 2022
lastupdated: "2022-11-05"

keywords: manage backup, schematics backups

subcollection: schematics

---

{{site.data.keyword.attribute-definition-list}}


# Managing backups
{: #manage-backups}

Backups for each {{site.data.keyword.bpshort}} instance data level are available. Some general information about backups.

* One backup is taken every day.
* Backups are available for 30 days.
* Backups cannot be deleted.
* Scheduling of the daily backup is not configurable.
* Backups are cross-regionally durable. Backups are stored across multiple regions, and restored to other regions, except for `US` and `EU` region, which cannot cross-regional boundaries.
* Pruning is achieved by configuring expiration policy in for backup Cloud Object Storage buckets.
* Backup storage is encrypted. If you need to manage the encryption keys, you can do so with the Key Protect integration. Otherwise, they are encrypted with a key that is automatically generated for your deployment.
* Backups are restored across accounts, but only by using the API or command-line.
* Backups are supported at {{site.data.keyword.bpshort}} instances level.
* Backups and restore at the user level are not supported.


## Restoring a backup
{: #restoring-backups}

Backups are restored at the {{site.data.keyword.bpshort}} instance data level for `US` and `EU` region. For the restore operation, you need to provide the date to locate the backup objects for restore operation. Restore operation happens in following phases to ensure operational readiness of {{site.data.keyword.bpshort}}. 

* Restore accounts database to target Cloudant instance to ensure that existing users can start by using {{site.data.keyword.bpshort}}.
* Restore Cloud Object Storage content.
* Restore metadata database contents.
* Restore operation in each of the phase first restores data from raw backup and then apply changes from incremental backup.

By default the new instance is auto sized to the same disk and memory allocation as the source instance at the time of the backup you are restoring from. If you need to adjust the resources that are allocated to the new instance. Be sure to allocate enough for your resource and workload; if the instance is not given enough resources, the restore fails.

You cannot delete the source instance while the backup is restoring. You must wait until the new instance is provisioned and the backup is restored and delete the old instance. Deleting an instance deletes its backups so not only the restore fail, you might not be able to recover the backup.
{: note}


## Steps to restore
{: #steps-to-restore}

Backups are automated to execute once in 24 hours in {{site.data.keyword.bpshort}}. You can restore the backup of specific date and time by following steps.

You can restore your data to a new, or existing empty Cloud Object Storage/Cloudant. You must have the required permission to execute the scripts provided in the [branch](https://github.ibm.com/blueprint/schematics-deploy).

Restoring a backup is supported when you restore into an empty database. If you delete all documents from a database, document deletion records are still present for replication consistency purposes. A database that contains only deleted documents is not considered empty, and so cannot be used as the target when you restore a backup.
{: note}

1. (Prerequisite) Create a new cluster by using {{site.data.keyword.bpshort}} Workspace.
2. Create a target Cloud Object Storage and a Cloudant database to restore.
3. Fork the [{{site.data.keyword.bpshort}} deploy branch](https://github.ibm.com/blueprint/schematics-deploy).
4. From the forked branch, configure the following parameters in `operators/restore/restore.yaml` file.

    | Name | Value | 
    | ---- | -----|
    | BACKUP_DATE| Specify the back date. For example, `20052021`.|
    | TARGET_COS_ENDPOINT | Specify your target COS endpoint URL.|
    | TARGET_COS_BUCKET_NAME | Specify name of the COS bucket. |
    | TARGET_CLOUDANT_URL | Specify your target Cloudant URL. |
    | CLOUDANT_IAM_API_KEY | Specify your IAM API key. |
    | TARGET_COS_ACCESS_KEY_ID | Specify your COS access key ID. |
    | TARGET_COS_SECRET_ACCESS_KEY | Specify your COS secret access key. |
    {: caption="Parameters to restore" caption-side="bottom"}

5. Execute `kubectl apply -f operators/restore/restore.yaml` command from the command-line.
6. Review the restored results and logs.

You completed the restore the Cloud Object Storage and a Cloudant resource. For more information, see [Disaster recovery and backup](#restoring-backups).




