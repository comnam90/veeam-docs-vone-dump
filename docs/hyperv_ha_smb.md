---
title: "HA SMB Performance Chart"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/hyperv_ha_smb.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# HA SMB Performance Chart


The HA Disk chart displays historical statistics on disk usage for the selected Highly Available SMB share created on Cluster Shared Volumes.

The following table provides information on predefined views and counters.

HA SMB Performance Chart

| Chart View | Counter | Measurement Unit | Description |
| Usage | Disk/CSV: Read | KB/s | Rate at which data was read from a volume in the Direct Access or Redirected Access mode. |
| Disk/CSV: Write | KB/s | Rate at which data was written to a volume in the Direct Access or Redirected Access mode. |
| Disk/CSV: Total | KB/s | Rate at which data was read from and written to a volume in the Direct Access or Redirected Access mode. |
| IOPS | Disk/CSV: Read/sec | Number | Rate at which read operations were performed directly on a volume. |
| Disk/CSV: Writes/sec | Number | Rate at which write operations were performed directly on a volume. |
| Disk/CSV: IOPS | Number | Rate at which read and write operations were performed directly on a volume. |
| Latency | Disk/CSV: Read Latency | Millisecond | Average latency between the time a read request arrived to a file system and the time when it was completed. |
| Disk/CSV: Write Latency | Millisecond | Average latency between the time a write request arrived to the file system and the time when it was completed. |
| Disk/CSV: Latency | Millisecond | Average latency required to complete read and write operations on a volume. |
| Datastore Queue Length | Disk/CSV: Read Queue Length | Number | Number of read operations queued for a volume. |
| Disk/CSV: Write Queue Length | Number | Number of write operations queued for a volume. |
| Disk/CSV: Queue Length | Number | Total number of read and write operations queued for a volume during the sample interval. |
| Direct/Redirected Usage | Disk/CSV: Redirected Bytes/sec | KB/s | Average amount of data transferred to or from the disk during write or read operations over the network stack. |
| Disk/CSV: Direct Bytes/sec | KB/s | Average amount of data transferred to or from the disk during write or read operations. |
| Direct/Redirected Latency | Disk/CSV: Direct Latency | Millisecond | Average latency required to complete read and write operations on a volume in the Direct Access mode. |
| Disk/CSV: Redirected Latency | Millisecond | Average latency required to complete read and write operations on a volume in the Redirected Access mode. |
| Direct/Redirected IOPS | Disk/CSV: Direct IOPS | Number | Rate at which read and write operations were performed directly on a disk. |
| Disk/CSV: Redirected IOPS | Number | Rate at which read and write operations were redirected to a volume through the network. |

Page updated 2026-08-03

