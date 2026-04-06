---
title: "VMware Cloud Director Performance Charts"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vcloud_charts.html"
last_updated: "12/17/2024"
product_version: "13.0.1.6168"
---

# VMware Cloud Director Performance Charts


To facilitate the troubleshooting process and quickly identify resource bottlenecks, you can drill down to performance charts right from the VMware Cloud Director view:

* [Overview](vsphere_overall.md)
* [CPU Performance Chart](vsphere_cpu.md)
* [Memory Performance Chart](vsphere_memory.md)
* [Datastore Performance Chart](vsphere_datastore.md)
* [Network Performance Chart](vsphere_network.md)
* [Virtual Disks Performance Chart](vsphere_virtual_disk.md)

You can track performance metrics for separate VMs within an organization, for a VM container (such as vApp, organization or organization VDC) and for hosts that support provider VDCs.

To drill down to a performance chart from the VMware Cloud Director view, do one of the following:

* In the VMware Cloud Director inventory, select an infrastructure object (VM or VM container) and go to the necessary performance chart tab in the information pane.
* Open the Alarms dashboard. In the list of alarms, select an alarm for the necessary VM or host. Click Performance in the Actions pane on the right and choose the required performance chart.
* Open the Alarms dashboard. In the list of alarms, select an alarm for the necessary VM or host. Right-click the alarm, choose Performance and select necessary performance chart from the shortcut menu.

|  |
| --- |
| Note: |
| When you open a performance chart for a host, Veeam ONE Client automatically switches to the Virtual Infrastructure. |

For performance charts in the VMware Cloud Director view, Veeam ONE supports a similar set of actions as for virtual infrastructure performance charts: you can change chart views and set time intervals, define objects to show on charts or select custom metrics. For details on customizing performance charts, see [Customizing VMware vSphere Performance Charts](customize_vsphere_charts.md).


