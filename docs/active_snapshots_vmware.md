---
title: "Active Snapshots"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/active_snapshots_vmware.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Active Snapshots


This report shows a list of all VMs with snapshots, including the oldest and the largest snapshots in the virtual environment.

* The Top VMs by Active Snapshot Size (GB) and Top VMs by Active Snapshot Age (Weeks) charts display top 5 VMs with the oldest and the largest snapshots in the virtual environment.

* The Details table provides the list of VMs with snapshots and shows snapshot name, its location, date and time when the snapshot was created, snapshot size and state of the VM.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* VMware Cloud Director objects: defines VMware Cloud Director components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Snapshot age, older than: defines snapshot age threshold. If a VM snapshot is older than the specified age, the VM will be included in the report.
* Ignore replica VMs created by Veeam products: defines whether to include VM replicas created by Veeam Backup & Replication in the report.

Veeam Backup & Replication uses VM snapshots as replica restore points. Such snapshot restore points may be large in size and remain on the datastore for a long period of time. If you have VM replicas created with Veeam Backup & Replication, select this check box to exclude VM replicas with snapshot restore points from the report.

|  |
| --- |
| Note: |
| If you run the Active Snapshots report with Veeam backup data and large-scale virtual infrastructure performance monitoring mode selected, the snapshot size data may be incorrect or absent. For more information on data collection modes, see [Scalability](utility_deployment.md) and [Choose Data Collection Mode](typical_choose_collection_mode.md). |

[View Report Example](./reports/Active%20Snapshots.pdf)

Use Case

Outdated snapshots consume valuable storage resources. Best practices for snapshots recommend that you delete snapshots older than 3 days, since they no longer reflect recent VM changes.

The report helps you detect outdated snapshots and better address the problem of wasted storage space.


