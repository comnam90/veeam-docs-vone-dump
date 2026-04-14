---
title: "Restore Operator Activity"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/restore_operator_activity.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Restore Operator Activity


This report allows you to keep an eye on all types of restore actions performed across the selected Veeam Backup & Replication servers. The report analyzes all guest file, application-level and full VM restore activities performed by any authorized user and arranges this information by restore date (from newest to oldest).

* The Summary section includes the following elements:

+ The Restores by User chart shows the number of restore actions performed by each authorized user.
+ The Restore Session Statistics chart shows the number of restore actions performed during the reporting period.

* The Details table provides information on restore actions, including restore type, initiating user, name of the recovered item or VM, restore point age, the intended restore destination and the success status of the completed job.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Users: defines backup administrators and restore operators whose restore activity must be analyzed.
* Restore type: defines a restore type to evaluate in the report (Full VM restore\*, Guest files (OS and NAS files), Application item restores, Restore from tape, All).
* Period: defines the time period to analyze in the report.

\*This entry includes the following components: full VM restores, Instant VM Recovery, restore of virtual disks, VM files, Replica Failover.

[View Report Example](./reports/Restore%20Operator%20Activity.pdf)

Use Case

Since data can be restored from the Veeam Backup & Replication console, Veeam Backup Enterprise Manager and Veeam self-service restore portals, using PowerShell scripts or through REST API, in large environments with multiple backup administrators it is often hard to track all performed restore actions.

The report helps you track the initiator of each restore attempt, find out the most popular recovery items and establish historical trends.


