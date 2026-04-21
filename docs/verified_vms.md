---
title: "Verified VMs"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/verified_vms.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Verified VMs


This report provides information on SureBackup jobs performed by Veeam Backup & Replication and displays the summary of verified VMs.

SureBackup and SureReplica technologies allow virtualization administrators to validate the recoverability of created backups and replicas in an isolated test environment by examining their key viability indicators. This ensures that your backups and replicas are fully reliable and minimizes the risk of data loss in case a VM fails.

* The Summary section provides an overview on the number of protected and verified VMs, displays the status history of verified VMs and verification rate during the reporting period.
* The Details table provides information on VMs tested and verified with SureBackup and SureReplica, including the number of failed verifications, last verified restore point, status of the last verification and the results of VM verification tests (ping commands, scripts execution and heartbeat messages).

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Last <N> weeks/months: defines the time period to analyze in the report.
* Platform: defines whether to analyze VMware vSphere or Microsoft Hyper-V infrastructure.
* Job type: defines a job type to evaluate in the report (Backup and replication jobs, Backup jobs only, Replication jobs only).

|  |
| --- |
| Note: |
| Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, Veeam ONE Web Client may show invalid data for Veeam Backup & Replication reports and dashboards. |

[View Report Example](./reports/Verified%20VMs.pdf)

Use Case

This report helps administrators to quickly review the results of completed SureBackup jobs and confirm that the created backups and replicas are recoverable and error-free. This ensures that production VMs are reliably protected against failures and data corruption.


