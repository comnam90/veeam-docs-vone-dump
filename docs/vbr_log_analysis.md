---
title: "Performing Log Analysis"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vbr_log_analysis.html"
last_updated: "9/30/2025"
product_version: "13.0.1.6168"
---

# Performing Log Analysis


Veeam Intelligent Diagnostics is a feature that allows you to automatically detect known issues in configuration and performance of backup infrastructure.

To use Veeam Intelligent Diagnostics:

1. Open Veeam ONE Web Client.
2. At the top right corner of the Veeam ONE Web Client window, click Configuration.
3. In the configuration menu on the left, click Data Collection.
4. In the inventory pane, select the desired object in the Object Name column.
5. In the Veeam Intelligent Diagnostics drop-down list specify the diagnostic actions:

* Click Start log analysis to start analysis.
* Click Stop log analysis to stop analysis.
* Click Schedule to schedule a start time for log analysis.

For details on Veeam Intelligent Diagnostics, see [Veeam Intelligent Diagnostics](intelligent_diagnostics.md).

Veeam Analytics service allows you to perform log analysis according to the defined schedule or manually:

* When a scheduled log analysis session starts, Veeam Analytics service analyzes Veeam Backup & Replication logs for the last 48 hours or since the last successful log analysis session (whichever is later).

By default, Veeam Analytics service is set to perform log analysis daily at 7:00 AM. To change the default log analysis schedule, see [Scheduling Automated Log Analysis](vbr_log_analysis.md#schedule).

* When you start a log analysis session manually, Veeam Analytics service analyzes Veeam Backup & Replication logs for the last 24 hours or since the last successful log analysis session (whichever is later).

For details on starting log analysis manually, see [Starting Log Analysis Manually](vbr_log_analysis.md#manual).

|  |
| --- |
| Note: |
| If silence mode is active for the target Veeam Backup & Replication server, log analysis cannot be run manually or by schedule. |

Scheduling Automated Log Analysis

To set up daily schedule for automated log analysis:

1. Open Veeam ONE Web Client.
2. At the top right corner of the Veeam ONE Web Client window, click Configuration.
3. In the configuration menu on the left, click Data Collection.
4. In the inventory pane, select the desired object from the list of Veeam Backup & Replication servers with installed Veeam Analytics service in the Object Name column.
5. In the Veeam Intelligent Diagnostics drop-down list click Schedule.
6. In the Log Analysis Schedule window, specify the time at which log analysis must start daily.
7. Click Save.

Starting Log Analysis Manually

1. Open Veeam ONE Web Client.
2. At the top right corner of the Veeam ONE Web Client window, click Configuration.
3. In the configuration menu on the left, click Data Collection.
4. In the inventory pane, select the desired object from the list of Veeam Backup & Replication servers with installed Veeam Analytics service in the Object Name column.
5. In the Veeam Intelligent Diagnostics drop-down list click Start log analysis.

Stopping Log Analysis

You can stop a session, for example, if log analysis is about to take long, and you do not want to produce workload on the production environment during business hours.

To stop log analysis:

1. Open Veeam ONE Web Client.
2. At the top right corner of the Veeam ONE Web Client window, click Configuration.
3. In the configuration menu on the left, click Data Collection.
4. In the inventory pane, select the desired object from the list of Veeam Backup & Replication servers with installed Veeam Analytics service in the Object Name column.
5. In the Veeam Intelligent Diagnostics drop-down list click Stop log analysis.


