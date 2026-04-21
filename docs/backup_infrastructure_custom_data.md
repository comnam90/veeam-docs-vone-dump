---
title: "Backup Infrastructure Custom Data"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_infrastructure_custom_data.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Backup Infrastructure Custom Data


This report features a collection of custom properties for Veeam Backup & Replication objects, including backup servers, backup jobs, VMs and computers. The report helps you analyze data protection aspects not covered by Veeam Backup & Replication reports.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Object type: defines a list of Veeam Backup & Replication objects to analyze in the report (Backup server, Job, Virtual machine, Computer, Repository, Workload).
* Columns: defines configuration properties to analyze in the report. The list of available properties will depend on the selected object type. Use the Filter field to search for the necessary properties by name. Note that the number of selected properties must not exceed 50.

|  |
| --- |
| Note: |
| To analyze data about protected VMs in the report, you must connect the target virtualization servers to Veeam ONE. For details on, see [Add Data Source](connecting_servers.md). |

[View Report Example](./reports/Backup%20Infrastructure%20Custom%20Data.pdf)

Use Case

Use the advanced collection of Veeam Backup & Replication object properties to create custom reports that display key aspects of the backup infrastructure and data protection operations.


