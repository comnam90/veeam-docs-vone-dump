---
title: "Viewing License Information"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/view_license_information.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Viewing License Information


You can view the details and current usage of your Veeam ONE license on the License Information page in Veeam ONE Web Client.

To view license information:

1. Open Veeam ONE Web Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the top right corner of the Veeam ONE Web Client window, click Configuration.
2. In the configuration menu on the left, click License Information.

The License Information page opens on the License tab.

[![View License Details](images/view_license_details.webp)](images/view_license_details.webp "View License Details")

License Details

The License tab shows general information about the installed Veeam ONE license:

* Status — the status of the installed license, such as Valid, Expired (N days of grace period remaining), Warning (License exceeded) or Not Installed.
* Type — the license type: Perpetual, Subscription, Rental, Community, Evaluation or NFR.
* Package — the license package, such as ONE, Essentials or Suite.
* Support ID — the customer identification number required when you contact Veeam Technical Support.
* Licensed to — the name of the company or user the license was issued to.
* Instances, Points or Sockets (depending on the license type) — the number of licensed units and the number currently used.
* Expiration date — the date when the license expires and the number of days remaining.
* [For Perpetual licenses] Support expiration date — the date when product support expires.

License Usage

The Instances, Points or Sockets tab (depending on your license type) shows how license units are consumed, broken down by workload type. The tab contains the following columns:

* Type — the workload or object type.
* Count — the number of objects of the given type.
* Multiplier — the multiplier applied to the object count to calculate consumption.
* Instances or Points — the number of instances or points the type consumes.

For a per-socket license, the Sockets tab shows the total number of licensed, used and remaining sockets rather than a per-workload breakdown.

The following workload types can consume license units:

* VMs — the number of managed VMs out of the total discovered on managed VMware vSphere and Microsoft Hyper-V hosts and Veeam Backup & Replication servers.
* Servers — the number of Veeam Agents that run in Server mode and are managed by Veeam Backup & Replication servers connected to Veeam ONE.
* Workstations — the number of Veeam Agents that run in Workstation mode and are managed by Veeam Backup & Replication servers connected to Veeam ONE.
* File Shares — the number of managed data blocks (500 GB each) of file shares protected by Veeam Backup & Replication servers connected to Veeam ONE.
* Cloud VMs — the number of Microsoft Azure VMs, Google Cloud VMs and AWS EC2 instances protected by cloud backup products integrated with Veeam Backup & Replication servers connected to Veeam ONE.
* Cloud File Shares — the number of AWS EFS and Microsoft Azure file shares protected by cloud backup products integrated with Veeam Backup & Replication servers connected to Veeam ONE.
* Cloud Databases — the number of Microsoft Azure SQL, AWS RDS and Google Cloud SQL databases protected by cloud backup products integrated with Veeam Backup & Replication servers connected to Veeam ONE.
* Applications — the number of enterprise applications protected with Veeam plug-ins for SAP HANA, Oracle RMAN, SAP on Oracle and SAP on MaxDB.
* Object Storage — the number of managed data blocks (500 GB each) of Amazon S3, Azure Blob and S3 compatible storage data protected by Veeam Backup & Replication servers connected to Veeam ONE.
* [For Rental licenses] Microsoft 365 users — the number of users protected by Veeam Backup for Microsoft 365 servers connected to Veeam ONE.

To view the individual workloads counted for a type, click the type in the Type column. The Licensed Workloads window lists each workload by Name and Host. To save the list to a CSV file, click Export to CSV.

![Viewing License Information](images/license_usage_sockets.webp)[![License Usage Details](images/license_usage_instances.webp)](images/license_usage_instances.webp "License Usage Details")

Page updated 2026-07-24

