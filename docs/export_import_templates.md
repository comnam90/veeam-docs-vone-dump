---
title: "Exporting and Importing Reports"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/export_import_templates.html"
last_updated: "9/23/2025"
product_version: "13.0.1.6168"
---

# Exporting and Importing Reports


You can export saved reports to a JSON file and import reports from a JSON file. Exporting and importing can be useful if you need to back up custom-designed reports, or if you want to copy saved reports from one Veeam ONE deployment to another.

|  |
| --- |
| Note |
| Reports cannot be imported into folders with reports saved from Veeam Backup & Replication. For details, see [Veeam Backup & Replication Web UI](https://helpcenter.veeam.com/docs/vbr/userguide/vbr_web_console.html?ver=13) and [Configuring Analytics View](https://helpcenter.veeam.com/docs/vbr/userguide/configure_analytics.html?ver=13). |

Exporting Reports

To export saved user report to a JSON file:

1. Open Veeam ONE Web Client.
2. Open the Saved Reports tab.
3. In the displayed list of reports, right-click a saved report which you want to export.
4. At the top of the report parameters, select Export parameters in the context menu.

The selected report will be exported to a JSON file and saved to the download location on your machine.

Exporting Report Folders

To export report folders to a JSON file:

1. Open Veeam ONE Web Client.
2. Open the Saved Reports tab.
3. In the report screen, under My reports, select the necessary folder or report.
4. At the top of the hierarchy, right-click the necessary folder and select Export parameters in the context menu.
5. In the displayed window, click Close.

The selected folder and all contained objects will be exported to a JSON file and saved to the download location on your machine.

Importing Reports

To import saved user reports from a JSON file:

1. Open Veeam ONE Web Client.
2. Open the Saved Reports tab.
3. In the report screen, select the necessary folder or report.
4. At the top of the hierarchy, right-click the necessary folder and select Import parameters in the context menu.
5. In the Windows Open dialog box, select the JSON file that describes saved user reports, and click Open.
6. In the displayed window, click Close.

Reports from the JSON file will be installed to the selected folder.


