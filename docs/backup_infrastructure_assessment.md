---
title: "Backup Infrastructure Assessment"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_infrastructure_assessment.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Backup Infrastructure Assessment


This report evaluates how optimally your backup infrastructure is configured and suggests actions aimed at boosting its efficiency.

|  |
| --- |
| Note: |
| * This report is available for VMware vSphere environments only.  * Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, Veeam ONE Web Client may show invalid data for Veeam Backup & Replication reports and dashboards. * Veeam Cloud Connect service providers cannot see performance data for proxies used by tenant data protection jobs. |

The report analyzes configuration of your virtual environment against a set of recommended baseline settings and implementations, identifies VMs that cannot be properly backed up due to configuration limitations, verifies problem areas and helps mitigate the issues.

* The Summary display contains the Verification Results chart that displays how many verification tests failed, passed or completed with warnings and how many criteria do not apply to your backup infrastructure (in percentage).
* The Report Data display shows whether verification tests for each criteria failed, passed or completed with warnings and marks criteria that does not apply to the infrastructure as Not required. It also shows a summary of recommendations for each test within the report infrastructure.

The report takes into account the following criteria when analyzing infrastructure configuration:

VM Configuration and Application-aware VM Processing

VM Configuration and Application-aware VM Processing

| Criterion | Description |
| Application-aware image processing for Windows Servers | The report searches for jobs that do not have the Enable application-aware image processing option enabled.  To create a transactionally consistent backup of a VM running VSS-aware applications (such as Active Directory, Microsoft SQL, Microsoft Exchange, Sharepoint) without shutting them down, Veeam Backup & Replication uses application-aware image processing. It is a proprietary technology that ensures successful VM recovery, as well as proper recovery of all applications installed on the VM without any data loss. |
| VMware tools quiescence for Linux/Unix VMs | The report searches for jobs that do not have the Enable VMware Tools quiescence option enabled.  When taking snapshots of a running VM, VMware Tools will quiesce the VM file systems to ensure integrity of on-disk data. However, under heavy I/O load, this delay in I/O could become too long. |
| VMware tools status | The report analyzes your virtual infrastructure to find VMs that do not have VMware Tools installed, running or up-to-date.  To enable backup with application-aware image processing, it is required that guest OS running inside your VMs have VMware Tools installed and running. |
| VMs verification | The report analyzes your virtual infrastructure to find VMs for which SureBackup jobs are not configured.  SureBackup and SureReplica are technologies developed to automate and simplify the recovery verification process — one of the most crucial parts of data management and protection. SureBackup and SureReplica let users verify the recoverability of every VM backup and replica, without additional hardware or administrative time and effort. |

Job Performance Optimization

Job Performance Optimization

| Criterion | Description |
| Parallel virtual disk processing | The report searches for Veeam Backup servers that do not have the Enable parallel VM and virtual disk processing option enabled.  Multiple VMs and VM disks can be processed in parallel, optimizing your backup infrastructure performance and increasing the efficiency of resource usage. |
| Virtual stand-by proxy server | The report analyzes your virtual infrastructure to find virtual backup proxy servers.  For data retrieval,Veeam Backup & Replication offers the Virtual Appliance mode. The mode can only be used if the backup proxy is deployed on a VM.  The Virtual Appliance mode uses the SCSI hot-add capability of ESXi hosts to attach disks of the backed up VM to the backup proxy VM. In this mode, VM data is retrieved directly from storage through the ESXi I/O stack, instead of going through the network stack, which improves performance. |
| Proxy server on the remote site | The report analyzes your virtual infrastructure to find backup proxy servers on the remote site.  Storing backups offsite always involves moving large volumes of data between remote sites. To solve the problem of insufficient network bandwidth to support VM data traffic and optimize data transfer over the WAN, it is recommended to deploy a proxy server on the remote site. |
| Direct SAN access iSCSI performance tweaks | The report analyzes your infrastructure to find backup proxies configured to use the Direct SAN Access mode working with iSCSI storage.  The Direct SAN Access mode is recommended if the ESXi host uses shared storage. The backup proxy leverages VADP to retrieve VM data directly from FC or iSCSI storage in the Storage Area Network (SAN). To retrieve data blocks from SAN LUN, the backup proxy uses metadata about the layout of VM disks on the SAN. Since data blocks are not retrieved over the Local Area Network (LAN), this mode minimizes disruptions to your production network during backup. |
| Meeting Backup Window | The report analyzes job sessions to find jobs whose duration exceeds the defined backup window.  If job duration exceeds the backup window and the bottleneck is a proxy, the report will provide recommendations to deploy more proxies.  This criterion is available only if you specified the Required Backup Window parameter. |
| Backup job processing mode optimizations | The report analyzes job statistics to find bottlenecks in the data flow.  As any backup application handles a great amount of data, it is important to make sure the data flow is efficient and all resources engaged in the backup process are optimally used. To identify a bottleneck in the data path, Veeam Backup & Replication detects the component with the maximum workload: that is, the component that works for the most time of the job.  In case the report discovers that a backup proxy is the weakest component in the data flow, it is recommended to deploy additional proxy servers. |

Backup Infrastructure Configuration

Backup Infrastructure Configuration

| Criterion | Description |
| VMs failed over to network processing mode | The report analyzes your virtual infrastructure to find VMs that failed over to the Network Processing mode.  The Network Processing mode can be used with any infrastructure configuration. However, when an alternative transport mode is applicable, the Network mode is not recommended because of the lowest data retrieval speed. |
| Backup server protection | The report analyzes your virtual infrastructure to find backup servers that do not run configuration backups on their database.  If a Veeam backup server fails, you can re-deploy the Veeam backup server, restore configuration data for the Veeam backup server from the backup and apply it to the re-built server. Alternatively, you can apply configuration data to any other Veeam backup server in your backup infrastructure. In terms of configuration, you get a replica of the Veeam backup server you had, without additional adjustments and fine-tuning. |
| SQL Server optimization | The report analyzes Veeam Backup & Replication databases hosted on SQL Server Express instances to check whether these instances need to be upgraded to the full version of SQL Server.  If the amount of data stored in Veeam Backup & Replication databases exceeds SQL Server Express capabilities, it may cause slow operation of the Veeam Backup & Replication console. |
| Repository free space | The report analyzes your virtual infrastructure to find repositories that have run out of free space. |
| Storage latency control | The report searches for jobs that do not have the Enable storage latency control option enabled.  Storage latency control should be enabled in the Veeam Backup & Replication console to ensure that running jobs do not impact storage availability to production workloads. |
| Proxy Server Configuration | The report analyzes your virtual infrastructure to find backup proxy servers for which the number of concurrent tasks is greater than the number of CPU cores. |

File level restores

File level restores

| Criterion | Description |
| Indexing of Guest OS files (optional) | The report searches for jobs that do not have the Enable guest file system indexing option enabled.  This criterion is available only if you selected the 1-Click file level restores parameter. |

Report Parameters

You can specify the following report parameters:

* Scope: defines a list of Veeam Backup & Replication servers to include in the report.
* 1-Click file restore sessions: defines whether the report will analyze the 1-click file level restore capabilities.
* Required backup window: defines an interval for daily backup sessions that should be assessed.

[View Report Example](./reports/Backup%20Infrastructure%20Assessment.pdf)

Use Case

The size and complexity of modern geographically disperse backup infrastructures makes it difficult to manage and optimize them.

Following the report recommendations, backup administrators can improve job configuration and implement the necessary hardware and software optimizations. This will help you attain better efficiency, lower resource consumption and expedite backup time.


