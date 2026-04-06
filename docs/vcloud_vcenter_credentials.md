---
title: "Step 5. Specify Credentials for Underlying vCenter Servers"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vcloud_vcenter_credentials.html"
last_updated: "7/4/2025"
product_version: "13.0.1.6168"
---

# Step 5. Specify Credentials for Underlying vCenter Servers


At the vCenter Credentials step of the wizard, specify credentials for each vCenter Server attached to VMware Cloud Director. By default, Veeam ONE uses the same credentials that you have specified at the [Credentials](vcloud_server_credentials.md) step of the wizard. However, if the underlying vCenter Servers must be connected under another user account, you can set the credentials for each vCenter Server manually:

1. Select the necessary vCenter Server in the list.
2. Click Set User and specify credentials to connect to the vCenter Server.
3. Repeat steps 1-2 for all vCenter Servers attached to VMware Cloud Director.
4. To test if connection settings are configured correctly, click the Check Connection button. Veeam ONE will attempt to establish connection with the vCenter Servers using the provided credentials.


