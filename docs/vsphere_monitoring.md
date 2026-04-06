---
title: "VMware vSphere Monitoring"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vsphere_monitoring.html"
last_updated: "5/12/2025"
product_version: "13.0.1.6168"
---

# VMware vSphere Monitoring


Veeam ONE Client offers a variety of tools for monitoring the VMware vSphere environment from any perspective and with any level of detail.

With Veeam ONE Client, you can:

1. Monitor health status of the virtual environment.

* Start with the Summary dashboards to check the overall health status of the virtual environment and reveal hotspots.

Quickly review the state of virtual infrastructure components, see the latest alarms, detect the most problematic objects and drill down to the problem source for further investigation.

* Use the Virtual Machines dashboard to view the list of VMs in a virtual infrastructure container and check additional details for every VM — VM current state, parent host, IP address, DNS name and the amount of resources currently consumed by the VM.
* Use the Top Objects dashboard to detect the most and less loaded components in the virtual environment.

Detect what virtual infrastructure objects are consuming the most and the least amount of CPU, memory, disk, network, and swap resources, or select additional counters to detect resource consumers in other areas.

1. View triggered alarms.

Switch to the Alarms dashboard to see details on breached thresholds, events and problems that occurred in the virtual environment.

Use the Actions pane on the alarms dashboard to detect root causes — drill down to performance charts, open VM console or view the list of in-guest processes.

1. Work with performance charts and track events.

Drill down to performance charts to diagnose performance problems. You can change predefined views, quickly switch between charts and view events occurring in your environment to get all-round statistics.

1. Investigate problems from within the guest OS.

Open the VM console or view the list of in-guest processes to diagnose problems related to a specific service, module or application.

Prerequisites

Before you start monitoring your virtual environment, make sure you have configured connections to virtual servers from which Veeam ONE will collect data. For details on configuring server connections, see [Connecting VMware vSphere Servers](vsphere_server_connect.md).

In This Section

* [VMware vSphere Summary Dashboards](vsphere_dashboards.md)
* [VMware vSphere Alarms](vsphere_alarms.md)
* [VMware vSphere Performance Charts](vsphere_charts.md)
* [VMware vSphere Tasks & Events](vsphere_events.md)
* [VMware vSphere Virtual Machines](vsphere_vms.md)
* [VMware vSphere Hosts](vsphere_hosts.md)
* [VMware vSphere Datastores](vsphere_datastores.md)
* [VMware vSphere Top Objects](vsphere_top_load.md)
* [Host Hardware State](vsphere_host_hardware_state.md)
* [VMware Remote Console (VMRC)](vsphere_console.md)
* [VMware vSphere In-Guest Processes](vsphere_processes.md)
* [VMware vSphere In-Guest Services](vsphere_services.md)
* [Launching vSphere Client](vsphere_client.md)


