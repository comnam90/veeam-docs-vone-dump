---
title: "Database Processing Verification"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/database_processing_verification.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Database Processing Verification


This report assesses application servers and application clusters added to the protection groups of Veeam Enterprise Application Plug-ins and lists databases with the information on whether these databases were processed or not.

* The Summary section includes information on the total number of processed and unprocessed databases and number of databases of each platform. Also the section includes the following elements:

+ The Databases by Processing State chart shows the number of processed and unprocessed databases.
+ The Databases by Latest Data Backup Session Status chart shows the number of databases with each status of the latest backup session.
+ The Databases by Platform by Processing State chart shows the number of processed and unprocessed databases of each platform.

* The Details table provides information on processed and unprocessed databases: servers or clusters on which the databases reside, database platforms, protection groups that include databases, backup policies that protect databases, backup repository that stores the database backups, number of backup sessions, date and time of the latest backup session, status of the latest backup session, date and time of the latest log backup session.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.

* Business View objects: defines Business View groups to analyze in the report.
* RPO: defines the maximum amount of data that you may accept to lose, expressed in time. RPO defines the age of the latest backup or replica files required to resume normal operation if system failure occurs. For example, to compile a list of VMs protected on a daily basis, you need to set the RPO value to 1 day or 24 hours.

* Platforms: defines a list of database platforms to include in the report (Oracle Database, SAP HANA, SAP on Oracle, Microsoft SQL Server).
* Backup policies: defines a list of backup policies protecting the databases to include in the report.
* Database exclusion rule: defines a list of databases that should be excluded from the report scope. You can enter database names explicitly or create a wildcard mask by using the asterisk (\*) to replace any number of characters. Multiple entries are separated by semicolon. For example, the following string will exclude databases with the \_R&D suffix from appearing in the report:\*\_R&D.

[View Report Example](./reports/Database%20Processing%20Verification.pdf)

Use Case

A database is a software component that is mission critical for a modern enterprise. The role of database management is constantly expanding, that is why you need to be sure that your databases are safely protected.

The report helps to identify databases that were not added to or were not successfully processed by backup policies.


