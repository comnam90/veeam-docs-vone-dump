---
title: "Scheduling Script Examples"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/appendix_scheduling_scripts.html"
last_updated: "2/26/2025"
product_version: "13.0.1.6168"
---

# Scheduling Script Examples


To facilitate the process of dashboards and report creation, you can schedule automatic delivery of dashboards and reports. As one of the delivery options, you can save created dashboards and reports to a disk or network share. To learn about scheduling dashboards and reports, see [Scheduling Dashboards](schedule_dashboards.md) and [Scheduling Reports](schedule_reports.md).

If you need to perform further manipulations with the saved files, you can configure Veeam ONE Web Client to run a custom script after reports and dashboards are saved to the target folder. Veeam ONE Web Client allows you to use .BAT, .CMD, .VBS, .JS, .WSF, .EXE, .VBE, .JSE, .WSH or .PS1 scripts.

You can pass the following parameters to post-delivery scripts:

Scheduling Script Examples

| Parameter | Description |
| %ReportName% | Name of the generated report. |
| %ReportFolder% | Target folder to which created reports are saved (as specified in the Path field). |
| %DashboardName% | Name of the generated dashboard. |
| %JobName% | Name of the scheduling job that generates reports. |
| “-hidden” | Defines whether it is necessary to open created .VMR reports with the Veeam Report Viewer. If the parameter is specified, the reports will not be opened. |

This section explains how to use post-delivery scripts and contains simple script examples.

* [Example A. Copying a Report to Network Shares](script_example_a.md)
* [Example B. Sorting Reports by Name](script_example_b.md)


