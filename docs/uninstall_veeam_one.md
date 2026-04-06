---
title: "Uninstalling Veeam ONE"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/uninstall_veeam_one.html"
last_updated: "9/2/2025"
product_version: "13.0.1.6168"
---

# Uninstalling Veeam ONE


To uninstall Veeam ONE, open the Start menu, go to Control Panel > Uninstall a program, choose Veeam ONE components you want to uninstall and click Remove.

[![Uninstalling Veeam ONE](images/uninstalling_veeam_one.webp)](images/uninstalling_veeam_one.webp "Uninstalling Veeam ONE")

If you installed Veeam ONE using the custom installation, repeat this procedure on every machine where the Veeam ONE components are installed.

The SQL Server instance installed and used by Veeam ONE is not removed during the uninstall of Veeam ONE. It needs to be removed separately using the standard Add or Remove Programs feature in Control Panel. Veeam ONE database and its data is retained until you manually remove the database or uninstall the SQL Server instance.


