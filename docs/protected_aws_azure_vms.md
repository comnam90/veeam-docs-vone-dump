---
title: "Protected Cloud Instances"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/protected_aws_azure_vms.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Protected Cloud Instances


This report analyzes backup, snapshot, replication, backup copy and archive protection of cloud instances in your Veeam Backup for Microsoft Azure, Amazon Web Services and Google Cloud Platform cloud infrastructures. Note that report scope includes only target repositories connected to Veeam Backup & Replication server.

A cloud instance is considered Protected if there is at least one valid backup, snapshot, replication, backup copy or archive protection restore point that meets the designated RPO for it. A cloud instance is considered Unprotected if it has outdated or missing restore points.

* The Summary section includes the following elements:

+ The Instances by Protection State chart shows the number of protected and unprotected cloud instances.
+ The Instances by Last Session Status chart shows status of the latest job session for discovered cloud instances.
+ The Unprotection Reason chart shows reasons for non-compliance with the specified RPO requirements.

* The Details section provides information on all protected and unprotected cloud instances including instance ID, protection type, policy name, backup, snapshot, replication, backup copy or archive protection target, number of available restore points and date and time of the latest backup, snapshot, replication, backup copy or archive protection.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* RPO (Recovery Point Objective): defines the maximum amount of data that you may accept to lose, expressed in time. RPO defines the age of the latest backup, snapshot, replication, backup copy or archive protection files required to resume normal operation if system failure occurs. For example, to compile a list of cloud instances protected on a daily basis, you need to set the RPO value to 1 day.
* Instance types: defines a type of cloud instances to include in the report (Amazon Web Services: EC2, RDS, EFS, VPC, DynamoDB, FSx, Redshift, Redshift Serverless; Microsoft Azure: Virtual Machines, SQL Database, Files, Virtual Network, Cosmos DB; Google Cloud: VMs, SQL, Spanner).
* Protection types: defines a type of protection to include in the report (Backup, Snapshot, Replication, Archive).
* Instance filter type: defines the filter type to apply to cloud instances defined in the Rule section (Inclusion, Exclusion)
* Rule: defines a list of cloud instances that should be included or excluded from the report scope depending on the Instance filter type selection. You can enter cloud instance names explicitly or create a wildcard mask by using the asterisk (\*) to replace any number of characters. Multiple entries are separated by semicolon. For example, the following string will exclude cloud instances with the \_R&D suffix from appearing in the report:\*\_R&D.

|  |
| --- |
| Note |
| The Region and Instance ID columns may display an entry as Undefined. This can occur either when a Veeam Backup server or platform service is unavailable, or if an instance has been deleted but restore points remain. Veeam Backup & Replication does not store instance ID or region information, leading to these fields displaying Undefined in the report. |

[View Report Example](./reports/Protected%20Cloud%20Instances.pdf)

Use Case

When you set up your backup jobs based on resource groups or employ complex exclusion parameters in job properties, some cloud instances may turn out to be excluded from the backup policies and therefore will lack proper protection.

This report displays a list of cloud instances protected by up-to-date backups and snapshots, as well as a list of unprotected cloud instances which have outdated or missing restore points. This information helps you validate the state of data protection in your organization.


