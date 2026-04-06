---
title: "Troubleshooting Performance of Categorized Objects"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/troubleshoot_bv_objects.html"
last_updated: "8/20/2024"
product_version: "13.0.1.6168"
---

# Troubleshooting Performance of Categorized Objects


Veeam ONE Client includes a set of dashboards that give you enhanced control over categorized virtual infrastructure objects and facilitate the troubleshooting process:

* Top N dashboards display top and bottom resource consumers in a group:

+ To view VMs that consume the greatest amount of compute, network and storage resources, choose the necessary VM group in the inventory pane and go to the Top Objects tab.
+ To view the most loaded hosts, choose the necessary host group in the inventory pane and navigate to Top Objects > Top Hosts.
+ To view the least loaded hosts, choose the necessary host group in the inventory pane and navigate to Top Objects > Bottom Hosts.

For details on the Top and Lowest Load dashboards, see [VMware vSphere Top Objects](vsphere_top_load.md) and [Microsoft Hyper-V Top Objects](hyperv_top_load.md).

* Tasks & Events dashboard shows tasks and events targeted for categorized objects.

To view the list of tasks and events for a categorized virtual infrastructure object, select it in the inventory pane and go to the Tasks & Events tab.

* Processes dashboard provides control over processes and services running inside the guest OS of a VM.

+ For Windows- based machines, you can view, end or restart processes.
+ You can view or end daemons on Linux-based machines.

To view the list of processes, select the necessary VM in the inventory pane and go to the Processes tab.

For details on VM processes, see [VMware vSphere In-Guest Processes](vsphere_processes.md) and [Microsoft Hyper-V In-Guest Processes](hyperv_processes.md).

* Console view allows you to access the VM guest OS right from the Veeam ONE Client interface.

To access a VM console, select the necessary VM in the inventory pane and go to the Console tab.

For details on working with VM console, see [VMware vSphere VM Console](vsphere_console.md) and [Microsoft Hyper-V VM Console](hyperv_console.md).


