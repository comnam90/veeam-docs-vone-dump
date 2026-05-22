---
title: "Deployment Project Statuses"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/deployment_project_states.html"
last_updated: "5/19/2026"
product_version: "13.0.1.6168"
---

# Deployment Project Statuses


Veeam ONE deployment projects may have one of the following statuses.

* To be calculated

The status indicates that project calculation is pending. Remediation action is to calculate the project. For details, see [Calculating Deployment Projects](build_deployment_projects.md).

* To be recalculated

The status is assigned if the project settings have changed, or changes in a concurrent project affect the project. Remediation action is to calculate the project. For details, see [Calculating Deployment Projects](build_deployment_projects.md).

* Not passed

The status indicates that the project simulation has completed but the deployment cannot be executed successfully due to anticipated resource constraints.

The deployment simulation analysis has concluded that it is impossible to place the desired number of hosts or VMs without causing the future resource utilization to exceed 100 percent on any of the performance metrics.

Remediation action is to view the project report and change the project settings in accordance with the report recommendations. For details, see [Viewing Deployment Project Report](view_project_report.md) and [Modifying Deployment Projects](modify_deployment_projects.md).

* Passed with warnings

This status indicates that the deployment is feasible but will cause the resource utilization to breach the threshold values. However, the resource utilization will not reach 100 percent.

Remediation action is to view the project report and change the project settings in accordance with the report recommendations. For details, see [Viewing Deployment Project Report](view_project_report.md) and [Modifying Deployment Projects](modify_deployment_projects.md).

* Passed successfully

The status indicates that the project has completed successfully and its requirements are fully met. There are enough resources to accomplish the planned deployment and maintain an acceptable level of resource utilization.


