---
title: "VM Uptime (vSphere)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vms_uptime_vmware.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# VM Uptime (vSphere)


This report analyzes VM uptime statistics to track VM availability.

* The Summary section includes the following elements:

+ The Top Uptime and Lowest Uptime charts display top 5 VMs in terms of the highest and the lowest uptime values.
+ The Uptime Distribution chart displays the number of VMs with different uptime values.

* The Virtual Machine Uptime table provides the full list of VMs whose uptime values are lower and greater than the specified thresholds.

Click a VM name to drill down to detailed information on triggered alarms and virtual machine restart events over a specified reporting period.

|  |
| --- |
| Note: |
| The Number of Restarts column shows the number of VM restarts from the VMware vSphere Client only. |

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Period: defines the time period to analyze in the report. Note that the reporting period must include at least one successfully completed Object properties data collection task for the selected scope. Otherwise, the report will contain no data.

* Business hours only: defines time of a day for which historical performance data will be used to calculate the performance trend. All data beyond this interval will be excluded from the baseline used for data analysis.

* Uptime, greater than: defines the desired minimum uptime value.
* Uptime, less than: defines the desired maximum uptime value.
* Group by: defines how data will be grouped in the report output (by Uptime, Datacenter, Cluster or Host).

[View Report Example](./reports/VM%20Uptime%20%28vSphere%29.pdf)

Use Case

Uptime is a measure of time a VM has been up and actively running on a host. When a VM is not operating, storage space allocated to it is not being used productively. Used this report to track uptime of virtualized workloads.


