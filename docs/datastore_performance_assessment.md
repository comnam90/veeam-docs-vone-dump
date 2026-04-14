---
title: "Datastore Performance Assessment"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/datastore_performance_assessment.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Datastore Performance Assessment


This report analyzes datastore performance and detects whether your datastores can sustain the current workload.

* The Assessment Results table shows the number of hosts connected to each datastore included in the report scope, the number of VMs that store data on the datastores, the number of virtual disks, and the average latency/IOPS values for each datastore. The report also provides recommendations on how to meet the defined parameters.
* The Top Datastores by Latency, Top Datastores by IOPS, Bottom Datastores by Latency and Bottom Datastores by IOPS charts show 5 most and least loaded datastores in terms of the highest and the lowest IOPS and latency values.

* The Details sections show performance charts with IOPS and latency statistics for each datastore, and details tables with latency and IOPS values for every host connected to the datastore.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Datastores: defines the datastore to analyze in the report.
* Interval: defines the time period to analyze in the report.
* Read latency (max) threshold: defines a threshold for the highest latency value for read operations. If the average read latency value for a datastore breaches the threshold, the datastore will be highlighted with red.
* Write latency (max) threshold: defines a threshold for the highest latency value for write operations. If the average write latency value for a datastore breaches the threshold, the datastore will be highlighted with red.
* Read operations count (max) threshold: defines a threshold for the maximum number of read ope rations. If the number of read operations for a datastore breaches the threshold, the datastore will be highlighted with red.
* Write operations count (max) threshold: defines a threshold for the maximum number of write operations. If the number of write operations for a datastore breaches the threshold, the datastore will be highlighted with red.

[View Report Example](./reports/Datastore%20Performance%20Assessment.pdf)

Use Case

Veeam Backup & Replication provides Backup I/O Control, a capability that allows you to define latency and IOPS thresholds for any datastore:

* The Stop assigning new tasks to datastore at option means that when the backup server is assigning a proxy for the virtual disk, it will take latency (IOPS) into consideration, and the backup job will wait for the datastore to become free before starting the backup.
* The Throttle I/O existing tasks at option is designed for situations when a backup job is already running and latency becomes an issue due to an external load. For example, if a SQL maintenance process were to start running in a VM using the same datastore as the backup job, then the backup job will automatically throttle its read I/O from the datastore so that latency drops below the specified threshold.

The report helps you assess current load on your datastores and make sure that by specifying the certain thresholds in Veeam Backup & Replication you maximize possible backup performance while minimizing the impact on production workloads.


