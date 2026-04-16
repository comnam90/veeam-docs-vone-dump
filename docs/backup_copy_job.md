---
title: "Backup Copy Job"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_copy_job.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Backup Copy Job


The main backup purpose is to protect your data against disasters and VM failures. Having only one copy of a backup file does not provide the necessary level of safety. To build a successful data protection and disaster recovery plan, you must have at least one independent copy of a backup file offsite, for example, in the remote site. To optimize data transfer between remote sites over the WAN, Veeam Backup & Replication offers the WAN acceleration technology.

To learn more about the 3-2-1 backup strategy and WAN acceleration, see the Veeam Blog article [How to follow the 3-2-1 backup rule with Veeam Backup & Replication](http://www.veeam.com/blog/how-to-follow-the-3-2-1-backup-rule-with-veeam-backup-replication.html).

This report analyzes amount of traffic transmitted to target repository by backup copy jobs, evaluates the efficiency of backup data transfer through WAN accelerators and estimates the amount of network traffic savings.

* The Summary section includes the following elements:

+ The Traffic Efficiency (GB) chart shows the actual amount of traffic read from the source datastore and the amount of traffic transmitted over the network to the target repository.
+ The Traffic Savings by Day (GB) chart shows the amount of traffic saved on each day of the reporting interval (that is, the difference between the amount of read traffic and the amount of transferred traffic).
+ The Savings Ratio by Day chart shows daily fluctuations in the raw data to traffic savings ratio.

* The Accelerators Details table provides details for each pair of WAN accelerators used by backup copy jobs, backup server, job name, service size, actual amount of data transferred to the target repository, amount of saved traffic and savings ratio.

Click a backup copy job name to drill down to details for the job.

* The Job Details table provides detailed information on, backup server, job names, session start time, source, status, source size (GB), backup file sizes, actual amount of data transferred, amount of saved traffic, savings ratio, WAN accelerator status, job type and copy mode.

|  |
| --- |
| Note: |
| For WAN accelerators used in Veeam Cloud Connect jobs, performance data is available only if the target WAN accelerator is present in the Veeam ONE infrastructure. |

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* WAN accelerators: defines pairs of source-to-target WAN accelerators to include in the report.
* Backup copy jobs: defines a list of backup copy jobs to include in the report.
* Period: defines the time period to analyze in the report.

[View Report Example](./reports/Backup%20Copy%20Job.pdf)

Use Case

WAN accelerators allow reducing the amount of network traffic transmitted to remote DR sites by leveraging the deduplication techniques.

This report helps you analyze traffic savings and raise the efficiency of your backup copy jobs.


