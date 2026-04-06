---
title: "Scale-Out Backup Repository Configuration"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/scaleout_backup_repository.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Scale-Out Backup Repository Configuration


The report provides configuration and resource utilization details for scale-out backup repositories in Veeam Backup & Replication.

* The Summary section provides an overview of configured scale-out repositories, such as the total number of the connected repositories, their capacity and utilization ratio, number of extents, their types, and a policy used for each repository.

+ The Top N Utilized Scale-Out Repositories (GB) and Top N Utilized Extents (GB) charts show most utilized scale-out repositories and their extents, total capacity, used space.

* The Details section provides information on each connected scale-out repository included in the report:

+ The Overview table shows the list of extents in the repository, their type, type of stored backup files, maximum number of concurrent tasks, region, container, operational restore windows settings, immutability, encryption settings, infrequent access storage, storage consumption limit, archive policy settings and deep archive settings.
+ The Dynamics of SOBR free space usage chart shows scale-out repository space usage dynamics over the past month.
+ The Details table provides information about extent capacity and free space in GB, size of full and incremental backups, and the number of VMs and computers stored on each extent.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Top N: defines the maximum number of scale-out repositories to display in the report.

[View Report Example](./reports/Scale-Out%20Backup%20Repository%20Configuration.pdf)

Use Case

The report shows configuration and utilization data for scale-out backup repositories and their extents.


