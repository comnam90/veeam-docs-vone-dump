---
title: "Recovery Verification Overview"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/surebackup_jobs_overview.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Recovery Verification Overview


This report validates the completion status of SureBackup jobs and displays the results of recovery verification tests. The report helps you reveal the list of operational VMs that can be restored from the produced backup or replicas.

* The Summary section includes the following elements:

+ The SureBackup Job Status chart chows the latest state of SureBackup job sessions.
+ The Verified VMs Status chart shows the percentage of VMs for which the latest SureBackup job session completed successfully, completed with warnings or failed, and percentage of VMs for which SureBackup jobs have not been run at all.
+ The Antivirus Check chart shows the results of the last antivirus check run.

* The Details table shows the results of completed SureBackup job sessions, including the name and status of the evaluated SureBackup job, the list of VMs included in the job, the application type of the verification model used to test each VM, the verification date and the date when backup or replica was created, the results of ping, heartbeat and script execution commands executed to verify recoverability of created copies, the version of the antivirus installed on a VM and the last antivirus check result.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.

* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Job type: defines a SureBackup job type to evaluate in the report (Backup, Replica, All).

|  |
| --- |
| Note: |
| Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, you will not be able to generate the report based on Business View objects. |

[View Report Example](./reports/Recovery%20Verification%20Overview.pdf)

Use Case

SureBackup is a unique Veeam technology that ensures that the VM being backed up or replicated is safely recoverable from the media. SureBackup allows you to validate backups and replicas of your VMs without impacting the production infrastructure. You can automatically verify every created restore point of every VM and ensure that they will function as expected in case a disaster strikes.

The report helps you discover issues that occur in operation of your backup infrastructure. It provides details on the state of SureBackup jobs so that you can reconfigure current job settings or include mission critical VMs in SureBackup jobs.


