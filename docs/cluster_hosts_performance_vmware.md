---
title: "Cluster Hosts Performance"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/cluster_hosts_performance_vmware.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Cluster Hosts Performance


This report aggregates historical data and shows performance statistics for all hosts in selected clusters across a time range. The report features a predefined list of performance counters and allows you to report on memory, CPU, disk and network usage.

* For each host in the cluster, the Summary section includes the following elements:

+ The summary table describes configuration of each host in the cluster, including allocated memory and CPU resources and the number of CPU cores and sockets.
+ The resource usage subsections provide information on CPU, memory, disk and network usage and analyzes resource usage trends for each host.

Click a host name in the summary table or in the resource usage table to drill down to performance charts with statistics on CPU, memory, disk and network usage for the host, and the list of top resource consuming VMs. You can click a VM name in the list to drill down to performance charts with statistics on CPU, memory, disk and network usage for the VM.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Period: defines the time period to analyze in the report. Note that the reporting period must include at least one successfully completed Object properties data collection task for the selected scope. Otherwise, the report will contain no data.
* Business hours only: defines time of a day for which historical performance data will be used to calculate the performance trend. All data beyond this interval will be excluded from the baseline used for data analysis.
* Metrics: defines a list of performance counters to analyze in the report.

[View Report Example](./reports/Cluster%20Hosts%20Performance.pdf)

Use Case

The report provides an overview of hardware resource consumption across your hosts. This information may help you identify hosts with performance issues, balance workloads, right-size resource provisioning, redefine DRS settings and optimize cluster overall performance.


