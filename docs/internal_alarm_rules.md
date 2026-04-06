---
title: "Rules for Internal Alarms"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/internal_alarm_rules.html"
last_updated: "10/31/2025"
product_version: "13.0.1.6168"
---

# Rules for Internal Alarms


Veeam ONE offers the following types of rules for internal alarms:

Rules for Internal Alarms

| Rule Type | Description |
| Audit log free space | An alarm is triggered if free disk space allocated to an audit log is below or beyond a specific value (for example, if free space is below 15%). |
| Database cleanup queue growth | An alarm is triggered when object information is deleted faster than the Veeam ONE server can process. |
| Event-based rule | An alarm is triggered if some Veeam Backup & Replication event is generated for the Veeam Backup Enterprise Manager. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Resource usage | An alarm is triggered if the specified counter is above or below the specified threshold value (for example, if CPU usage exceeds 90%). |
| Staging data processing state | An alarm is triggered if the age of the oldest staging data file reaches the specified value. |
| Recon Scanner threat detection | An alarm is triggered if Recon Scanner raises an alert based on one or more suspicious behaviors. |
| Veeam ONE Web Client task state | An alarm is triggered if Veeam ONE Web Client task state is equal or not equal to a specific state value (Failed, Warning, Success). |


