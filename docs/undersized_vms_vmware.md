---
title: "Undersized VMs (vSphere)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/undersized_vms_vmware.html"
last_updated: "9/10/2025"
product_version: "13.0.1.6168"
---

# Undersized VMs (vSphere)


This report helps you detect virtual machines that have less allocated vRAM or vCPU resources than they require. The report analyzes historical performance and configured resource allocation to provide recommendations for an optimized VM configuration and allocation of resources.

* The Summary section provides an overview of the current state of your infrastructure, including the total number of VMs and the number of CPU and memory undersized VMs, and shows recommendations on resource allocation.

* The Undersized Virtual Machines by CPU and Undersized Virtual Machines by Memory tables display VMs with insufficient CPU and memory resources and deliver recommendations for their reconfiguration.

Click a VM name in the Virtual Machine column to drill down to VM performance charts that show how CPU and memory usage has been changing within the reporting period.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* VMware Cloud Director objects: defines VMware Cloud Director components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Last <N>: defines the time period to analyze in the report. Note that the reporting period must include at least one successfully completed Object properties data collection task for the selected scope. Otherwise, the report will contain no data.
* Business hours only: defines time of a day for which historical performance data will be used to calculate the performance trend. All data beyond this interval will be excluded from the baseline used for data analysis.
* CPU ready, more than (%): defines the threshold for the percentage of time during which CPU resources were in the ready state. If the CPU Ready Time value for a VM exceeds the specified threshold, the VM will be included in the report.
* Swap out rate, more than (KBps): defines the threshold for the percentage of the time which a VM spent waiting for memory to be swapped back in from disk. If the Swap Wait Time value for a VM exceeds the specified threshold, the VM will be included in the report.
* CPU utilization (%): defines the CPU utilization threshold. If the CPU usage value for a VM exceeds the specified threshold, the VM will be included in the report.
* Memory utilization (%): defines the memory utilization threshold. If the memory usage value for a VM exceeds the specified threshold, the VM will be included in the report.
* Memory counter type: defines whether the Memory Active or Memory Consumed performance metric should be analyzed in the report.

|  |
| --- |
| Note: |
| Veeam ONE Web Client checks whether the CPU ready and CPU Usage conditions are true at the same time, and then whether Swap out rate and Memory Usage conditions are true at the same time (in other words, the conditions in each pair are joined by Boolean “AND”).  Then Veeam ONE Web Client checks whether a pair of these conditions is true, in other words, pairs of these conditions are joined by Boolean “OR”. |

[![Undersized VMs Report](images/vmware_undersized_vms_01.webp)](images/vmware_undersized_vms_01.webp "Undersized VMs Report")

Use Case

This report provides practical recommendations for restoring performance of VMs that have less resources than they need. You may consider adding the specified amount of resources for the VM, relocating the VM to a more powerful host, or committing increased resources to a resource pool shared by the undersized VM.


