---
title: "VM Performance (vSphere)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/virtual_machine_performance_vmware.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# VM Performance (vSphere)


This report aggregates historical data and shows performance statistics for a selected VM across a time range.

* The Navigation section shows path to the selected object, including VMware vSphere VC, datacenter, cluster and resource pool.

Click a cluster, host or resource pool name to drill down to performance charts with statistics on CPU, memory, disk and network usage.

* The Performance subsections provide information on CPU, memory, disk and network usage and analyzes resource usage trends.

Report Parameters

You can specify the following report parameters:

* Object: defines the VM to analyze in the report.
* Period: defines the time period to analyze in the report. Note that the reporting period must include at least one successfully completed Object properties data collection task for the selected VM. Otherwise, the report will contain no data.
* Business hours only: defines time of a day for which historical performance data will be used to calculate the performance trend. All data beyond this interval will be excluded from the baseline used for data analysis.

[View Report Example](./reports/VM%20Performance%20%28vSphere%29.pdf)

Use Case

The report allows you to verify that you have provided enough resources to the virtual machine.


