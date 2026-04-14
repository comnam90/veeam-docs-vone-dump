---
title: "Cluster Configuration (vSphere)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/cluster_configuration_vmware.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Cluster Configuration (vSphere)


This report documents the current configuration of clusters in your infrastructure.

* The Summary section charts provide an overview of cluster resources in terms of memory, CPU and storage utilization.
* The Details table provides information on each cluster, including total number of hosts in the cluster, the amount of allocated resources and statuses of HA (High Availability) and DRS (Distributed Resource Scheduler) features.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Cluster type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

[View Report Example](./reports/Cluster%20Configuration%20%28vSphere%29.pdf)

Use Case

The report allows you to keep an eye on the state of hardware resources provisioned to your clusters, and to verify configuration settings applied to these clusters. This may help you balance workloads and right-size the environment to attain higher performance.


