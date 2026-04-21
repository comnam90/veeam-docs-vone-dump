---
title: "Data Sovereignty Violations"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/data_sovereignty_violations.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Data Sovereignty Violations


This report shows potential data sovereignty violations by listing all protected objects with backups or replicas residing in a different location.

* The Summary display contains charts that display the sovereignty violations of production data, their backups, backup copies and replicas.
* The Report Data display contains the Data Sovereignty Violations tables that show details on the location mismatch of backups, backup copies, tapes and replicas for a data source grouped by Veeam Backup & Replication server name. The Objects with no Location Tag table displays all objects in the infrastructure that have no location tag grouped by the type of object.

Report Parameters

You can specify the following report parameters:

* Scope: defines a list of Veeam Backup & Replication servers to include in the report.
* Protection types: defines a list of Veeam Backup & Replication jobs to include in the report.
* Workload types: defines whether physical computers or virtual machines are included in the report.

|  |
| --- |
| Note: |
| Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, Veeam ONE Web Client may show invalid data for Veeam Backup & Replication reports and dashboards. |

[View Report Example](./reports/Data%20Sovereignty%20Violations.pdf)

Use Case

Veeam Backup & Replication supports a notion of location which you can assign to virtual infrastructure, backup infrastructure and agent management objects. Location settings helps to monitor where production data and their copies and replicas reside geographically.

The report analyzes whether any backups, backup copies and replicas reside in a location different from a data source and displays results as pie charts. This visual representation will help you identify which jobs and objects violate data protection regulations accepted in your organization.


