---
title: "Backup Infrastructure Audit"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_infrastructure_audit.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Backup Infrastructure Audit


This report tracks configuration changes in your backup environment, providing detailed information about every change for each object.

* The Summary section includes the following elements:

+ The Modifications by Object Types chart illustrates types of changed objects and shows the share of particular object type changes.
+ The Modifications per User chart illustrates which users made changes and shows the share of changes made by each user.

* The Details table lists descriptions of changes made to particular objects.

|  |
| --- |
| Note: |
| * For WAN accelerators used in Veeam Cloud Connect jobs, performance data is available only if the target WAN accelerator is present in the Veeam ONE infrastructure. * Veeam Cloud Connect service providers cannot see performance data for proxies used by tenant data protection jobs. * This report uses Windows Events collected from machines with Veeam Backup & Replication servers deployed and Events Data collection configured. Remote Event Log Management must also be enabled for this report. For details on Remote Event Log Management, see [Firewall Rules](firewall_rules.md). |

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.

* Period: defines the time period to analyze in the report.
* Object types: defines a list of backup infrastructure objects to include in the report (Backup Server, Backup Proxy, Backup Repository, Cloud Gateway, WAN Accelerator, Cloud Repository).
* Users: defines a list of backup users, changes from whom to include in the report.

[View Report Example](./reports/Backup%20Infrastructure%20Audit.pdf)

Use Case

The report allows backup administrators to get details on recent infrastructure changes made by authorized users so that any unwanted action can be quickly rolled back.


