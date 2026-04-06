---
title: "VMware vSphere Performance Charts"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vsphere_charts.html"
last_updated: "4/30/2025"
product_version: "13.0.1.6168"
---

# VMware vSphere Performance Charts


Performance charts show how key performance counters have been changing over time to help you diagnose performance issues and perform root cause analysis.

|  |
| --- |
| Note |
| Performance statistics for VMs are gathered and displayed from the VMware vSphere environment and not from within the Guest OS. This is because the guest OS is unaware of the hypervisor's resource allocations and cannot recognize when the hypervisor temporarily de-schedules VM resources during periods of inactivity. |

Performance charts include the following elements:

* Axes

Performance charts display data for a particular time period (the horizontal axis) using two scales of measurement units (vertical axes). The measurement units may vary depending on selected performance counters. However, the number of units is always limited to two.

* Graphs

Performance charts include one or more graphs. Every graph on a performance chart visualizes a specific counter for an infrastructure object or a container of infrastructure objects.

* Legend

The chart legend shows details about objects and counters displayed in the chart. The details include key color, object name, list of counters and units of measurement, the latest, minimum, average, and maximum counter values.

* Chart views

Performance charts come with a number of predefined chart views. Every view logically groups related counters to display the most valuable data and help you speed up troubleshooting and root cause analysis of performance problems.

Performance charts can be easily customized. For details on customization options, see [Customizing VMware vSphere Performance Charts](customize_vsphere_charts.md).

Accessing Performance Charts

To access a performance chart for an infrastructure object or infrastructure segment:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click Virtual Infrastructure.
2. In the inventory pane, select the necessary infrastructure object or segment.
3. Open the Performance tab.

[![Virtual Infrastructure Performance Charts](images/vmware_performance_chart.webp)](images/vmware_performance_chart.webp "Virtual Infrastructure Performance Charts")

In This Section

* [Overview](vsphere_overall.md)
* [CPU Performance Chart](vsphere_cpu.md)
* [Memory Performance Chart](vsphere_memory.md)
* [Network Performance Chart](vsphere_network.md)
* [Datastore Performance Chart](vsphere_datastore.md)
* [Virtual Disks Performance Chart](vsphere_virtual_disk.md)
* [Storage Path Performance Chart](vsphere_storage_path.md)
* [Storage Adapter Performance Chart](vsphere_storage_adapter.md)
* [Disk Space Chart](vsphere_disk_space.md)
* [Disk I/O Chart](vsphere_disk_io.md)
* [Disk Issues Chart](vsphere_disk_issues.md)
* [Customizing VMware vSphere Performance Charts](customize_vsphere_charts.md)


