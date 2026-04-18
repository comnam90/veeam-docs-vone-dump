---
title: "Idle Templates"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/idle_templates_vmware.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Idle Templates


Templates are preconfigured images of your VMs that help you to easily deploy multiple copies of the model VMs across the infrastructure.

* The Summary section shows the total number of templates, the number of idle templates and the amount of wasted storage space.
* The Details table provides information on inactive templates, including template location, size and the last time the template was used.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Allowed period of inactivity: defines the amount of time that the template must be inactive to be included in the report.

|  |
| --- |
| Note: |
| You can exclude specific datastores from this report. This can be useful when you are not interested in examining particular datastores for garbage files (for example, local datastores, datastores hosting ISO files or backups). In this case, you can exclude unnecessary datastores from the collection scope. For more information, see [Choosing Datastores to Report On](datastores_to_report.md). |

[View Report Example](./reports/Idle%20Templates.pdf)

Use Case

VM templates consume valuable storage resources. Use this report to review the list of your templates and identify templates that can be deleted or moved to less costly datastores to reclaim additional storage space.


