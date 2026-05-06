---
title: "Multiple Organizations vDC Performance"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/organizations_vdc_performance.html"
last_updated: "5/5/2026"
product_version: "13.0.1.6168"
---

# Multiple Organizations vDC Performance


This report aggregates historical data and shows performance statistics for selected organization virtual datacenters across a time range. The report features a predefined list of performance counters and allows you to report on memory, CPU, disk and network usage.

* The Summary table provides an overview on organization datacenters, including allocation model, used CPU, memory and storage allocation and used network count.

Click an organization virtual datacenter name in the summary table or in the resource usage table to drill down to performance charts with statistics on CPU, memory, disk and network usage for the virtual datacenter.

* The Performance subsections show performance charts with resource usage statistics, list top resource consuming vApps and VMs and resource usage trends for them.

Click a vApp name in the list of top resource consuming vApps to drill down to performance charts with statistics on CPU, memory, disk and network usage for the vApp.

Click a VM name in the list of top resource consuming VMs to drill down to performance charts with statistics on CPU, memory, disk and network usage for the VM.

Report Parameters

You can specify the following report parameters:

* VMware Cloud Director objects: defines a list of organization virtual datacenters to analyze in the report.
* Period: defines the time period to analyze in the report.
* Business hours only: defines time of a day for which historical performance data will be used to calculate the performance trend. All data beyond this interval will be excluded from the baseline used for data analysis.
* Metrics: defines a list of performance counters to analyze in the report.
* Top N: defines the maximum number of vApps and VMs to display in the report output.

[![Multiple Organizations vDC Performance Report](images/multiple_organizations_vdc_performance_01.webp)](images/multiple_organizations_vdc_performance_01.webp "Multiple Organizations vDC Performance Report")
[![Multiple Organizations vDC Performance Report](images/multiple_organizations_vdc_performance_02.webp)](images/multiple_organizations_vdc_performance_02.webp "Multiple Organizations vDC Performance Report")

Use Case

The report helps you identify organization virtual datacenters with performance issues, right-size resource provisioning and eliminate potential performance bottlenecks.


