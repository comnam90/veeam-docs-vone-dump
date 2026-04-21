---
title: "Current Backup Alarms State Overview"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/current_backup_alarms_state.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Current Backup Alarms State Overview


This report shows all unresolved alarms that Veeam ONE Client triggered for the Veeam Backup & Replication infrastructure.

* The Summary display includes the following elements:

+ The Total Issues Number chart shows the total number of alarms specified in the Alarm Status parameter.
+ The Top 10 Issues table displays 10 most frequent unresolved alarms, their status, and how many times they were triggered.

* The Report Data display shows objects names, backup servers, object types, names of triggered alarms, their status, repeat count, triggering events and time, and affected backup infrastructure objects.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Alarms statuses: defines statuses of alarms to display in the report (Acknowledged; Error; Error, Warning; Error, Warning, Acknowledged).

[View Report Example](./reports/Current%20Backup%20Alarms%20State%20Overview.pdf)

Use Case

You can use this report to detect and resolve current and the most pressing issues with Veeam Backup & Replication.


