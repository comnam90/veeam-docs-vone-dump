---
title: "Step 10. Specify Connection Ports"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/advanced_choose_ports_web.html"
last_updated: "9/2/2025"
product_version: "13.0.1.6168"
---

# Step 10. Specify Connection Ports


At the Port Configuration step of the wizard, specify connection settings for Veeam ONE Web Client:

* In the Website port field, type a number of the port that will be used to access the Veeam ONE Web Client through a web browser.

The default port number is 1239.

* In the Certificate list, choose a certificate that will be used to secure traffic between the Veeam ONE Web Client and a web browser.

You can choose an existing certificate installed on the machine or select the setup wizard to generate a self-signed certificate.

|  |
| --- |
| Note: |
| * If you generate or choose a self-signed certificate, you must configure a trusted connection between the Veeam ONE Web Client and a web browser later. For details, see [Accessing Veeam ONE Components](access.md#configure_trusted). * You can change the selected certificate after installation. For details, see [Change Default Certificate](upgrade_change_certificate.md). |

[![Veeam ONE Specify WebUI Ports](images/advanced_webui_ports.webp)](images/advanced_webui_ports.webp "Veeam ONE Specify WebUI Ports")


