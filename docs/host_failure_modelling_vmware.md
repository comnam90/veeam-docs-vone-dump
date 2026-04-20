---
title: "Host Failure Modelling (vSphere)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/host_failure_modelling_vmware.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Host Failure Modelling (vSphere)


This report allows you both to simulate a failure of one or more hosts, and forecast CPU and memory usage for clusters.

* The Summary section provides an overview of the current state of your infrastructure (the total number of clusters, hosts, datastores and VMs) and shows recommendations on resource allocation.

* The Modelling Results charts display the total amount of CPU and memory resources left and lost in clusters in case of a host failure. The VMs Migration Count chart shows the number of VMs that will need to be relocated to another host (VMs to Migrate) and the number of VMs that will operate as usual (Unaffected VMs) in case of a host failure.

* The Details table provides details on CPU and memory current and predicted utilization for all clusters included in the report.

Click a cluster name to drill down to details on current and predicted resource usage for the cluster. Click a number in the Affected VMs column to drill down to details for the VMs that need to be migrated.

* The Recommendations section provides recommendations for the resources whose utilization thresholds will be breached.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Number of failed hosts: defines the number of random hosts for which you want to simulate a failure.
* Failed hosts: defines a list of hosts for which you want to simulate a failure.
* Business View migration scope: filters report scope objects that belong to the selected Business View groups.
* CPU utilization threshold (%): defines the CPU usage threshold as a percentage of total cluster CPU resources.
* Memory utilization threshold (%): defines the used memory threshold as a percentage of total cluster memory resources.

[View Report Example](./reports/Host%20Failure%20Modelling%20%28vSphere%29.pdf)

Use Case

The report provides recommendations on appropriate resource allocation, which can help prevent possible CPU and memory resource shortfalls in future and maintain the optimal performance of your infrastructure.


