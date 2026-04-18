---
title: "Garbage Files"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/garbage_files_vmware.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Garbage Files


This report shows an overview of storage consumed by files that do not belong to VMs comprised in the infrastructure inventory.

* The Summary chart displays total amount of free space, amount of space consumed by non-garbage files and amount of space consumed by garbage files on datastores from the selected scope (in percentage).
* The Details table shows the full list of datastores with folders that contain garbage files.

Click a folder name in the details table to drill down to the list of garbage files in the folder.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Storage type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

|  |
| --- |
| Note: |
| * You can exclude specific datastores from this report. This can be useful when you are not interested in examining particular datastores for garbage files (for example, local datastores, datastores hosting ISO files or backups). In this case, you can exclude unnecessary datastores from the collection scope. For more information, see [Choosing Datastores to Report On](datastores_to_report.md). * If you run the Garbage Files report with Veeam backup data and large-scale virtual infrastructure performance monitoring mode selected, no data will display in the report. For more information on data collection modes, see [Scalability](utility_deployment.md) and [Choose Data Collection Mode](typical_choose_collection_mode.md). |

[View Report Example](./reports/Garbage%20Files.pdf)

Use Case

If a VM was improperly deleted or relocated, or if a snapshot operation failed, some residual elements belonging to the VM may remain on the datastore.

This report allows you to check your infrastructure for garbage files that waste storage space and impact ROI.


