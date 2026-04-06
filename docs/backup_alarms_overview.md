---
title: "Backup Alarms Overview"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_alarms_overview.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Backup Alarms Overview


This report provides an overview of the data protection health state. It allows you to track Veeam Backup & Replication alarms triggered by Veeam ONE Client, and see most affected Veeam Backup & Replication jobs and components.

* The Summary display includes the following elements:

+ The Job Issues History chart displays the total number of warnings and errors for jobs for each day within a reporting period.
+ The Backup Infrastructure Alarms chart displays the total number of warnings and errors for infrastructure alarms for each day within a reporting period.
+ The Top 10 VMs with Issues table lists 10 most affected VMs and the number of alarms triggered for each machine.
+ The Top 5 Jobs with Issues chart displays top 5 jobs that caused more alarms than other jobs.
+ The Top 10 Triggered Alarms table shows 10 the most frequent alarms and how many times each alarm was triggered.

* The Report Data display shows the Details table that provides information on affected backup infrastructure objects and displays how many alarms were triggered.

The report also calculates a trend for each object. It compares information on alarms triggered over the reporting period (day/week/month/year) with the number of alarms triggered during the day/week/month/year previous to the reporting period. For example, if the selected reporting period is one month, the trend will use the month previous to the reporting period to calculate the trend. By comparing two equal periods, the report shows whether the number of triggered alarms increased or reduced. Therefore, you can track data protection health state changes.

Click a number in the Alarms Triggered column to drill down to alarm details.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines backup infrastructure objects to analyze in the report.
* Period: defines the time period to analyze in the report.
* Alarm types: defines a list of data protection object types to analyze and include in the report.

* Alarms: defines a list of alarms to analyze in the report. The options in the list depend on the selected Alarm types parameter.

For details on alarms you can select in the list, see [Veeam Backup & Replication Alarms](backup_alarms_events.md).

[View Report Example](./reports/Backup%20Alarms%20Overview.pdf)

Use Case

The report provides an overview of the data protection health state, shows the list of the frequently triggered alarms and displays the most affected backup infrastructure objects.


