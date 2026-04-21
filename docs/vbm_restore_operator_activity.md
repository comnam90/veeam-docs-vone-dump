---
title: "Restore Operator Activity (Veeam Backup for Microsoft 365)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vbm_restore_operator_activity.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Restore Operator Activity (Veeam Backup for Microsoft 365)


This report allows you to monitor all types of restore actions performed across your selected Veeam Backup for Microsoft 365 servers. The report analyzes restored applications including mail, OneDrive, sites and Teams performed by any authorized user that can additionally be grouped by customized settings.

* The Summary section includes the following elements:

+ The Top 10 Operators by Restores list shows the top 10 users who have initiated the largest number of restore sessions.
+ The Top 10 Restored Objects list shows the top 10 objects with the largest number of restore sessions.
+ The Restores by Type chart shows restore operations by type (Restore, View, Save, Export, Send).
+ The Restores by Application chart shows the number of restores by type of application (Mail, OneDrive, Site, Teams).
+ The Restore Sessions by Application Type chart and table shows the number of restore sessions per day by application type (Mail, OneDrive, Site, Teams).
+ The Restore Sessions Details table provides information on each restore action, including restore type, initiating user, name of recovered item, restore start time and item size, intended restore destination and status of intended job.

* The Report Data display provides information on each restore action, including restore type, initiating user, name of recovered item, restore start time and item size, intended restore destination and status of intended job.

|  |
| --- |
| Note: |
| Veeam ONE only collects information about restores from Veeam Backup for Microsoft 365 versions 8 and above. Restore data from versions below 8 is not presented in this report. |

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup for Microsoft 365 servers to include in the report.
* Organizations: defines the Microsoft organizations to analyze in the report.
* Restore types: defines the list of restore types to analyze in the report (Restore, View, Save, Export and Send).
* Application types: defines the list of application types to analyze in the report.

* Period: defines the time period to analyze in the report.

[View Report Example](./reports/Restore%20Operator%20Activity%20%28Veeam%20Backup%20for%20Microsoft%20365%29.pdf)

Use Case

As data can be restored from the Veeam Backup for Microsoft 365 console, using PowerShell scripts or through REST API, in large environments with multiple backup administrators it is often hard to track all performed restore actions.

This report helps you track the initiator of each restore attempt, asses the most regularly restored objects and establish historical trends.


