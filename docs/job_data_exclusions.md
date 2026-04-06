---
title: "Job Data Exclusions"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/job_data_exclusions.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Job Data Exclusions


The report provides information about objects, such as VMs, disks, folders and templates, excluded from backup, backup copy and replication jobs in Veeam Backup & Replication.

* The Summary section includes Jobs with Object-level Exclusions, Jobs with Disk Exclusions and File System Exclusions charts that display the share of jobs with excluded objects, disks and file system objects and jobs without exclusions.
* The Exclusions tables show exclusion settings and objects excluded from processing in Veeam Backup & Replication.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Job type: defines types of Veeam Backup & Replication jobs to analyze in the report (Backup, Replication, Backup Copy, All types).
* Jobs: defines Veeam Backup & Replication jobs to analyze in the report.

[View Report Example](./reports/Job%20Data%20Exclusions.pdf)

Use Case

The report allows you to review exclusion settings configured in jobs and check objects excluded from backups and replicas. For more information in exclude types available in Veeam Backup & Replication, see section [Data Exclusion](https://helpcenter.veeam.com/docs/backup/vsphere/data_exclusion.html) of the Veeam Backup & Replication User Guide.


