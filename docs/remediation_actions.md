---
title: "Alarm Remediation Actions"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/remediation_actions.html"
last_updated: "12/17/2024"
product_version: "13.0.1.6168"
---

# Alarm Remediation Actions


To automate virtual and backup infrastructure troubleshooting, you can configure Veeam ONE to run remediation actions as soon as alarms are triggered.

|  |
| --- |
| ![Alarm Remediation Actions](images/icon_note.webp) Note: |
| To run remediation actions for the backup infrastructure, you must have Veeam ONE agents installed on connected Veeam Backup & Replication servers. For details on installing and configuring Veeam ONE agents, see [Managing Veeam ONE Agents](manage_one_agents.md). |

Veeam ONE offers the following types of remediation for alarms:

* Predefined actions that are configured for the most commonly used out-of-the-box alarms. For each alarm severity level, Veeam ONE can run only one predefined action.

For the list of alarms with predefined remediation actions, see [Remediation Actions](appendix_remediation.md).

* Custom scripts that you can specify in the settings of any alarm. For each severity level, Veeam ONE can run one or more custom scripts.

You can select the resolution type for alarm remediation actions:

* Manual — when an alarm is triggered, you must approve the remediation action manually. This type of resolution is default for alarms with predefined remediation actions.
* Automatic — when an alarm is triggered, Veeam ONE will automatically run a predefined remediation action or custom script.

Veeam ONE makes 3 attempts to run a remediation action or script. If the remediation is successful, the alarm status will change to Acknowledged. If for some reason Veeam ONE fails to run an action or script, the alarm will remain active.

Related Topics

[Approving Alarm Remediation Actions](remediate_alarms.md)


