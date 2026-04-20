---
title: "Backup Inventory"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_inventory.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Backup Inventory


This report provides inventory information on configuration of your Veeam Backup & Replication infrastructure.

* The License Information section shows product license details. The Installed Licenses subsection includes the license type, the number of licensed and used sockets and instances, support expiration and license expiration dates, the overall and used capacity. The Instances Usage subsection shows groups of managed objects, number of objects in each group, and number of instances consumed by each group.
* The Veeam B&R Infrastructure section provides information about backup servers, including the version of Veeam Backup & Replication installed, the number and type of backup proxies and backup repositories managed by backup servers.
* The Backup Proxies section provides information about backup proxy servers, including the type of transport mode chosen for proxy servers, the number of maximum allowable concurrent tasks, connected datastores, and shows whether throttling is enabled for these servers.

Veeam Cloud Connect service providers cannot see performance data for proxies used by tenant data protection jobs.

* The Veeam Plugins for Enterprise Applications section provides information about protected data on enterprise databases, including version, type and number of objects.
* The Tape Servers section provides information about tape servers and tape libraries connected to the servers, and shows whether throttling is enabled for these servers.
* The Backup Repositories section shows a list of backup repositories and provides additional details including the repository capacity and free space, the amount of space used by full and incremental backups, the number of backup jobs utilizing a repository and the number of workloads residing in backups stored on a repository.
* The Scale-Out Backup Repositories section shows a list of scale-out backup repositories and provides additional details including the repository regular extents and capacity tiers, their capacities and free space, the amount of used space, the number of backup jobs utilizing a repository and the number of workloads residing in backups stored on a repository.
* The WAN Accelerators section provides information about WAN accelerators and their configuration, including a port number, the number of allowed concurrent connections, cache size, the amount of free space in cache, and cache location.

For WAN accelerators used in Veeam Cloud Connect jobs, performance data is available only if the target WAN accelerator is present in the Veeam ONE infrastructure.

* The Cloud Repositories section provides information about cloud repositories available for cloud tenants, including physical repositories on which cloud storage is allocated, storage quota, free space remaining on the repositories, the number of workloads residing in backups stored on a repository, repository expiration date.
* The Cloud Gateway Servers section provides information about cloud gateways configured on Veeam Cloud Connect servers, including OS of a machine that performs the role of a cloud gateway, IP address or DNS name of this machine, a port that a cloud gateway uses to transport data, and related gateway pools.
* The Cloud Gateway Pools section provides information about number of gateways in each gateway pool.

* The Jobs section displays all backup jobs, their types and the number of workloads in each job.

|  |
| --- |
| Note: |
| Veeam ONE displays file backup copy jobs together with other backup copy jobs. |

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.

[View Report Example](./reports/Backup%20Inventory.pdf)

Use Case

This report displays information on the state of backup infrastructure components and provides product licensing details.


