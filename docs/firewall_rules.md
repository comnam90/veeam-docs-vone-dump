---
title: "Firewall Rules"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/firewall_rules.html"
last_updated: "6/19/2026"
product_version: "13.0.2.6723"
---

# Firewall Rules


The following table lists exceptions that should be enabled in Windows Firewall Settings. For details on additional firewall rules, see this [KB](https://www.veeam.com/kb2696) article.

Firewall Rules

| Server | App/Feature | Details |
| Hyper-V host | Remote Event Log Management:   * Remote Event Log Management (NP-In) * Remote Event Log Management (RPC) * Remote Event Log Management (RPC-EPMAP)   COM+ Network Access:   * COM+ Network Access (DCOM-In) | Required to collect events data from Hyper-V hosts. |
| Veeam Backup & Replication server | Remote Event Log Management:   * Remote Event Log Management (NP-In) * Remote Event Log Management (RPC) * Remote Event Log Management (RPC-EPMAP)   COM+ Network Access:   * COM+ Network Access (DCOM-In) | Required to collect events data from Veeam Backup & Replication servers. |
| Veeam Backup for Microsoft 365 Server | COM+ Network Access:   * COM+ Network Access (DCOM-In)   Network Discovery:   * Network Discovery (LLMNR-UDP-In) | Required to gather CPU and memory performance data from Veeam Backup for Microsoft 365 servers. |


