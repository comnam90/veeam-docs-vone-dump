---
title: "Unmapped Datastore LUNs"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/unmapped_datastore_luns.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Unmapped Datastore LUNs


This report provides information about all detected shared datastores that are not mapped to any existing backup proxy. If you are going to use the Direct SAN Access mode, datastore LUNs must be mapped to a proxy server.

* The Summary section provides an overview on the total number of datastores, the number of unmapped datastores, their capacity and the number of VMs on unmapped datastores.
* The Details section displays detailed mapped and unmapped datastore information, such as capacity the amount of free and used space, and the number of stored VMs.

Report Parameters

You can specify the following report parameters:

* Scope: defines a virtual infrastructure level and its sub-components to analyze in the report.

|  |
| --- |
| Note: |
| Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, Veeam ONE Web Client may show invalid data for Veeam Backup & Replication reports and dashboards. |

[View Report Example](./reports/Unmapped%20Datastore%20LUNs.pdf)

Use Case

The Direct SAN Access mode is recommended if the ESXi host uses shared storage. In the Direct SAN mode, proxy servers will not be able to read data from LUNs if they are not mapped. This report allows you to detect datastore LUNs that are not mapped to any proxy server in your backup infrastructure.


