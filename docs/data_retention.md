---
title: "Data Retention"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/data_retention.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Data Retention


Data collected from virtual and backup servers is organized to the Veeam ONE database. Veeam ONE retains data in the database as follows:

* For categorization data, Veeam ONE retains one sample in the database. This data is updated with every new data collection.
* For topology, configuration, audit and performance data, Veeam ONE keeps multiple samples based on the retention policy. Performance data is aggregated in the database according to the scheme described below.
* For events collected from backup and virtual servers, Veeam ONE keeps all collected instances.

Performance Data Aggregation

As the performance data ages, Veeam ONE aggregates it for long-term storage. Data aggregation helps save disk space on the database server and speed up generation of performance reports and charts.

Veeam ONE uses the following aggregation scheme for performance data:

Performance Data Aggregation

| Period | Optimized for Veeam backup data and virtual infrastructure performance monitoring | Optimized for Veeam backup data and large-scale virtual infrastructure performance monitoring | Veeam Backup Data Only |
| Hour | 20 seconds for VMware vSphere 30 seconds for Microsoft Hyper-V | 15 minutes | 20 seconds |
| Week | 5 minutes | 30 minutes | 5 minutes |
| Year | 2 hours | 2 hours | 2 hours |

Sampling intervals at which data is stored to the database depend on Veeam ONE data collection mode. For example, for the Veeam backup data only mode, raw data (data with 20-second resolution) is stored for 1 hour. After 1 hour, raw data is aggregated to 5-minute resolution data. After 1 week, data with 5-minute resolution is aggregated to 2-hour resolution data. Data with this level of detail is stored in the database for up to 1 year.

To draw performance charts, Veeam ONE uses data with various aggregation levels, depending on the period for which performance data is shown. For example, for Veeam backup data only mode, performance charts for the past hour use samples with 20-second resolution, charts for the past day use data with 5-minute resolution and so on.

To generate performance reports, Veeam ONE uses data with 2-hour resolution.

If you use Veeam ONE for monitoring and reporting in large environments, the Veeam ONE database can grow quickly. To support large virtual and backup infrastructures and reduce the size of the Veeam ONE database, you can increase aggregation intervals for performance data. To learn how to change aggregation intervals, contact Veeam Support at <https://www.veeam.com/support.html>.

Page updated 2026-08-03

