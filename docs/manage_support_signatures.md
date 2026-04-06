---
title: "Managing Signatures"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/manage_support_signatures.html"
last_updated: "9/18/2025"
product_version: "13.0.1.6168"
---

# Managing Signatures


If automatic signature update is enabled, and Veeam ONE server is connected to the Internet, it will connect to the Veeam Technical Support web server and update signatures automatically on a daily basis.

For details on enabling automatic signature update, see [Other Settings](other_settings_server.md).

Alternatively, you can manually check for an available update of signatures or import signatures from file provided by Veeam Technical Support.

Updating Signatures

To update diagnostic signatures:

1. Open Veeam ONE Web Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the top right corner of the Veeam ONE Web Client window, click Configuration.
2. In the configuration menu on the left, click Data Collection.
3. Click Update Signatures in the Veeam Intelligent Diagnostics drop-down list.

Veeam ONE Web Client will connect to Veeam Technical Support server over the Internet, check if an update is available, and download the latest version of signatures.

Importing Signatures

If Veeam ONE Client server has no Internet connection, you can manually import the file with the latest version of signatures:

1. Obtain the .package file from [Veeam website](https://www.veeam.com/intelligent-diagnostics-signatures-download.html).
2. Open Veeam ONE Web Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the top right corner of the Veeam ONE Web Client window, click Configuration.
2. In the configuration menu on the left, click Data Collection.
3. Click Import Signatures in the Veeam Intelligent Diagnostics drop-down list.
4. Specify a path to the .package file downloaded from Veeam website and click Import.


