---
title: "Veeam Backup & Replication Performance Charts"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_charts.html"
last_updated: "3/12/2025"
product_version: "13.0.1.6168"
---

# Veeam Backup & Replication Performance Charts


To identify performance bottlenecks within the backup data flow, you can drill down to the following performance charts:

* [CPU Performance Chart](backup_cpu.md)
* [Memory Performance Chart](backup_memory.md)
* [Disk Performance Chart](backup_disk.md)
* [Network Performance Chart](backup_network.md)
* [Cache Performance Chart](cdp_cache_chart.md)

To draw the charts, Veeam ONE gathers Windows Performance Monitor metrics from the guest OS of backup infrastructure components (for this reason, performance charts for Linux-based repositories are not available). You can track performance metrics for physical and virtual backup servers, proxies, repositories, WAN accelerators or Enterprise Manager servers.

To drill down to a performance chart for a backup infrastructure component:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click Veeam Backup & Replication.
2. Select the necessary backup infrastructure component.
3. Open the necessary performance chart tab.

For performance charts in the Veeam Backup & Replication, you can change chart views and set time intervals, define objects to show on charts or select custom metrics.


