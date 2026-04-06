---
title: "Multiple Clusters Performance"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/multiple_clusters_performance_vmware.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Multiple Clusters Performance


This report aggregates historical data and shows performance statistics for selected clusters across a time range. The report features a predefined list of performance counters and allows you to report on memory, CPU, disk and network usage.

* The Summary section describes configuration of each selected cluster, including allocated memory and CPU resources, the number of CPU cores and sockets and CPU and memory usage rates.

Click a cluster name to drill down to performance charts with statistics on CPU, memory, disk and network usage for the cluster.

* The Performance subsections provide information on CPU, memory, disk and network usage, including usage trends and top resource consuming hosts and VMs in the cluster.

Click a host name in the list of top resource consuming hosts to drill down to performance charts with statistics on CPU, memory, disk and network usage for the host.

Click a VM name in the list of top resource consuming VMs to drill down to performance charts with statistics on CPU, memory, disk and network usage for the VM.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Period: defines the time period to analyze in the report. Note that the reporting period must include at least one successfully completed Object properties data collection task for the selected scope. Otherwise, the report will contain no data.
* Business hours only: defines time of a day for which historical performance data will be used to calculate the performance trend. All data beyond this interval will be excluded from the baseline used for data analysis.
* Top N: defines the maximum number of hosts and VMs to display in the report output.
* Metrics: defines a list of performance counters to analyze in the report.

[View Report Example](./reports/Multiple%20Clusters%20Performance.pdf)

Use Case

The report provides an overview of hardware resource consumption across your clusters. This information may help you identify clusters with performance issues, balance workloads, right-size resource provisioning, redefine DRS settings and optimize cluster overall performance.


