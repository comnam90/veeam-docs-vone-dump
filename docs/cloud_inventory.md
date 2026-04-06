---
title: "Cloud Connect Inventory"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/cloud_inventory.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Cloud Connect Inventory


This report provides inventory information on the Veeam Backup & Replication and Veeam Cloud Connect infrastructures.

* The License Information section shows product license details, including the total number of instances consumed by physical computers (workstations and servers) backup, number of instances consumed by cloud backups and replicas, the breakdown of total and used instances for licensed objects, and license expiration date.
* The Rental Licenses section shows number of rental instances consumed by tenants' physical computers (workstations and servers) and VM cloud backup, as well as total and used instances.
* The Veeam B&R Infrastructure section provides information about backup servers, including the version of Veeam Backup & Replication installed, the number and type of backup proxies and backup repositories managed by backup servers.
* The Backup Proxies section provides information about backup proxy servers, including the server type (file proxy or VM proxy), the type of transport mode chosen for proxy servers, the number of maximum allowable concurrent tasks, connected datastores, and shows whether throttling is enabled for these servers.

Veeam Cloud Connect service providers cannot see performance data for proxies used by tenant data protection jobs.

* The Tape Servers section provides information about tape servers and tape libraries connected to the servers, and shows whether throttling is enabled for these servers.
* The Backup Repositories section shows a list of backup repositories and provides additional details including the repository capacity and free space, the amount of space used by full and incremental backups, the number of backup jobs utilizing a repository and the number of VMs and computers residing in backups stored on a repository.
* The Scale-Out Backup Repositories section shows a list of scale-out backup repositories and provides additional details including the repository regular extents and capacity tiers, their capacities and free space, the amount of used space, the number of backup jobs utilizing a repository and the number of VMs and computers residing in backups stored on a repository.
* The WAN Accelerators section provides information about WAN accelerators and their configuration, including a port number, the number of allowed concurrent connections, cache size, the amount of free space in cache, and cache location.

For WAN accelerators used in Veeam Cloud Connect jobs, performance data is available only if the target WAN accelerator is present in the Veeam ONE infrastructure.

* The Cloud Repositories section provides information about cloud repositories including underlying backup repositories, quotas, the amount of free space left, the number of VMs and computers residing in backups stored on the repositories, and quota expiration dates.
* The Cloud Gateway Servers section provides information about configuration of cloud gateways including guest OSes, IP addresses, ports numbers and related gateway pools.
* The Cloud Gateway Pools section provides information about number of gateways in each gateway pool.
* The Hardware Plans section shows the amount of virtual computing, memory and storage resources allocated to a hardware plan and the number of users subscribed to each plan.
* The Clusters/Hosts section provides information about hosts and clusters unitized in cloud hardware plans, their CPU and memory resources, and the number of VM replicas on a host/cluster.
* The Storages section shows total capacity of cloud storage, amount of free space and the number of VM replicas located on each storage.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.

|  |
| --- |
| Note: |
| * Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, Veeam ONE Web Client may show invalid data for Veeam Backup & Replication reports and dashboards. * To analyze data about replicated VMs in the report, you must connect the target virtualization servers to Veeam ONE. For details on, see [Add Data Source](connecting_servers.md). |

[View Report Example](./reports/Cloud%20Connect%20Inventory.pdf)

Use Case

This report displays inventory information for the Veeam Backup & Replication and Veeam Cloud Connect infrastructure components including licensing details.


