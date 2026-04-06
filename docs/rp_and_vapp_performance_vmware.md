---
title: "Resource Pool and vApp Performance"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/rp_and_vapp_performance_vmware.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Resource Pool and vApp Performance


This report aggregates historical data and shows performance statistics for a selected resource pool/vApp across a time range.

The report shows tables and performance charts with statistics on CPU, memory, disk and network usage for the resource pool/vApp. The report also lists top resource consuming VMs and calculates resource usage trends for them.

* The Navigation section shows path to the selected object, including VMware vSphere VC, datacenter, cluster and resource pool.

Click a cluster name to drill down to performance charts with statistics on CPU, memory, disk and network usage for the cluster.

* The Performance subsections provide information on CPU, memory, disk and network usage, including usage trends and top resource consuming VMs.

Click a VM name in the list of top resource consuming VMs to drill down to performance charts with statistics on CPU, memory, disk and network usage for the VM.

Report Parameters

You can specify the following report parameters:

* Object: defines the resource pool or vApp to analyze in the report.
* Period: defines the time period to analyze in the report. Note that the reporting period must include at least one successfully completed Object properties data collection task for the selected resource pool/vApp. Otherwise, the report will contain no data.
* Business hours only: defines time of a day for which historical performance data will be used to calculate the performance trend. All data beyond this interval will be excluded from the baseline used for data analysis.
* Top N: defines the maximum number of VMs to display in the report output.

[View Report Example](./reports/Resource%20Pool%20and%20vApp%20Performance.pdf)

Use Case

The report helps you identify resource pools and vApps with performance issues, evaluate how efficiently your resource pools and vApps are performing, and decide whether additional right-sizing or reconfiguration actions are necessary.


