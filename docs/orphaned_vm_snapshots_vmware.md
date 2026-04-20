---
title: "Orphaned VM Snapshots"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/orphaned_vm_snapshots_vmware.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Orphaned VM Snapshots


This report detects VM snapshots that reside on datastores but do not show up in the VMware Snapshot Manager.

* The Datastore Space Usage (GB) chart displays the total amount of free space, amount of space consumed by files other than orphaned snapshots and amount of space consumed by orphaned snapshots on datastores from the selected scope.
* The Details table provides the full list of datastores with folders that contain orphaned snapshots.

The red color bar in the Snapshot: File name column shows how much datastore space is used by each folder with orphaned snapshots.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Datastores: defines datastores to analyze for the presence of orphaned snapshots.

|  |
| --- |
| Note: |
| If you run the Orphaned VM Snapshots report with Veeam backup data and large-scale virtual infrastructure performance monitoring mode selected, no data will display in the report. For more information on data collection modes, see [Scalability](utility_deployment.md) and [Choose Data Collection Mode](typical_choose_collection_mode.md). |

[View Report Example](./reports/Orphaned%20VM%20Snapshots.pdf)

Use Case

Orphaned snapshots consume valuable storage resources. Use this report to discover locations of useless snapshots that can be deleted to reclaim additional storage space.


