---
title: "Idle VMs (vSphere)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/idle_vms_vmware.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Idle VMs (vSphere)


Idle VMs are virtual machines that remain running even though they are no longer used, for example the project or POC is complete — but the VMs were never decommissioned. These Idle VMs consume CPU, memory and storage resources that could be used by other active machines.

This report shows a list of idle VMs in terms of CPU, memory, disk and network utilization.

* The Summary section includes the following elements:

+ The Idle/Active VMs chart shows the number of idle and active VMs.
+ The Wasted Storage, GB chart shows the amount of valuable and wasted storage resources.
+ The Idle CPU, GHz and Idle Memory, GB charts show the amount of active and idle CPU and memory resources.

* The Details table provides information on idle VMs, including cluster or host name, VM name, CPU, memory, disk and network usage, and the number of days during which VM was inactive.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* VMware Cloud Director objects: defines VMware Cloud Director components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Last <N>: defines the time period to analyze in the report. Note that the reporting period must include at least one successfully completed Object properties data collection task for the selected scope. Otherwise, the report will contain no data.
* CPU usage, less than (GHz): defines CPU usage threshold. If the average CPU usage for a VM is below the threshold during certain number of days (defined by Time in the selected state), the VM will be considered to be “Idle”.
* Memory consumed, less than (GB): defines memory usage threshold. If the average memory usage for a VM is below the threshold during certain number of days (defined by Time in the selected state), the VM will be considered to be “Idle”.
* Disk usage, less than (KBps): defines disk usage threshold. If the average disk usage for a VM is below the threshold during certain number of days (defined by Time in the selected state), the VM will be considered to be “Idle”.
* Network usage, less than (KBps): defines network usage threshold. If the average network usage for a VM is below the threshold during certain number of days (defined by Time in the selected state), the VM will be considered to be “Idle”.
* Time spent in the defined conditions (%): defines the percentage of days in the reporting period when the average resource usage (CPU, Memory, Disk and Network) of the VM was below the selected thresholds.

|  |
| --- |
| Note: |
| Veeam ONE Web Client checks whether the CPU usage, Memory consumed, Disk usage and Network usage conditions are true at the same time (in other words, the conditions are joined by “AND”). |

[View Report Example](./reports/Idle%20VMs%20%28vSphere%29.pdf)

Use Case

Idle VMs waste valuable storage resources. Use this report to review performance of your VMs and identify VMs that can be shut down or reconfigured to reclaim additional storage resources.


