---
title: "Microsoft SQL Server"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/sql_server.html"
last_updated: "8/7/2025"
product_version: "13.0.1.6168"
---

# Microsoft SQL Server


For the Veeam ONE database, use a server that meets the following requirements.

Hardware Recommendations

Hardware Recommendations

| Specification | Veeam Backup Data Only | Virtual Infrastructure |
| CPU, RAM | CPU and RAM sizing requirements are the same as for the [Veeam ONE Server](one_server.md).  Note: the Standard Edition of SQL Server does not allow the use of more than 4 CPU sockets (or more than 24 cores in total). If the recommended amount of cores or sockets exceeds these limits, SQL Server Enterprise Edition must be used.  Important! These requirements assume that the Veeam ONE database is hosted on a dedicated Microsoft SQL Server. If the SQL Server is shared by several applications, compute requirements will be higher. To calculate the amount of resources required by other applications, see application-specific sizing recommendations for Microsoft SQL Server. | |
| Disk | Install the OS and Microsoft SQL Server on different drives.  OS Drive: 50 GB  Application drive: Use the [Veeam ONE Database Calculator](https://www.veeam.com/calculators/simple/monitoring/) to size application data. With partitioning scripts, you will have the following distribution of the Veeam ONE database size:   * Primary Tables: 20% * Partitioned Tables: 80%   Size the following tables in accordance with Microsoft SQL Server recommendations:   * Primary Logs * Partitioned Logs * TempDB   Other: SSD RAID storage with broadband connectivity must be used for the TempDB table. | |
| Other | If you use a virtualized Microsoft SQL Server, this server must run on a separate LUN/datastore from Veeam ONE Server. | |

Software and OS Requirements

Software and OS Requirements

| Specification | Requirement |
| Software | Microsoft SQL Server (Full and Express Editions):   * Microsoft SQL Server 2025 * Microsoft SQL Server 2022 * Microsoft SQL Server 2019 * Microsoft SQL Server 2017 (Microsoft SQL Server 2017 Express edition without cumulative updates is included in Veeam ONE installation package) * Microsoft SQL Server 2016 * Microsoft Azure SQL Database * Amazon RDS for SQL Server   Reporting Services (optional):   * Microsoft SQL Server Reporting Services 2025 * Microsoft SQL Server Reporting Services 2022 * Microsoft SQL Server Reporting Services 2019 * Microsoft SQL Server Reporting Services 2017 * Microsoft SQL Server Reporting Services 2016 |

Database Size

To calculate an expected size of the Veeam ONE database, use the Veeam ONE Database Calculator. The calculator helps estimate disk space required to store VMware vSphere, Microsoft Hyper-V and Veeam Backup & Replication data.

For details, see <https://www.veeam.com/kb2246>.


