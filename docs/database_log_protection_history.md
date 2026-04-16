---
title: "Database Log Protection History"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/database_log_protection_history.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Database Log Protection History


This report provides historical overview of all database log backup jobs. It also includes the list of protected and unprotected databases for each virtual and physical machine. The report helps you ensure that critical databases are properly protected and that transaction logs for these databases have been successfully backed up.

A database is considered to be Protected if it was backed up at least once during the last backup job session. A database is considered to be Unprotected if it was not backed up during the last backup job session.

* The Summary display includes the following elements:

+ The Databases by Protection State chart shows the number of protected and unprotected databases and databases excluded from processing.
+ The SLA chart shows how many log backup intervals within the specified RPO period completed with successful log shipment (in percentage).
+ The Job Sessions by Status chart shows results of job sessions.
+ The Summary panel shows the number of configured backup jobs, the total number of VMs and computers included in these jobs, the number of processed application servers and clusters, and the total number of hosted databases.

* The Details table provides additional information on the efficiency of executed jobs, number of protected, unprotected and excluded databases, number of missed intervals, actual difference between configured log backup interval and time actually required.
* The Backup Copy Job Details table provides information about each backup copy job. This table helps users monitor job progress and troubleshoot issues with backup copy operations.
* The Database Protections Details table provides protection details for monitored databases. This table enables users to verify database backup coverage and identify databases that may require attention.

|  |
| --- |
| Note |
| Values displayed in the SLA column on this report are for the average of the selected period, not the latest session. |

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Database types: defines a list of database types to include in the report (Microsoft SQL, Oracle Database, PostgreSQL, SAP HANA, SAP on Oracle, SAP on MaxDB).
* Job types: defines the types of jobs that can be selected to include in the report (VM backup, Agent backup, Agent backup policy, Application backup policy).
* Backup jobs: defines a list of backup jobs to include in the report. Note that the report will include information on Oracle backup jobs only for Veeam Backup & Replication servers version 11 or later.
* Show backup copy (immediate copy) jobs: defines whether to include information on immediate backup copy jobs in the report.
* Interval: defines the time period to analyze in the report.

[View Report Example](./reports/Database%20Log%20Protection%20History.pdf)

Use Case

A database is a software component that is mission critical for a modern enterprise. The role of database management is constantly expanding, that is why you need to be sure that your databases are safely protected.

The report allows you to track historical statistics for SQL and Oracle backup jobs, ensure that the configured jobs allow you to meet the desired SLA requirements.

|  |
| --- |
| Note |
| This report supports SQL, PostgreSQL and Oracle database log backup jobs and Enterprise Application plugins. |


