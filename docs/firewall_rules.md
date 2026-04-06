---
title: "Firewall Rules"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/firewall_rules.html"
last_updated: "4/3/2025"
product_version: "13.0.1.6168"
---

# Firewall Rules


The following table lists exceptions that should be enabled in Windows Firewall Settings.

Firewall Rules

| Server | App/Feature | Details |
| Hyper-V host | Remote Event Log Management:   * Remote Event Log Management (NP-In) * Remote Event Log Management (RPC) * Remote Event Log Management (RPC-EPMAP)   COM+ Network Access:   * COM+ Network Access (DCOM-In) | Required to collect events data from Hyper-V hosts. |
| Veeam Backup & Replication server | Remote Event Log Management:   * Remote Event Log Management (NP-In) * Remote Event Log Management (RPC) * Remote Event Log Management (RPC-EPMAP)   COM+ Network Access:   * COM+ Network Access (DCOM-In) | Required to collect events data from Veeam Backup & Replication servers. |
| Veeam Backup for Microsoft 365 Server | COM+ Network Access:   * COM+ Network Access (DCOM-In)   Network Discovery:   * Network Discovery (LLMNR-UDP-In) | Required to gather CPU and memory performance data from Veeam Backup for Microsoft 365 servers. |


