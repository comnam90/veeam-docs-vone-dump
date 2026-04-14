---
title: "Cloud Connect User Report (Backup)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/cloud_user_report_backup.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Cloud Connect User Report (Backup)


This report gathers information on storage quota usage and activity of users that consume Veeam Cloud Connect repository resources. The report forecasts the date when cloud repositories will run out of available storage quota and helps you ensure there is enough space for backup data at any point in time.

* The Summary display includes the following elements:

+ The Overview subsections provide information on the total number of users, the number of users who were active/inactive during past 30 days, the number of users who will run out of quota in the next 30 days, the total number of cloud repositories, the total storage quota, total amount of space used and left on repositories, and number of VMs and computers.

+ The Top Users By Days Left to Reach Quota and Top Users By Quota Utilization (%) charts display 5 users that will run out of space sooner than other users and 5 users with the highest level of space utilization.

* The Report Data display provides the Tenant Detail and Tenant Session Details tables that show information on user activity on each day of the reporting period, the number of VMs and computers in backups stored on the repository, cloud repository quota assigned to the user, the amount of used and free space on the repository, amount of data transferred to the cloud, space usage trend, the date the user contract expires and the last time and date when the user was active. The report also forecasts the number of days left before the user runs out of quota.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers and Veeam Cloud Connect tenants to include in the report.
* Last <N> weeks/months: defines the time period to analyze in the report.

|  |
| --- |
| Note: |
| The number of VMs and computers in backups on cloud repositories may differ from the number of VMs and computers specified in Veeam Backup & Replication. Veeam Backup & Replication shows the number of licensed VMs and computers only, while Veeam ONE shows the total for licensed and stored VMs and computers. |

[View Report Example](./reports/Cloud%20Connect%20User%20Report%20%28Backup%29.pdf)

Use Case

This report allows Veeam Cloud Providers (VCPs) to analyze configuration and quota usage on cloud repositories. The report helps VCPs define which repositories are running out of free space, keep an eye on user activity and decide whether to increase quota for the users.


