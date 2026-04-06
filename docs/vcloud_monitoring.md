---
title: "VMware Cloud Director Monitoring"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vcloud_monitoring.html"
last_updated: "5/12/2025"
product_version: "13.0.1.6168"
---

# VMware Cloud Director Monitoring


Veeam ONE Client offers a comprehensive view for the logical and physical layers of the VMware Cloud Director infrastructure. Veeam ONE collects real-time statistics from connected VMware Cloud Director servers and underlying vCenter Servers to help you track provider capacities, monitor resource usage and identify issues that may potentially result in SLA breaches.

With Veeam ONE Client, you can:

1. Monitor health status of the VMware Cloud Director infrastructure.

Start with the Summary dashboards to check the health status of the VMware Cloud Director infrastructure and supporting VMware vSphere components.

View the latest alarms, track pending blocking tasks and expired leases and review the overall state of vApps and VMs provisioned by Cloud Director tenants.

1. View triggered alarms.

Switch to the Alarms dashboard to see details on issues and problems occurred in the VMware Cloud Director infrastructure. VMware Cloud Director alarms will notify you on increasing resource usage for provider and organization VDCs, expiring vApp runtime and storage leases, blocking tasks left with no response, and the health status of Cloud Director infrastructure components.

1. Work with performance charts.

Drill down to performance charts to diagnose performance problems and identify resource bottlenecks.

Track CPU, memory, disk and network performance for underlying hosts, VMs, VM containers, organizations, organization VDCs and vApps.

1. Monitor Cloud Director capacities and resource usage.

Monitor available, allocated and consumed resources to make sure that VMs and vApps have enough allocated CPU, memory and storage resources, and Cloud Director tenants have enough capacities to run their workloads.

1. Investigate problems from within the guest OS.

View the list of in-guest processes to diagnose problems related to a specific service, module or application within the guest OS.

Prerequisites

Before you start monitoring the VMware Cloud Director environment, make sure you have configured connections to Cloud Director servers from which Veeam ONE will collect data. For details on configuring server connections, see [Connecting VMware Cloud Director Servers](vcloud_server_connect.md).

In This Section

* [VMware Cloud Director Summary Dashboards](vcloud_dashboards.md)
* [VMware Cloud Director Alarms](vcloud_alarms.md)
* [VMware Cloud Director Performance Charts](vcloud_charts.md)
* [VMware Cloud Director Resources](vcloud_resources.md)
* [Tracking Blocking Tasks](vcloud_blocking_tasks.md)
* [Troubleshooting Virtual Machine Performance](troubleshoot_vcloud_vms.md)


