---
title: "Connection Settings"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/connection_settings.html"
last_updated: "4/3/2025"
product_version: "13.0.1.6168"
---

# Connection Settings


To ensure that Veeam ONE can update the license and Veeam Intelligent Diagnostics signatures and send license usage statistics to the Veeam licensing server, check that:

* The firewall on Veeam ONE Server allows connections required for proper communication between Veeam ONE components. For more information, see [Ports](ports.md) and [Firewall Rules](firewall_rules.md).
* [If you connect to the Internet through a proxy server] winhttp proxy settings are properly configured on Veeam ONE Server.
* TLS 1.2 is enabled on Veeam ONE Server.


