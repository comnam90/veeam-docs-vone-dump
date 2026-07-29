---
title: "Replica Billing"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/replica_billing.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Replica Billing


This report helps you assess storage management costs for the backup infrastructure and tracks the consumption of storage by VM replicas.

The report estimates storage resources required to store replicas. The cost can be calculated based on the price of 1 GB or TB of consumed storage space or on the price of a single VM replica. If there is a datastore or volume that is more expensive than other ones, an administrator can also specify the price adjustment factor (or the multiplier) that characterizes the premium charged for access to the datastore/volume.

* The Details section provides information on each replication job, including the number of replicated up VMs, total amount of gigabytes transferred to the storage and total cost.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a backup infrastructure subset to analyze in the report.
* Replication jobs: defines a list of replication jobs to include in the report.
* Period: defines the interval for which the billing statement is required.
* Price: defines a storage price for accommodating 1 GB/TB of replica files or a price for a VM replica.
* Individual datastore price multipliers: defines the price adjustment factor that characterizes the benefit (and the expense) of using the preferred datastore/volume storage capabilities. The resulting cost is calculated by multiplying the basic rate by the datastore multiplier.

To edit price multipliers:

1. Click Configure.
2. In the Configure Individual Datastore Price Multipliers window, select the target datastore and click Edit.
3. In the Set Individual Datastore Price Multiplier window, specify the desired price adjustment multiplier and click Save.
4. Repeat steps b–c for each datastore price multiplier you want to edit.

* Datastores: defines a list of datastores and volumes that will be analyzed in the report.
* Customer: defines a customer name to be displayed in the report output.

|  |
| --- |
| Note: |
| Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, Veeam ONE Web Client may show invalid data for Veeam Backup & Replication reports and dashboards. |

[View Report Example](./reports/Replica%20Billing.pdf)

Use Case

This report allows managed storage providers (MSP) to generate billing statements for customers and charge them for the used storage.

The report can help administrators to evaluate efficiency of the storage resources utilization.

Page updated 2026-07-22

