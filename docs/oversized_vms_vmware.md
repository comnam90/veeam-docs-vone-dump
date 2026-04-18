---
title: "Oversized VMs (vSphere)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/oversized_vms_vmware.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Oversized VMs (vSphere)


This report helps you to detect VMs that have more allocated vRAM or vCPU resources than they require. The report analyzes historical performance and configured resource allocation to provide recommendations for an optimized VM configuration and allocation of resources.

* The Summary section provides details on the total number of VMs, number of oversized VMs by vCPU and vRAM, and amount of vCPU and vRAM resources that can be reclaimed.

* The Oversized Virtual Machines by CPU table provides a list of VMs from which you can reclaim vCPU resources. For each VM, the table details the number of configured vCPUs, average and peak CPU usage, and provides recommendations on vCPU configuration.

Click a VM name to drill down to VM performance charts that show how CPU usage was changing during the reporting period.

* The Oversized Virtual Machines by Memory table provides a list of VMs from which you can reclaim vRAM resources. For each VM, the table details the amount of allocated memory, average and peak memory usage, and provides recommendations on memory configuration.

Click a VM name to drill down to VM performance charts that show how memory usage was changing during the reporting period.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* VMware Cloud Director objects: defines VMware Cloud Director components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Last <N>: defines the time period to analyze in the report. Note that the reporting period must include at least one successfully completed Object properties data collection task for the selected scope. Otherwise, the report will contain no data.
* Business hours only: defines time of a day for which historical performance data will be used to calculate the performance trend. All data beyond this interval will be excluded from the baseline used for data analysis.
* Memory counter type: defines whether the Memory Active or Memory Consumed performance metric should be analyzed in the report.
* Top N: defines the maximum number of VMs to display in the report output.

[View Report Example](./reports/Oversized%20VMs%20%28vSphere%29.pdf)

Use Case

This report helps you discover VMs with excessive hardware provisioning. You may consider decreasing hardware provisioning for the VM in vSphere configuration options, relocating the VM to less powerful hosts, or adding more VMs to a shared resource pool to optimize resource allocation and reclaim wasted resources.


