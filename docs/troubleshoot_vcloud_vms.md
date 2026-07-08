---
title: "Troubleshooting Virtual Machine Performance"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/troubleshoot_vcloud_vms.html"
last_updated: "7/8/2026"
product_version: "13.0.2.6723"
---

# Troubleshooting Virtual Machine Performance


Veeam ONE Client includes a set of dashboards that give you enhanced control over VMs provisioned in the VMware Cloud Director environment, and help you facilitate the troubleshooting process:

* Top VMs dashboard displays the top resource consumers for CPU, memory, datastore, network usage, snapshot size and snapshot age.

To view VMs that consume the greatest amount of compute, network and storage resources, select the necessary VM container in the inventory pane and go to the Top VMs tab. For more information, see [VMware vSphere Top and Lowest Load](vsphere_top_load.md).

* Tasks & Events dashboard shows VMware vSphere tasks and events targeted at a specific VM.

To view the list of tasks and events for a VM, select it in the inventory pane and go to the Tasks & Events tab. For more information, see [VMware vSphere Tasks & Events](vsphere_events.md).

* Processes dashboard provides control over processes currently running inside the guest OS of a VM. You can view, end and restart processes on Windows- based machines. You can also view and end daemons on Linux-based machines.

To view the list of processes, select the necessary VM in the inventory pane and go to the Processes tab. For more information, see [VMware vSphere In-Guest Processes](vsphere_processes.md).

* Services dashboard provides control over services currently running inside the guest OS of a VM. You can view, start, stop and restart services on VMs. For Windows-based machines, you can also create alarms based on the service state or object performance.

To view the list of processes, select the necessary VM in the inventory pane and go to the Services tab. For more information, see [VMware vSphere In-Guest Services](vsphere_services.md).

* Console dashboard lists running in-guest processes and helps you diagnose problems related to a specific service, module or application.

To access a VM console, select the necessary VM in the inventory pane and go to the Console tab. For more information, see [VMware vSphere VM Console](vsphere_console.md).


