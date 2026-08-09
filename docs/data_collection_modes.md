---
title: "Data Collection Modes"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/data_collection_modes.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Data Collection Modes


Data collection mode determines what metrics Veeam ONE will collect, and specifies the product configuration in a number of areas. Choosing an appropriate data collection mode allows you to optimize monitoring and reporting performance and improve user experience in Veeam ONE.

The [Data Collection Mode](typical_choose_collection_mode.md) is configured during deployment and can be modified after deployment using the [Veeam ONE Settings Utility](appendix.md).

Settings

Changing between data collection modes affects the following Veeam ONE settings.

Settings

| Configuration Option | Description | Veeam backup data and virtual infrastructure | Veeam backup data and large-scale virtual infrastructure | Veeam Backup Data Only |
| VMware real-time performance | Timeout for collecting VMware vSphere real-time performance data. | 30 minutes | 30 minutes | N/A |
| Sampling renewal interval for real-time counters. | 20 seconds | 300 seconds (5 minutes) | N/A |
| VMware historical performance | Sampling renewal interval for historical counters (older than one hour). | 5 minutes | 30 minutes | 5 minutes |
| Sampling renewal interval for historical counters (older than one week). | 2 hours | 2 hours | 2 hours |
| Min tree check interval | Updating the object inventory tree in Veeam ONE Client. | 10 seconds | 1 minute | 10 seconds |
| Page update delay | Loading data after choosing an object in the object inventory tree in Veeam ONE Client. | 0.5 second | 1.5 second | 0.5 second |
| Get VM snapshot timeout | Timeout for collecting data about VM snapshot files from datastores. | 900 seconds (15 minutes) | 3600 seconds (1 hour) | 900 seconds (15 minutes) |
| Virtual machines files data collection | Collecting information about VM files (for the Active Snapshots and Garbage Files reports). | Yes | No | No |
| Hyper-V real-time performance | Timeout for collecting Microsoft Hyper-V real-time performance data. | 30 minutes | 30 minutes | N/A |
| Sampling renewal interval for real-time counters. | 60 seconds | 300 seconds (5 minutes) | N/A |

Collected Performance Metrics

Data collection mode defines what performance metrics must be collected.

Collected Performance Metrics

| Performance Metric | Object Type | Veeam backup data and virtual infrastructure | Veeam backup data and large-scale virtual infrastructure | Veeam Backup Data Only |
| Available Memory | Backup Enterprise Manager | Yes | Yes | Yes |
| CPU Usage | Backup Enterprise Manager | Yes | Yes | Yes |
| Disk Bytes/sec | Backup Enterprise Manager | Yes | Yes | Yes |
| Memory Usage | Backup Enterprise Manager | Yes | Yes | Yes |
| Network Bytes Sent/sec | Backup Enterprise Manager | Yes | Yes | Yes |
| Available Memory | Backup Server | Yes | Yes | Yes |
| CPU Usage | Backup Server | Yes | Yes | Yes |
| Disk Bytes/sec | Backup Server | Yes | Yes | Yes |
| Memory Usage | Backup Server | Yes | Yes | Yes |
| Network Bytes Sent/sec | Backup Server | Yes | Yes | Yes |
| Available Memory | Backup Repository | Yes | Yes | Yes |
| Backup Repository Capacity | Backup Repository | Yes | Yes | Yes |
| CPU Usage | Backup Repository | Yes | Yes | Yes |
| Disk Bytes/sec | Backup Repository | Yes | Yes | Yes |
| Memory Usage | Backup Repository | Yes | Yes | Yes |
| Network Bytes Sent/sec | Backup Repository | Yes | Yes | Yes |
| Repository File Backups Size | Backup Repository | Yes | Yes | Yes |
| Repository Image Backups Size | Backup Repository | Yes | Yes | Yes |
| Repository Used Space | Backup Repository | Yes | Yes | Yes |
| Slot Capacity | Backup Repository | Yes | Yes | Yes |
| Used Slots | Backup Repository | Yes | Yes | Yes |
| Available Memory | Backup Proxy | Yes | Yes | Yes |
| CPU Usage | Backup Proxy | Yes | Yes | Yes |
| CDP Proxy Cache Size | Backup Proxy | Yes | Yes | Yes |
| CDP Proxy Cache Usage | Backup Proxy | Yes | Yes | Yes |
| CDP Proxy Cache Usage % | Backup Proxy | Yes | Yes | Yes |
| Disk Bytes/sec | Backup Proxy | Yes | Yes | Yes |
| Memory Usage | Backup Proxy | Yes | Yes | Yes |
| Network Bytes Sent/sec | Backup Proxy | Yes | Yes | Yes |
| Slot Capacity | Backup Proxy | Yes | Yes | Yes |
| Used Slots | Backup Proxy | Yes | Yes | Yes |
| Available Memory | WAN Accelerator | Yes | Yes | Yes |
| CPU Usage | WAN Accelerator | Yes | Yes | Yes |
| Disk Bytes/sec | WAN Accelerator | Yes | Yes | Yes |
| Memory Usage | WAN Accelerator | Yes | Yes | Yes |
| Network Bytes Sent/sec | WAN Accelerator | Yes | Yes | Yes |
| Available Memory | Tape Server | Yes | Yes | Yes |
| CPU Usage | Tape Server | Yes | Yes | Yes |
| Disk Bytes/sec | Tape Server | Yes | Yes | Yes |
| Memory Usage | Tape Server | Yes | Yes | Yes |
| Network Bytes Sent/sec | Tape Server | Yes | Yes | Yes |
| External Repository Used Space | External Repository Used Space | Yes | Yes | Yes |
| Object Storage Repository Used Space | Object Storage Repository Used Space | Yes | Yes | Yes |
| Storage Usage | VMware Cloud Director Organization VDC | Yes | Yes | No |
| CPU Usage | VMware Cloud Director Provider VDC | Yes | Yes | No |
| Memory Usage | VMware Cloud Director Provider VDC | Yes | Yes | No |
| Storage Space Usage | VMware Cloud Director Provider VDC | Yes | No | No |
| Storage Space Usage Pct | VMware Cloud Director Provider VDC | Yes | Yes | No |
| Backup Job Memory Usage | Veeam Backup & Replication Objects | Yes | Yes | Yes |
| Backup Job Processor Usage | Veeam Backup & Replication Objects | Yes | Yes | Yes |
| Adapter I/O | ESXi Host | Yes | No | No |
| Adapter Read I/O | ESXi Host | Yes | No | No |
| Adapter Read Latency | ESXi Host | Yes | No | No |
| Adapter Read Rate | ESXi Host | Yes | No | No |
| Adapter Write I/O | ESXi Host | Yes | No | No |
| Adapter Write Latency | ESXi Host | Yes | No | No |
| Adapter Write Rate | ESXi Host | Yes | No | No |
| Average CPU Ready | ESXi Host | Yes | Yes | No |
| CPU Usage | ESXi Host | Yes | Yes | No |
| CPU Usage MHz | ESXi Host | Yes | Yes | No |
| Disk/ESXi: Datastore Bus Resets | ESXi Host | Yes | Yes | No |
| Disk/ESXi: Datastore Command Aborts | ESXi Host | Yes | Yes | No |
| Disk/ESXi: Datastore Highest Latency | ESXi Host | Yes | Yes | No |
| Disk/ESXi: Datastore I/O | ESXi Host | Yes | Yes | No |
| Disk/ESXi: Datastore Latency Observed by VMs | ESXi Host | Yes | No | No |
| Disk/ESXi: Datastore Maximum Queue Depth | ESXi Host | Yes | No | No |
| Disk/ESXi: Datastore Read I/O | ESXi Host | Yes | Yes | No |
| Disk/ESXi: Datastore Read Latency | ESXi Host | Yes | Yes | No |
| Disk/ESXi: Datastore Read Rate | ESXi Host | Yes | Yes | No |
| Disk/ESXi: Datastore Usage | ESXi Host | Yes | Yes | No |
| Disk/ESXi: Datastore Write I/O | ESXi Host | Yes | Yes | No |
| Disk/ESXi: Datastore Write Latency | ESXi Host | Yes | Yes | No |
| Disk/ESXi: Datastore Write Rate | ESXi Host | Yes | Yes | No |
| Memory Active | ESXi Host | Yes | Yes | No |
| Memory Baloon | ESXi Host | Yes | Yes | No |
| Memory Compressed | ESXi Host | Yes | No | No |
| Memory Consumed | ESXi Host | Yes | Yes | No |
| Memory Latency | ESXi Host | Yes | No | No |
| Memory Overhead | ESXi Host | Yes | No | No |
| Memory Pressure | ESXi Host | Yes | Yes | No |
| Memory Shared | ESXi Host | Yes | No | No |
| Memory Shared Common | ESXi Host | Yes | No | No |
| Memory Swap Used | ESXi Host | Yes | Yes | No |
| Memory Usage | ESXi Host | Yes | Yes | No |
| Network Receive Rate | ESXi Host | Yes | Yes | No |
| Network Transmit Rate | ESXi Host | Yes | Yes | No |
| Network Usage | ESXi Host | Yes | Yes | No |
| Packet Receive Errors | ESXi Host | Yes | No | No |
| Packet Transmit Errors | ESXi Host | Yes | No | No |
| Path I/O | ESXi Host | Yes | No | No |
| Path Read I/O | ESXi Host | Yes | No | No |
| Path Read Latency | ESXi Host | Yes | No | No |
| Path Read Rate | ESXi Host | Yes | No | No |
| Path Write I/O | ESXi Host | Yes | No | No |
| Path Write Latency | ESXi Host | Yes | No | No |
| Path Write Rate | ESXi Host | Yes | No | No |
| Power Usage | ESXi Host | Yes | No | No |
| Receive Packets Dropped | ESXi Host | Yes | No | No |
| Received Packets per Second | ESXi Host | Yes | No | No |
| Swap In Rate | ESXi Host | Yes | No | No |
| Swap Out Rate | ESXi Host | Yes | No | No |
| Total Errors | ESXi Host | Yes | No | No |
| Total Packets Dropped | ESXi Host | Yes | No | No |
| Transmit Packets Dropped | ESXi Host | Yes | No | No |
| Transmitted Packets per Second | ESXi Host | Yes | No | No |
| VM Heartbeat | ESXi Host | Yes | Yes | No |
| Average CPU Idle All Cores | vSphere Virtual Machine | Yes | No | No |
| Average CPU Ready All Cores | vSphere Virtual Machine | Yes | Yes | No |
| Average CPU Standstill All Cores | vSphere Virtual Machine | Yes | No | No |
| Average CPU Wait All Cores | vSphere Virtual Machine | Yes | No | No |
| CPU Co-Stop All Cores | vSphere Virtual Machine | Yes | No | No |
| CPU Usage | vSphere Virtual Machine | Yes | Yes | No |
| CPU Usage MHz | vSphere Virtual Machine | Yes | Yes | No |
| Datastore Bus Resets | vSphere Virtual Machine | Yes | Yes | No |
| Datastore Command Aborts | vSphere Virtual Machine | Yes | Yes | No |
| Datastore Highest Latency | vSphere Virtual Machine | Yes | Yes | No |
| Datastore I/O | vSphere Virtual Machine | Yes | Yes | No |
| Datastore Read I/O | vSphere Virtual Machine | Yes | Yes | No |
| Datastore Read Latency | vSphere Virtual Machine | Yes | Yes | No |
| Datastore Read Rate | vSphere Virtual Machine | Yes | Yes | No |
| Datastore Usage | vSphere Virtual Machine | Yes | Yes | No |
| Datastore Write I/O | vSphere Virtual Machine | Yes | Yes | No |
| Datastore Write Latency | vSphere Virtual Machine | Yes | Yes | No |
| Datastore Write Rate | vSphere Virtual Machine | Yes | Yes | No |
| Disk/vSAN: Recovery Write I/O | vSphere Virtual Machine | Yes | No | No |
| Disk/vSAN: Recovery Write Latency | vSphere Virtual Machine | Yes | No | No |
| Disk/vSAN: Recovery Write Rate | vSphere Virtual Machine | Yes | No | No |
| Guest Disk Free Space | vSphere Virtual Machine | Yes | No | No |
| Guest Disk Usage | vSphere Virtual Machine | Yes | Yes | No |
| Memory Active | vSphere Virtual Machine | Yes | Yes | No |
| Memory Baloon | vSphere Virtual Machine | Yes | Yes | No |
| Memory Baloon Percent | vSphere Virtual Machine | Yes | Yes | No |
| Memory Compressed | vSphere Virtual Machine | Yes | No | No |
| Memory Consumed | vSphere Virtual Machine | Yes | Yes | No |
| Memory Entitlement | vSphere Virtual Machine | Yes | No | No |
| Memory Latency | vSphere Virtual Machine | Yes | No | No |
| Memory Overhead | vSphere Virtual Machine | Yes | No | No |
| Memory Saved by Zipping | vSphere Virtual Machine | Yes | No | No |
| Memory Shared | vSphere Virtual Machine | Yes | No | No |
| Memory Swapped | vSphere Virtual Machine | Yes | Yes | No |
| Memory Usage | vSphere Virtual Machine | Yes | Yes | No |
| Network Receive Rate | vSphere Virtual Machine | Yes | Yes | No |
| Network Transmit Rate | vSphere Virtual Machine | Yes | Yes | No |
| Network Usage | vSphere Virtual Machine | Yes | Yes | No |
| Power Usage | vSphere Virtual Machine | Yes | No | No |
| Process CPU Usage | vSphere Virtual Machine | Yes | Yes | No |
| Process Memory Usage | vSphere Virtual Machine | Yes | Yes | No |
| Read I/O | vSphere Virtual Machine | Yes | No | No |
| Read Latency | vSphere Virtual Machine | Yes | No | No |
| Read Rate | vSphere Virtual Machine | Yes | No | No |
| Received Packets per Second | vSphere Virtual Machine | Yes | No | No |
| Running Services | vSphere Virtual Machine | Yes | Yes | No |
| Swap In Rate | vSphere Virtual Machine | Yes | No | No |
| Swap Out Rate | vSphere Virtual Machine | Yes | Yes | No |
| Transmitted Packets per Second | vSphere Virtual Machine | Yes | No | No |
| Virtual Disk Provisioned | vSphere Virtual Machine | Yes | Yes | No |
| Virtual Disk Used | vSphere Virtual Machine | Yes | Yes | No |
| VM Hearbeat | vSphere Virtual Machine | Yes | Yes | No |
| Write I/O | vSphere Virtual Machine | Yes | No | No |
| Write Latency | vSphere Virtual Machine | Yes | No | No |
| Write Rate | vSphere Virtual Machine | Yes | Yes | No |
| Disk/Datastore: Datastore Bus Resets | vSphere Datastore | Yes | Yes | No |
| Disk/Datastore: Datastore Command Aborts | vSphere Datastore | Yes | Yes | No |
| Disk/Datastore: Datastore I/O | vSphere Datastore | Yes | Yes | No |
| Disk/Datastore: Datastore Provisioned Space | vSphere Datastore | Yes | Yes | No |
| Disk/Datastore: Datastore Read I/O | vSphere Datastore | Yes | Yes | No |
| Disk/Datastore: Datastore Read Latency | vSphere Datastore | Yes | Yes | No |
| Disk/Datastore: Datastore Read Rate | vSphere Datastore | Yes | Yes | No |
| Disk/Datastore: Datastore Usage | vSphere Datastore | Yes | Yes | No |
| Disk/Datastore: Datastore Write I/O | vSphere Datastore | Yes | Yes | No |
| Disk/Datastore: Datastore Write Latency | vSphere Datastore | Yes | Yes | No |
| Disk/Datastore: Datastore Write Rate | vSphere Datastore | Yes | Yes | No |
| Disk/Datastore: Free Space | vSphere Datastore | Yes | Yes | No |
| Average Pressure | Hyper-V Host | Yes | Yes | No |
| Committed Bytes | Hyper-V Host | Yes | No | No |
| Disk/Host: Avg Disk Queue Length | Hyper-V Host | Yes | Yes | No |
| Disk/Host: Avg Disk Read Bytes/sec | Hyper-V Host | Yes | Yes | No |
| Disk/Host: Avg Disk sec/Read | Hyper-V Host | Yes | Yes | No |
| Disk/Host: Avg Disk sec/Write | Hyper-V Host | Yes | Yes | No |
| Disk/Host: Avg Disk Usage Bytes/sec | Hyper-V Host | Yes | Yes | No |
| Disk/Host: Avg Disk Write Bytes/sec | Hyper-V Host | Yes | Yes | No |
| Guest Run Time | Hyper-V Host | Yes | No | No |
| Heartbeat | Hyper-V Host | Yes | Yes | No |
| Heartbeat Status | Hyper-V Host | Yes | Yes | No |
| Host CPU Wait Time | Hyper-V Host | Yes | Yes | No |
| Hyper-V Services Memory Consumed | Hyper-V Host | Yes | Yes | No |
| Hyper-V Services Memory Usage | Hyper-V Host | Yes | Yes | No |
| Hypervisor Run Time | Hyper-V Host | Yes | No | No |
| Idle Time | Hyper-V Host | Yes | Yes | No |
| Memory Consumed | Hyper-V Host | Yes | Yes | No |
| Memory Usage | Hyper-V Host | Yes | Yes | No |
| Network Bytes Received/sec | Hyper-V Host | Yes | Yes | No |
| Network Bytes Sent/sec | Hyper-V Host | Yes | Yes | No |
| Network Bytes Total/sec | Hyper-V Host | Yes | Yes | No |
| Network Offloaded Connections | Hyper-V Host | Yes | No | No |
| Network Outbound Errors | Hyper-V Host | Yes | Yes | No |
| Network Output Queue Length | Hyper-V Host | Yes | Yes | No |
| Network Packets Received/sec | Hyper-V Host | Yes | No | No |
| Network Packets Sent/sec | Hyper-V Host | Yes | No | No |
| Network Packets/sec | Hyper-V Host | Yes | No | No |
| Network Received Errors | Hyper-V Host | Yes | No | No |
| Page Faults/sec | Hyper-V Host | Yes | No | No |
| Page Reads/sec | Hyper-V Host | Yes | No | No |
| Page Writes/sec | Hyper-V Host | Yes | No | No |
| Pages Input/sec | Hyper-V Host | Yes | No | No |
| Pages Output/sec | Hyper-V Host | Yes | No | No |
| Pages/sec | Hyper-V Host | Yes | Yes | No |
| Total Interrupts/sec | Hyper-V Host | Yes | No | No |
| Total Run Time | Hyper-V Host | Yes | Yes | No |
| Total Run Time MHz | Hyper-V Host | Yes | Yes | No |
| vCPU Total Run Time | Hyper-V Host | Yes | No | No |
| Virtual Switch Bytes Received/sec | Hyper-V Host | Yes | No | No |
| Virtual Switch Bytes Sent/sec | Hyper-V Host | Yes | No | No |
| Virtual Switch Bytes/sec | Hyper-V Host | Yes | No | No |
| Virtual Switch Packets Received/sec | Hyper-V Host | Yes | No | No |
| Virtual Switch Packets Sent/sec | Hyper-V Host | Yes | No | No |
| Virtual Switch Packets/sec | Hyper-V Host | Yes | No | No |
| CPU Wait Time | Hyper-V Virtual Machine | Yes | Yes | No |
| Current Pressure | Hyper-V Virtual Machine | Yes | Yes | No |
| Demand | Hyper-V Virtual Machine | Yes | Yes | No |
| Errors/min | Hyper-V Virtual Machine | Yes | Yes | No |
| Flushes/min | Hyper-V Virtual Machine | Yes | Yes | No |
| Guest Disk Free Space | Hyper-V Virtual Machine | Yes | Yes | No |
| Guest Disk Used Space | Hyper-V Virtual Machine | Yes | Yes | No |
| Guest Run Time | Hyper-V Virtual Machine | Yes | Yes | No |
| Guest vCPU Guest Run Time MHz | Hyper-V Virtual Machine | Yes | Yes | No |
| Guest Visible Physical Memory | Hyper-V Virtual Machine | Yes | Yes | No |
| Hypervisor Run Time | Hyper-V Virtual Machine | Yes | No | No |
| IOPS | Hyper-V Virtual Machine | Yes | Yes | No |
| Legacy Network Bytes /sec | Hyper-V Virtual Machine | Yes | No | No |
| Legacy Network Bytes Dropped/sec | Hyper-V Virtual Machine | Yes | No | No |
| Legacy Network Bytes Received/sec | Hyper-V Virtual Machine | Yes | No | No |
| Legacy Network Bytes Sent/sec | Hyper-V Virtual Machine | Yes | No | No |
| Physical Memory | Hyper-V Virtual Machine | Yes | Yes | No |
| Process CPU Usage | Hyper-V Virtual Machine | Yes | Yes | No |
| Process Memory Usage | Hyper-V Virtual Machine | Yes | Yes | No |
| Reads/sec | Hyper-V Virtual Machine | Yes | Yes | No |
| Running Services | Hyper-V Virtual Machine | Yes | Yes | No |
| Total Run Time | Hyper-V Virtual Machine | Yes | Yes | No |
| vCPU Total Run Time MHz | Hyper-V Virtual Machine | Yes | No | No |
| Virtual Disk Provisioned | Hyper-V Virtual Machine | Yes | Yes | No |
| Virtual Disk Used | Hyper-V Virtual Machine | Yes | Yes | No |
| Virtual Network Bytes /sec | Hyper-V Virtual Machine | Yes | Yes | No |
| Virtual Network Bytes Received/sec | Hyper-V Virtual Machine | Yes | Yes | No |
| Virtual Network Bytes Sent/sec | Hyper-V Virtual Machine | Yes | Yes | No |
| Virtual Network Packets Received/sec | Hyper-V Virtual Machine | Yes | No | No |
| Virtual Network Packets Sent/sec | Hyper-V Virtual Machine | Yes | No | No |
| Virtual Storage Read Bytes/sec | Hyper-V Virtual Machine | Yes | Yes | No |
| Virtual Storage Usage Bytes/sec | Hyper-V Virtual Machine | Yes | Yes | No |
| Virtual Storage Write Bytes/sec | Hyper-V Virtual Machine | Yes | Yes | No |
| Writes/sec | Hyper-V Virtual Machine | Yes | Yes | No |
| Disk Free Space | Hyper-V Physical Disk | Yes | Yes | No |
| Disk Provisioned Space | Hyper-V Physical Disk | Yes | Yes | No |
| Disk Used Space | Hyper-V Physical Disk | Yes | Yes | No |
| Disk/Physical Disk: Avg Disk Queue Length | Hyper-V Physical Disk | Yes | No | No |
| Disk/Physical Disk: Avg Disk sec/Read | Hyper-V Physical Disk | Yes | Yes | No |
| Disk/Physical Disk: Avg Disk sec/Write | Hyper-V Physical Disk | Yes | Yes | No |
| Disk/Physical Disk: Disk Bytes/sec | Hyper-V Physical Disk | Yes | Yes | No |
| Disk/Physical Disk: Disk Read Bytes/sec | Hyper-V Physical Disk | Yes | Yes | No |
| Disk/Physical Disk: Disk Transfers/sec | Hyper-V Physical Disk | Yes | Yes | No |
| Disk/Physical Disk: Disk Write Bytes/sec | Hyper-V Physical Disk | Yes | Yes | No |
| Cache IO Read Bytes/sec | Hyper-V CSV 2012 | Yes | No | No |
| Cache Reads/sec | Hyper-V CSV 2012 | Yes | No | No |
| CSV FS Free Space | Hyper-V CSV 2012 | Yes | Yes | No |
| CSV FS Provisioned Space | Hyper-V CSV 2012 | Yes | No | No |
| CSV FS Used Space | Hyper-V CSV 2012 | Yes | No | No |
| Disk/CSV 2012: Direct Bytes/sec | Hyper-V CSV 2012 | Yes | Yes | No |
| Disk/CSV 2012: Direct IOPS | Hyper-V CSV 2012 | Yes | Yes | No |
| Disk/CSV 2012: Direct Latency | Hyper-V CSV 2012 | Yes | Yes | No |
| Disk/CSV 2012: IOPS | Hyper-V CSV 2012 | Yes | No | No |
| Disk/CSV 2012: Latency | Hyper-V CSV 2012 | Yes | Yes | No |
| Disk/CSV 2012: Queue Length | Hyper-V CSV 2012 | Yes | No | No |
| Disk/CSV 2012: Read Bytes/sec | Hyper-V CSV 2012 | Yes | Yes | No |
| Disk/CSV 2012: Read Latency | Hyper-V CSV 2012 | Yes | Yes | No |
| Disk/CSV 2012: Read Queue Length | Hyper-V CSV 2012 | Yes | No | No |
| Disk/CSV 2012: Reads/sec | Hyper-V CSV 2012 | Yes | No | No |
| Disk/CSV 2012: Redirected Bytes/sec | Hyper-V CSV 2012 | Yes | Yes | No |
| Disk/CSV 2012: Redirected IOPS | Hyper-V CSV 2012 | Yes | Yes | No |
| Disk/CSV 2012: Redirected Latency | Hyper-V CSV 2012 | Yes | Yes | No |
| Disk/CSV 2012: Total Bytes/sec | Hyper-V CSV 2012 | Yes | Yes | No |
| Disk/CSV 2012: Write Bytes/sec | Hyper-V CSV 2012 | Yes | Yes | No |
| Disk/CSV 2012: Write Latency | Hyper-V CSV 2012 | Yes | Yes | No |
| Disk/CSV 2012: Write Queue Length | Hyper-V CSV 2012 | Yes | No | No |
| Disk/CSV 2012: Writes/sec | Hyper-V CSV 2012 | Yes | No | No |
| SMB Share Free Space | Hyper-V Share | Yes | Yes | No |
| SMB Share Used Space | Hyper-V Share | Yes | No | No |
| SMB Share Provisioned Space | Hyper-V Share | Yes | No | No |
| Disk/Share: IOPS | Hyper-V Share | Yes | No | No |
| Disk/Share: Writes/sec | Hyper-V Share | Yes | No | No |
| Disk/Share: Reads/sec | Hyper-V Share | Yes | No | No |
| Disk/Share: Virtual Storage Usage Bytes/sec | Hyper-V Share | Yes | No | No |
| Disk/Share: Virtual Storage Write Bytes/sec | Hyper-V Share | Yes | Yes | No |
| Disk/Share: Virtual Storage Read Bytes/sec | Hyper-V Share | Yes | Yes | No |
| Disk/Share: SMB Share Error Count/min | Hyper-V Share | Yes | No | No |
| Disk/Share: SMB Share Flush Count/min | Hyper-V Share | Yes | No | No |

Page updated 2026-08-03

