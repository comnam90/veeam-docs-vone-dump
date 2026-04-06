---
title: "Step 6. Review Connection Settings"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vcloud_server_review.html"
last_updated: "9/30/2025"
product_version: "13.0.1.6168"
---

# Step 6. Review Connection Settings


At the Summary step of the wizard, review the connection details and click Finish.

[![Click the image to zoom in](images/connect_vcloud_review.webp)](images/connect_vcloud_review.webp "Click the image to zoom in")

The VMware Cloud Director hierarchy will become available in the VMware Cloud Director view. Note that it may take a while for Veeam ONE to collect and display data for the newly added VMware Cloud Director and its child objects.

When you connect VMware Cloud Director, Veeam ONE also connects underlying vCenter Servers and initiates data import. vCenter Servers become available on the Data Collection Overview page and in the Infrastructure View, and you can work with them as with regular VMware vSphere infrastructure servers. If the vCenter Server attached to VMware Cloud Director is already connected, Veeam ONE will only create an association between the VMware Cloud Director hierarchy and the vCenter Server.


