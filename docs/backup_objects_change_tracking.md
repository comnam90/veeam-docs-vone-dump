---
title: "Backup Objects Change Tracking"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_objects_change_tracking.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Backup Objects Change Tracking


This report provides detailed information on backup infrastructure configuration changes performed within the reporting period. It includes the exact time of change and the name of the user who did the change.

* The Summary section includes the following elements:

+ The Modifications by Object Types chart illustrates types of changed objects and shows the share of particular object type changes.
+ The Modifications per Initiator chart illustrates which users made changes and shows the share of changes made by each user.
+ The Modifications by Day chart displays distribution of changes performed during report period.

* The Details table lists descriptions of changes made to particular objects.

|  |
| --- |
| Note: |
| Veeam Cloud Connect service providers cannot see performance data for proxies used by tenant data protection jobs. |

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.

* Period: defines the time period to analyze in the report.
* Object types: defines a list of backup infrastructure objects to include in the report (Backup Server, Backup Proxy, Backup Repository, All Items).
* Object inclusion rule: defines names of objects to include in the report. You can enter object names explicitly or create a wildcard mask by using the asterisk (\*) to replace any number of characters. Multiple entries are separated by semicolon.
* Users: defines a list of backup users, changes from whom to include in the report.

[View Report Example](./reports/Backup%20Objects%20Change%20Tracking.pdf)

Use Case

The report allows backup administrators to get details on recent infrastructure modifications made to target objects so that any unwanted action can be quickly rolled back.


