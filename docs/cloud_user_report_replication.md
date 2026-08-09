---
title: "Cloud Connect User Report (Replication)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/cloud_user_report_replication.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Cloud Connect User Report (Replication)


This report analyzes Veeam Cloud Connect users' replication activity, and provides information on cloud host and storage quota usage over the specified period. The report reveals Veeam Cloud Connect users with the greatest amount of provisioned CPU, memory and storage resources, as well as users with the greatest number of replicated VMs.

* The Summary section includes the following elements:

* The Overview subsections provide information on the total number of Veeam Cloud Connect replication users, number of users with standalone and VMware Cloud Director accounts, configured hardware plans and total VMs replicated. It also includes information on standalone and VMware Cloud Director tenants' compute and storage resources, their capacity, amount of provisioned and used resources.
* The Top Users by VMs Replicated chart displays 5 users with the greatest number of VMs replicated to cloud.
* The Top Users by CPU/Memory/Storage Quota charts display 5 users with the greatest amount of provisioned CPU, memory and storage resources, and visualize the amount of used cloud resources.

* The Report Data display shows the Details and VM Details tables that provide information on Veeam Cloud Connect users, their virtualization platform, hardware plan, number of VMs replicated to cloud on each day of the reporting period, amount of provisioned and used CPU, memory and storage resources. If the resource usage value is approaching the quota limit, the value is highlighted with yellow in the table. If the quota is exceeded, the resource usage value is highlighted with red.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers and Veeam Cloud Connect tenants to include in the report.
* Last <N> weeks/months: defines a time period to analyze in the report.

|  |
| --- |
| Note: |
| * Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, Veeam ONE Web Client may show invalid data for Veeam Backup & Replication reports and dashboards. * To analyze data about replicated VMs in the report, you must connect the target virtualization servers to Veeam ONE. For details on, see [Adding Data Source](connecting_servers.md). |

[View Report Example](./reports/Cloud%20Connect%20User%20Report%20%28Replication%29.pdf)

Use Case

This report allows Veeam Cloud Providers (VCPs) to analyze cloud host and storage configuration and quota usage. The report helps VCPs reveal whether cloud compute and storage resources are approaching their limits, keep an eye on users replicating their workloads to cloud, and decide whether it is necessary to increase users' quotas.

Page updated 2026-08-03

