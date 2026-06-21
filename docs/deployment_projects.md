---
title: "Deployment Projects"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/deployment_projects.html"
last_updated: "6/19/2026"
product_version: "13.0.2.6723"
---

# Deployment Projects


Veeam ONE Web Client deployment projects allow you to predict future resource utilization and plan resource reservations in your virtual environment.

With deployment projects, you can run complex simulation tasks to predict the effects of:

* Adding or evicting hosts in a cluster

* Adding new VMs or decommissioning existing VMs

Deployment projects compare the projected resource capacities against the future resource demand, help identify potential resource shortages and provide practical recommendations that an administrator should undertake to succeed with the actual deployment.

For example, you can simulate how many VMs similar to an existing Microsoft SQL Server can be added in a cluster without the risk of causing resource contention or degraded cluster performance. Deployment projects can be helpful in assessing various hardware replacement scenarios or forecasting the amount of compute and storage resources that need to be provisioned.

|  |
| --- |
| Note: |
| Deployment projects are not available in Veeam ONE Community edition. |

Deployment Projects and Scenarios

Every deployment project includes a specific simulation scenario. A simulation scenario describes what amount of resources must be added to or evicted from the managed environment.

In simulation scenarios, you can:

* Select an existing host or a VM and use it as a baseline model to calculate the effects of adding or evicting resources
* Explicitly specify host or VM configuration

Simulation scenarios can be targeted at a host or cluster, termed container — a recipient node that will undergo the capacity changes and whose future performance and resource utilization will be assessed.

Condition for Acceptance

The deployment project is considered successful if future resource utilization and performance metrics do not breach the designated thresholds that define the maximum tolerable resource load. The thresholds are preset and can be customized if necessary.

Tentatively successful projects (projects completed with warnings) will cause the metrics to breach the thresholds but stay beyond 100 percent of resource utilization (for example, memory usage exceeding a 90 percent threshold but being less than 100 percent).

Calculation Background

Resource availability and performance modelling is based on comparing future demand for resources against the projected resource capacity. The following factors are used in the analysis:

* Current compute capacities
* Additional capacities introduced through adding new hosts or evicting VMs
* Withdrawn compute capacities through evicting hosts
* Extra capacities required to run new VMs

The following algorithms are employed to forecast workloads:

* When a new VM is added, it is assumed that the VM will use all its provisioned resources.
* When an existing VM is selected as a baseline model, Veeam ONE will use the average value of the VM resource consumption during the current week.
* When calculating the amount of free space, Veeam ONE verifies that there is sufficient storage capacity for all virtual disks of the VM.

Deployment Project Interdependencies

You can create several simulation scenarios that describe complex conditions, such as introducing new and decommissioning existing hosts or VMs in the same container, at the same time. You can also create deployment scenarios with overlapping due dates.

When you create a new deployment project or make changes in the existing deployment project, Veeam ONE checks if there is any overlapping project. If there are changes that may affect the concurrent project, Veeam ONE Web Client will prompt you to recalculate the overlapping projects.


