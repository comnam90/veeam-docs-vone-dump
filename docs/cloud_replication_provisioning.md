---
title: "Cloud Connect Replication Provisioning"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/cloud_replication_provisioning.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Cloud Connect Replication Provisioning


This report allows you to identify cloud hosts, clusters and datastores that are over-provisioned and under-provisioned with resources and make sure CPU, memory and storage resources are allocated efficiently.

* The Summary display includes the following elements:

+ The Top 5 Over-provisioned Hosts/Clusters (by CPU), GHz chart displays 5 most over-provisioned cloud hosts and clusters by CPU and displays their total CPU capacity and the amount of computing resources provisioned for them.
+ The Top 5 Over-provisioned Hosts/Clusters (by Memory), GB chart displays 5 most over-provisioned cloud hosts and clusters by memory and displays their total memory capacity and the amount of memory resources provisioned for them.
+ The Top 5 Over-provisioned Datastores, GB chart displays 5 most over-provisioned cloud datastores by memory and displays their total memory capacity and the amount of memory resources provisioned for them.

* The Report Data display provides the Provisioned Hosts (by CPU), Provisioned Hosts (by Memory) and Provisioned Datastores tables that display information on cloud hosts and clusters that are over-provisioned and under-provisioned with CPU, memory and storage resources and provides information about resource allocation on these hosts.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of virtual infrastructure objects to include in the report.
* CPU Utilization Thresholds: defines minimum and maximum CPU utilization thresholds in percent.
* Memory Utilization Thresholds: defines minimum and maximum memory utilization thresholds in percent.
* Datastore Utilization Thresholds: defines minimum and maximum storage utilization thresholds in percent.

|  |
| --- |
| Note: |
| * Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, Veeam ONE Web Client may show invalid data for Veeam Backup & Replication reports and dashboards. * To analyze data about replicated VMs in the report, you must connect the target virtualization servers to Veeam ONE. For details on, see [Add Data Source](connecting_servers.md). * When specifying threshold intervals, note the following:  + If the amount of provisioned CPU, memory or storage resources is higher than the specified maximum threshold, an object (such as a host, cluster or datastore) is considered over-provisioned. + If the amount of provisioned CPU, memory or storage resources is less than the specified minimum threshold, an object (such as a host, cluster or datastore) is considered under-provisioned. + If the amount of provisioned CPU, memory or storage resources is between the minimum and maximum thresholds, an object (such as a host, cluster or datastore) will not be included in the report charts or tables as the provisioning value is considered normal. |

[View Report Example](./reports/Cloud%20Connect%20Replication%20Provisioning.pdf)

Use Case

The report helps define whether existing hardware plans match hosts and datastores capabilities. Use this data to avoid potential issues that may be caused by excessive over-provisioning of cloud replication hosts.


