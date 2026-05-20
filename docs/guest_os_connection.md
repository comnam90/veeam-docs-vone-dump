---
title: "Connection to VM Guest OS"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/guest_os_connection.html"
last_updated: "5/19/2026"
product_version: "13.0.1.6168"
---

# Connection to VM Guest OS


The account used to collect data from guest OSes of Windows VMs, must have the following permissions:

* Local Administrator on the guest OS
* List folder contents on all guest OS volumes

|  |
| --- |
| Note: |
| To collect data from non-domain Windows VMs, or VMs with an unelevated local Administrator account, you must complete additional configuration steps to allow Veeam ONE perform data collection. For details, see [Connection Under UAC](connection_under_uac.md). |


