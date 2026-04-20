---
title: "Over-Provisioned Backup Repositories"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/cloud_overprovisioned_repositories.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Over-Provisioned Backup Repositories


When configuring cloud repositories, cloud administrators can allocate more storage space than there is available on the underlying backup repository. This report helps you assess the potential impact of excessive over-provisioning for cloud repositories.

* The Summary display includes the following elements in addition to individual charts for each connected repository:

+ The Top 5 Over-provisioned Repositories chart shows 5 repositories whose amount of provisioned storage space exceeds the total capacity.
+ The Top 5 Under-provisioned Repositories chart shows 5 repositories whose amount of provisioned storage space is way below the total capacity.
+ The Top Repositories with Least Amount of Free Space table displays top 5 repositories that will run out of free space sooner than other repositories.

* The Report Data display includes Details table that provides information on the repository capacity, amount of free space, amount of space provisioned to Veeam Cloud Connect tenants, provisioning ratio and the number of VMs and computers stored on the repository.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers and repositories to include in the report.
* Space utilization: defines the threshold for the amount of space in use on repositories.
* Free space (min): defines the threshold for the amount of free space left on repositories.
* Show graphs: defines whether to include charts in the report output.

[View Report Example](./reports/Over-Provisioned%20Backup%20Repositories.pdf)

Use Case

The report analyzes repository space utilization trend and calculates the number of days left before storage utilization will breach the specified threshold.


