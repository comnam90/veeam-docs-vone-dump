---
title: "How Many More VMs Can be Provisioned"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vms_to_provision_vmware.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# How Many More VMs Can be Provisioned


This report calculates the number of additional VMs that your existing infrastructure can support before the resource utilization reaches the specified threshold value.

The report evaluates total capacity of your infrastructure and provides estimation of how many sample VMs of a certain profile can be added without causing the specified resource utilization threshold to be breached. Calculation of additional VM sets is based on the predicted future performance of the sample VM and the predicted virtual infrastructure capacities.

* The Summary section provides information on total number of VMs in capacity, number of existing VMs and VMs that can be added, and VM configuration and average performance.

+ The Constraining Resource Per Each Object table displays resources for which the specified thresholds will be breached first for each host, cluster or datastore.

* The Details table provides information on average and predicted resource usage for each host, cluster or datastore.

Click a host, cluster or datastore name in the details table to drill down to in-depth forecast information for the host, cluster or datastore.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Host type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Datastores: defines a list of datastores to analyze in the report.
* VM sample: defines a VM profile that will be used as a sample for calculating the number of VM sets:

+ If you choose a specific VM, the report will calculate how many similar VMs can be added.
+ If you choose Average VM configuration, the report will assess average configuration across all your VMs, and calculate how many VM of this configuration can be added.

Note that VMs in the profile must be currently in the powered on state, and that performance data collection must be completed for the given VMs.

* Count reserved CPU and memory: defines whether CPU and memory reservations should be taken into account when calculating the number of VMs to be added.
* CPU utilization (%): defines the CPU usage threshold as a percentage of total cluster CPU resources.
* Memory utilization (%): defines the used memory threshold as a percentage of total cluster memory resources.
* Space utilization (%): defines the threshold for the maximum amount of space in use on a datastore.
* Free space (min): defines the threshold for the minimum amount of free space in GB left on a datastore.
* Read speed (max): defines the threshold for read rate in MB per second for datastores.
* Write speed (max): defines the threshold for write rate in MB per second for datastores.
* Max vCPUs per physical core: defines the threshold for the maximum number of vCPU cores per a single instance of the logical CPU core.
* Put 1 host from each cluster into maintenance mode: defines whether to simulate putting one host into maintenance mode when calculating the number of VMs to be added.

[View Report Example](./reports/How%20Many%20More%20VMs%20Can%20be%20Provisioned.pdf)

Use Case

This report helps administrators to discover how many additional VMs can be deployed without affecting infrastructure performance.


