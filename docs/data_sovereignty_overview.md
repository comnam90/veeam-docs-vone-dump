---
title: "Data Sovereignty Overview"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/data_sovereignty_overview.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Data Sovereignty Overview


This report lists all protected objects, backups and replicas grouped by location.

* The Summary display contains charts that display locations of production data, their backups, backup copies and replicas.
* The Report Data display shows the following:

* The Backup Infrastructure Objects table lists all objects of a backup infrastructure and their locations.
* The Data Location table shows details on the location of backups, backup copies and replicas for data sources grouped by production data location.

Report Parameters

You can specify the following report parameters:

* Infrastructure Objects: defines a list of Veeam Backup & Replication servers to include in the report.
* VM and computer locations: defines a list of locations configured on monitored Veeam Backup & Replication servers.

|  |
| --- |
| Note: |
| Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, Veeam ONE Web Client may show invalid data for Veeam Backup & Replication reports and dashboards. |

[View Report Example](./reports/Data%20Sovereignty%20Overview.pdf)

Use Case

Veeam Backup & Replication supports a notion of location which you can assign to virtual infrastructure, backup infrastructure and agent management objects. Location settings helps to monitor where production data and their copies and replicas reside geographically.

The report analyzes the location of backups, backup copies and replicas for a data source and displays it as pie charts. This visual representation will help you monitor your data in a geographically disperse infrastructure.


