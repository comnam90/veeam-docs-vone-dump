---
title: "Protected Files and Object Storage"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/protected_file_object_storage.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Protected Files and Object Storage


This report analyzes backup protection of unstructured data stored in file shares and object storage. The report examines the status of Veeam Backup & Replication protected files and provides details on your infrastructure SLAs.

File shares, buckets and storage accounts that have not been added to any Veeam Backup & Replication inventory are not included in this report.

* The Summary display includes the following elements:

+ The Report Parameters and Summary sections shows the volume of backup objects by their data structure status on your backup servers (Total Unstructured Data, Protected Unstructured Data, Unprotected Unstructured Data).
+ The Unstructured Data Protection Status chart shows the division of your backup data into structured and unstructured instances.
+ The Unstructured Data Last Backup State chart shows the status of your data backups on their success or failure state.
+ The Unstructured Data Last Backup Age chart shows the status of your backup data based on its Recovery Point Objective status.

* The Report Data display includes the following tables:

+ The Details - Protected Unstructured Data table shows the status of all file and object storage sources that are successfully protected by a backup job including server and job names, protection types, processing and restore type data.
+ The Details - Unprotected Unstructured Data table shows the status of all file and object storage sources that are not currently protected by a backup job including server and job names, unprotected reason, processing and restore type data.
+ The Job Details - Protected Unstructured Data table shows the status of all discovered file and object storage sources that are currently protected including groups, backup servers, results, processing data and skipped locations.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.

* RPO: defines the Recovery Point Objective time period which is the maximum period for acceptable loss of data (value, time period definition including minutes, hours, days and so on).
* Processed Percentage: defines the percentage of the acceptable volume of data retention for restore operations.
* Unstructured Data exclusion rule: defines a list of file/object that should be excluded from the report scope. You can enter names explicitly or create a wildcard mask by using the asterisk (\*) to replace any number of characters. Multiple entries are separated by semicolon. For example, the following string will exclude machines with the \_R&D suffix from appearing in the report:\*\_R&D.
* Job types: defines a job type to evaluate in the report (File backup, Object storage backup).

[View Report Example](./reports/Protected%20Files%20and%20Object%20Storage.pdf)

Use Case

This report helps you discover protected objects that breach the target SLA, and jobs that do not operate properly.


