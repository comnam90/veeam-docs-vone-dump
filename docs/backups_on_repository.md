---
title: "Backups on Repository"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backups_on_repository.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Backups on Repository


This report provides detailed information about files stored on backup repositories.

* The Summary section includes the following elements:

+ The Top Repositories by Used Space, % chart displays top 5 repositories in terms of the greatest amount of used space of restore points and the largest amount of backed up data.
+ The Top Repositories by VM/Computer/File Object Storage/Application Backups, GB charts display top repositories in terms of the greatest number of VMs, computers and file sources stored on the repository.

* The Details section provides information on repository type, capacity, free and used space as well as detailed information about backups stored on the repository.

|  |
| --- |
| Important! |
| If one restore point contains several VMs, the report will not provide detailed information on the size of individual backups for every VMs in this restore point. For details on, see [Backup Chain Formats](https://helpcenter.veeam.com/docs/backup/vsphere/per_vm_backup_files.html). |

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Backup repositories: defines a list of backup repositories to include in the report.
* Protected workloads: defines types of objects to include in the report (Virtual machine, Computer, File share, Unstructured Data, Enterprise Application).

[View Report Example](./reports/Backups%20on%20Repository.pdf)

Use Case

This report helps you monitor space usage on backup repositories and the amount of VMs, computers and file sources stored on repositories.


