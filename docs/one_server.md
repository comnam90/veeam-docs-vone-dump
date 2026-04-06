---
title: "Veeam ONE Server"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/one_server.html"
last_updated: "3/6/2026"
product_version: "13.0.1.6168"
---

# Veeam ONE Server


For the Veeam ONE Server component, use a server that meets the following requirements.

Hardware Recommendations

Hardware Recommendations

| Specification | Veeam Backup Data Only[1](#1) | Virtual Infrastructure |
| CPU | The amount of required CPU resources depends on the number of workloads being protected in the managed infrastructure:   * 2–4 vCPUs for 1,000–10,000 protected workloads * 4–6 vCPUs for 10,000–20,000 protected workloads * 6–8 vCPUs for 20,000–40,000 protected workloads * 8–10 vCPUs for 40,000–60,000 protected workloads   Regardless of the number of protected workloads:   * For every connected Veeam Backup for Microsoft 365 server, additional 1 vCPU core is required. * For every connected Veeam Backup & Replication server, additional 0.03 vCPU core is required. | The amount of required CPU resources depends on the number of hosts in the managed infrastructure:   * 4 vCPUs for up to 1,500 VMs * 4–12 vCPUs for 1,500–10,000 VMs * 12–16 vCPUs for 10,000–20,000 VMs * 16+ vCPUs for 20,000+ VMs |
| RAM | The amount of required memory resources depends on the number of workloads being protected in the managed infrastructure:   * 4 GB for up to 1,000 protected workloads * 4–15 GB for 1,000–10,000 protected workloads * 15–30 GB for 10,000–20,000 protected workloads * 30–50 GB for 20,000-40,000 protected workloads * 50–80 GB for 40,000 - 60,000 protected workloads   Regardless of the number of protected workloads:   * For every connected Veeam Backup for Microsoft 365 server, additional 500 MB RAM is required.2 * For every connected Veeam Backup & Replication server, additional 60 MB RAM is required. | 50 MB per 15 managed VMware VMs and 600 MB per managed vCenter Server.  Note: This requirement assumes that there are no standalone hosts in the managed infrastructure. All hosts must be included in clusters, and clusters must be managed by vCenter Server/SCVMM. Such configuration results in fewer connections to virtual servers during data collection, and requires less memory resources.  In environments with standalone hosts connected to Veeam ONE directly, memory requirements will be higher. |
| Disk | 50 GB recommended space for Veeam ONE cache and Veeam Intelligent Diagnostics logs. | |
| Bandwidth | 1 Mbit/sec for 100 hosts | |

1Under the condition that a protected workload is included in one data protection job scheduled to run daily, that is, has one restore point per day. For example, if a workload is included in two data protection jobs, consider it as two protected workloads, as it will consume twice as much computing resources.

2Individual protected workloads for Veeam Backup for Microsoft 365 include User, Group, Site and Teams.

Software and OS Requirements

Software and OS Requirements

| Specification | Requirement |
| OS | Only 64-bit versions of the following operating systems are supported:   * Microsoft Windows Server 2025 * Microsoft Windows Server 2022 * Microsoft Windows Server 2019 * Microsoft Windows Server 2016 * Microsoft Windows 11 (Professional and Enterprise editions with minimum supported version 22H2) * Microsoft Windows 10 version 1909 and LTS builds (Minimum supported version 21H2 for LTSC channel and 22H2 for GA)   Note: Semi-Annual Channel (SAC) releases are supported. |
| Software | The following components are included in the Veeam ONE setup package and can be installed automatically:   * Microsoft ASP.NET Core Shared Framework 8.0.17 * Microsoft Windows Desktop Runtime 8.0.17 * Microsoft .NET Runtime 8.0.17 * Microsoft .NET Framework 4.7.2  * Microsoft System CLR Types for SQL Server 2014 * Microsoft SQL Server 2014 Management Objects * Microsoft Internet Information Services (IIS) 10.0 or later * Microsoft Application Request Routing 3.0 * IIS URL Rewrite Model 2.1 * Microsoft Universal C Runtime   To connect SCVMM servers to Veeam ONE, the following software is required:   * System Center 2025 Virtual Machine Manager console (for connecting SCVMM 2025 servers) * System Center 2022 Virtual Machine Manager console (for connecting SCVMM 2022 servers) * System Center 2019 Virtual Machine Manager console (for connecting SCVMM 2019 servers) * System Center 2016 Virtual Machine Manager console (for connecting SCVMM 2016 servers) * Microsoft PowerShell 3.0 (required for SCVMM 2016, and SCVMM 2019 consoles)   Be sure to install the same versions of the Admin UI and the SCVMM Server, and to update both components to the same update version. |
| Other | * Windows Management Instrumentation service must be enabled to allow data collection from Veeam Backup & Replication servers. * File and Print Sharing service must be enabled to enable remote Veeam ONE Client connections to the Veeam ONE service. |


