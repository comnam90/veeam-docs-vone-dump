---
title: "Disk Issues Chart"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vsphere_disk_issues.html"
last_updated: "6/24/2026"
product_version: "13.0.2.6723"
---

# Disk Issues Chart


The Disk Issues chart displays historical statistics on the number of disk bus resets and disk command aborts that have occurred in the defined interval. This chart is available for datastores and datastore clusters.

[![Disk Issues Chart](images/vmware_disk_issues_performance_chart.webp)](images/vmware_disk_issues_performance_chart.webp "Disk Issues Chart")

The following table provides information on predefined views and counters.

Disk Issues Chart

| Chart View | Measurement Unit | Counter | Description |
| Datastore Issues | Disk/ESXi: Datastore Bus Resets | Number | Number of aborted SCSI commands. |
| Disk/ESXi: Datastore Command Aborts | Number | Number of SCSI bus reset commands. |


