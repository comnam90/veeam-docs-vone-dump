---
title: "Capacity Planning for Backup Repositories"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/capacity_planning_for_repositories.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Capacity Planning for Backup Repositories


This report estimates the amount of free space available on backup repositories and forecasts how many days remain before a repository will run out of available storage capacity.

Backup repositories tend to run out of free space when outdated restore points overload the datastore. This report helps you ensure there is enough space for your backup data at any point in time. The report also provides recommendations on how to adjust the allocated storage resources to meet the future demand for backup storage. Furthermore, it calculates the amount of additional space that needs to be provisioned to accommodate the necessary restore points.

To calculate future repository performance, the report analyzes historical performance data for the selected time period, calculates the performance utilization trend and applies this trend to the safety interval (that is, the selected number of days during which the specified threshold should not be breached). This helps you rationally plan your resources.

* The Summary display provides an overview of the backup infrastructure (the total number of repositories, jobs and stored computers, VMs and file shares), shows repositories capacity, the amount of free space, the utilization ratio, the number of days left before specified thresholds will be reached, and the amount of space required to sustain the current workloads without exceeding the specified thresholds.

+ The Top 5 Utilized Repositories and Top 5 Repositories by Days Left charts display 5 repositories that will run out of free space sooner than other repositories and the number of days left before space usage level on these repositories breaches the specified threshold. Additionally, each each repository configured for the report has its own accompanying virtual chart.

* The Report Data display provides the Details and Backup Repository Free Space Usage tables displaying information on the total repository capacity, number of VMs, computers, file shares, applications and object storage data in backups stored on the repository and the number of days left before the repository runs out free space.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of backup repositories to analyze in the report.
* Space utilization threshold: defines the maximum amount of used space measured as a percentage of total capacity on the available repositories.
* Free space (min) threshold: defines the minimum total amount of free space on the repositories.

* Safety interval: defines the safety interval (that is, the required minimum number of days during which the specified space threshold should not be breached).

* Analyze performance data for: defines the time period to analyze in the report.

[View Report Example](./reports/Capacity%20Planning%20for%20Backup%20Repositories.pdf)

Use Case

The report allows you to analyze configuration and space usage on backup repositories and to forecast how many days remain before the repository reaches its full capacity. You can use the report to assess the required amount of additional space that needs to be allocated to support the uninterrupted backup operations for a specified number of days into the future.


