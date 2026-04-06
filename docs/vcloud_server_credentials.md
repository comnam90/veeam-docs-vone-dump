---
title: "Step 4. Specify Credentials for VMware Cloud Director"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vcloud_server_credentials.html"
last_updated: "9/30/2025"
product_version: "13.0.1.6168"
---

# Step 4. Specify Credentials for VMware Cloud Director


At the Credentials step of the wizard, click Add credentials and specify credentials of the user account for connecting to VMware Cloud Director. For details on adding credentials records, see [Security](credentials_manager.md).

[![Click the image to zoom in](images/connect_vcloud_provide_credentials.webp)](images/connect_vcloud_provide_credentials.webp "Click the image to zoom in")

1. When you add a VMware Cloud Director host, Veeam ONE saves to the configuration database a thumbprint of the TLS certificate installed on the VMware Cloud Director host and all vCenter servers under it. During every subsequent connection to the server, Veeam ONE uses the saved thumbprint to verify the server identity and avoid the man-in-the-middle attack.

If the certificate installed on the server is not trusted, Veeam ONE displays a warning.

+ To view detailed information about the certificate, click View Certificate.

+ If you trust the server, click Trust and Continue.

+ If you do not trust the server, click Cancel. Veeam ONE will display an error message, and you will not be able to connect to the server.


