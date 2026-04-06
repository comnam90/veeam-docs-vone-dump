---
title: "VMware vSphere Hosts"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vsphere_hosts.html"
last_updated: "3/12/2025"
product_version: "13.0.1.6168"
---

# VMware vSphere Hosts


You can view the list of ESXi hosts in your VMware vSphere infrastructure — on vCenter Server or in a datacenter.

To view the list of hosts:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click Virtual Infrastructure.
2. In the inventory pane, select the necessary infrastructure container.
3. Open the Infrastructure Objects tab and navigate to Hosts.
4. To find the necessary host by name, use the Search field at the top of the list.
5. Click column names to sort hosts by a specific parameter.

For example, to view hosts with the greatest number of VMs, you can sort VMs in the list by VM Count.

[![List of Hosts](images/vmware_hosts_list.webp)](images/vmware_hosts_list.webp "List of Hosts")

For every host in the list, the following details are available:

* Object — name of the host
* Parent Object — name of the parent infrastructure object
* CPU Count — number of CPU cores on the host
* CPU Frequency — frequency of the host CPU core in GHz
* Memory Size — amount of physical memory available on the host
* VM Count — number of VMs that reside on the host

You can choose what columns to show or hide in the Hosts table:

* To hide one or more columns, right-click the table header, and clear check boxes next to the corresponding data fields.
* To make hidden columns visible, right-click the table header, and select check boxes next to the corresponding data fields.


