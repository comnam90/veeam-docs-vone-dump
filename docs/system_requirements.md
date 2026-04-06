---
title: "System Requirements"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/system_requirements.html"
last_updated: "3/26/2026"
product_version: "13.0.1.6168"
---

# System Requirements


Before you deploy Veeam ONE, make sure that your environment meets the necessary system requirements.

All-in-One Deployment

If you plan to use the all-in-one deployment scenario, the machine on which you plan to deploy Veeam ONE must meet the following hardware requirements:

* CPU: x86-x64 processor, 4 cores minimum\*
* Memory: 8 GB RAM minimum, 16 GB RAM recommended. Using modern high clock speed memory (DDR3 and higher) and an independent database server improves data processing performance.\*
* Hard Disk Space: 50 GB for product operation and sufficient disk space for Microsoft SQL Server and Veeam ONE database. Use the [Veeam ONE Database Calculator](https://www.veeam.com/kb2246) to size application data.

\*Regardless of the number of protected workloads, for every connected Veeam Backup & Replication server, additional 0.03 vCPU core and 60 MB RAM are required.

Check OS and software requirements for the following Veeam ONE components:

Veeam ONE Server

Veeam ONE Server

| Specification | Requirement |
| OS | Only 64-bit versions of the following operating systems are supported:   * Microsoft Windows Server 2025 * Microsoft Windows Server 2022 * Microsoft Windows Server 2019 * Microsoft Windows Server 2016 * Microsoft Windows 11 (Professional and Enterprise editions with minimum supported version 22H2) * Microsoft Windows 10 version 1909 and LTS builds (Minimum supported version 21H2 for LTSC channel and 22H2 for GA)   Note: Semi-Annual Channel (SAC) releases are supported. |
| Software | The following components are included in the Veeam ONE setup package and can be installed automatically:   * Microsoft ASP.NET Core Shared Framework 8.0.17 * Microsoft Windows Desktop Runtime 8.0.17 * Microsoft .NET Runtime 8.0.17 * Microsoft .NET Framework 4.7.2  * Microsoft System CLR Types for SQL Server 2014 * Microsoft SQL Server 2014 Management Objects * Microsoft Internet Information Services (IIS) 10.0 or later * Microsoft Application Request Routing 3.0 * IIS URL Rewrite Model 2.1 * Microsoft Universal C Runtime   To connect SCVMM servers to Veeam ONE, the following software is required:   * System Center 2025 Virtual Machine Manager console (for connecting SCVMM 2025 servers) * System Center 2022 Virtual Machine Manager console (for connecting SCVMM 2022 servers) * System Center 2019 Virtual Machine Manager console (for connecting SCVMM 2019 servers) * System Center 2016 Virtual Machine Manager console (for connecting SCVMM 2016 servers) * Microsoft PowerShell 3.0 (required for SCVMM 2016, and SCVMM 2019 consoles)   Be sure to install the same versions of the Admin UI and the SCVMM Server, and to update both components to the same update version. |
| Other | * Windows Management Instrumentation service must be enabled to allow data collection from Veeam Backup & Replication servers. * File and Print Sharing service must be enabled to enable remote Veeam ONE Client connections to the Veeam ONE service. |

Microsoft SQL Server for Veeam ONE

|  |
| --- |
| Note |
| All versions of Microsoft SQL Server must have a supported compatibility level of 130 or later. |

Microsoft SQL Server for Veeam ONE

| Specification | Requirement |
| Software | Microsoft SQL Server (Full and Express Editions):   * Microsoft SQL Server 2025 * Microsoft SQL Server 2022 * Microsoft SQL Server 2019 * Microsoft SQL Server 2017 (Microsoft SQL Server 2017 Express edition without cumulative updates is included in Veeam ONE installation package) * Microsoft SQL Server 2016 * Microsoft Azure SQL Database * Amazon RDS for SQL Server   Reporting Services (optional):   * Microsoft SQL Server Reporting Services 2025 * Microsoft SQL Server Reporting Services 2022 * Microsoft SQL Server Reporting Services 2019 * Microsoft SQL Server Reporting Services 2017 * Microsoft SQL Server Reporting Services 2016 |

|  |
| --- |
| Note: |
| * For production deployment of Veeam ONE, it is recommended to use Microsoft SQL Server Standard Edition or higher and Microsoft SQL Server Reporting Services Standard Edition or higher. * For large-scale deployments with, it is recommended to use Microsoft SQL Server Standard Edition or higher. For details on large-scale deployment recommendations, see [Sizing and Scalability Best Practices](scalability.md). * For production deployment of Veeam ONE, it is recommended to use Microsoft SQL Server Reporting Services Standard Edition or higher. Note that if you use Microsoft SQL Server Reporting Services Developer, Web or Express Editions, Veeam ONE functionality may be limited. * Ensure you have sufficient space on disk for Veeam ONE database. The database can quickly grow in size due to a large amount of collected data, or because of Microsoft SQL Server configuration. For details, see [KB2210](https://www.veeam.com/kb2210). * If you choose to host Veeam ONE database on Microsoft SQL Server Express, be informed there is a 10 GB database (50 GB since Microsoft SQL Server 2025) size limitation for this edition. For details, see [Editions and Supported Features for SQL Server](https://msdn.microsoft.com/en-en/library/cc645993.aspx). * You can run Veeam ONE database in Microsoft SQL Server Always ON availability group. For details, see [KB2312](https://www.veeam.com/kb2312). * In order for the Veeam ONE database to be added to the Always ON Availability Group (AOAG), its recovery model must be switched to Full mode. Consequently, the database begins generating transaction logs that must be managed because Veeam ONE is designed to operate with a Simple recovery model database and does not truncate its transaction logs. * You can host Veeam ONE database installation on Amazon Web Services Relational Database Service (AWS RDS). * Veeam ONE supports only .NET version 8.0. Using any .NET version other than 8.0 can result in errors or failure in Veeam ONE. * Lightweight pooling must be disabled on the SQL Server. |

Veeam ONE Reporting Database

Veeam ONE Reporting Database

| Specification | Requirement |
| Software | PostgreSQL  Local or remote installation of the following versions:   * PostgreSQL 14.x * PostgreSQL 15.x * PostgreSQL 16.x * PostgreSQL 17.x (PostgreSQL 17.6 is included in the Veeam ONE v13 setup) * PostgreSQL 18.x   Note - the PostgreSQL instance must have UTF-8 as the default encoding for the database. |

Veeam ONE Web Services

Veeam ONE Web Services

| Specification | Requirement |
| Hardware | CPU: x86-x64 processor (minimum 2 cores). Using faster multi-core processors improves data processing performance.  Memory: 2 GB RAM (minimum). Using modern high clock memory (DDR3 and higher) improves data processing performance. |
| OS | Only 64-bit versions of the following operating systems are supported:   * Microsoft Windows Server 2025 * Microsoft Windows Server 2022 * Microsoft Windows Server 2019  * Microsoft Windows Server 2016 * Microsoft Windows 11 (Professional and Enterprise editions with minimum supported version 22H2)  * Microsoft Windows 10 version 1909 and LTS builds (Minimum supported version 21H2 for LTSC channel and 22H2 for GA)   Note: Semi-Annual Channel (SAC) releases are supported. |
| Software | The following components are included in the Veeam ONE setup package and can be installed automatically:   * Microsoft .NET Runtime 8.0.17 * Microsoft ASP.NET Core Shared Framework 8.0.17 * Microsoft Windows Desktop Runtime 8.0.17 * Microsoft .NET Framework 4.7.2 * Microsoft System CLR Types for SQL Server 2014 * Microsoft SQL Server 2014 Management Objects * Microsoft Internet Information Services (IIS) 10.0 or later * Microsoft Application Request Routing 3.0 * IIS URL Rewrite Module 2.1 * Microsoft Universal C Runtime |

Veeam ONE Client

Veeam ONE Client

| Specification | Requirement |
| OS | Only 64-bit versions of the following operating systems are supported:   * Microsoft Windows Server 2025 * Microsoft Windows Server 2022 * Microsoft Windows Server 2019  * Microsoft Windows Server 2016 * Microsoft Windows 11 (Professional and Enterprise editions with minimum supported version 22H2)  * Microsoft Windows 10 version 1909 and LTS builds (Minimum supported version 21H2 for LTSC channel and 22H2 for GA)   Note: Semi-Annual Channel (SAC) releases are supported. |
| Software | The following components are included in the Veeam ONE setup package and can be installed automatically:   * Microsoft Windows Desktop Runtime 8.0.17 * Microsoft Core XML 6.0 Parser and SDK * Microsoft Windows Installer 4.5 |

Veeam ONE Web Client

Veeam ONE Web Client

| Specification | Requirement |
| Software | * The latest versions of Microsoft Edge, Google Chrome or Mozilla Firefox. Microsoft Edge Legacy is not supported. * The browser must have JavaScript enabled * Microsoft Office 2010, 2013, 2016, 2019, or Microsoft Office 365 * Microsoft Visio 2010, 2013, 2016, 2019 * Any up-to-date PDF viewer * 1280x720 minimum screen resolution. |

Custom Deployment

If you plan to use the custom deployment scenario, the machines on which you plan to deploy Veeam ONE components must be sized depending on the managed workloads. For details on hardware recommendations for custom deployments, see [System Requirements for Large-Scale Deployment](requirements.md).


