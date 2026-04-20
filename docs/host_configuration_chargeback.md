---
title: "Host Configuration Chargeback"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/host_configuration_chargeback.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Host Configuration Chargeback


This report helps to make infrastructure costs audit and identify the most and least expensive VMs based on the hardware price and VM configuration.

The report analyzes hardware CPU, memory, storage capacities and their cost to calculate the cost of resources allocated to VMs. The cost of resources allocated to a VM is calculated based on VM configuration: the amount of vCPU, vRAM and storage resources provisioned to a VM.

|  |
| --- |
| Note: |
| * For VMs with thin-provisioned or dynamic disks, the report takes into account the amount of provisioned disk space, not actually used disk space. * For VMs with dynamic memory, the report takes into account the amount of allocated memory. |

* The Summary section includes the following elements:

+ Number of hosts, datastores and VMs, average costs of physical and virtual resources (processor core, virtual CPU, memory GB, storage TB), and total hardware cost.

+ The Cost Distribution chart shows the cost of hardware CPU, memory and storage resources.
+ The VM Power Status chart shows the number of running and powered-off VMs.
+ The Top 10 Most Expensive VMs subsection shows the most expensive VMs in terms of consumed resources, and provides cost of average CPU, memory and storage resources used by each VM. This chart is available if you choose to include VM details in the report.

* The Details tables provide information on physical CPU, memory and storage capacities, amount of provisioned vCPU, vRAM and storage resources, and the cost of these resources. If you choose to show VM cost details in the report parameters, the report also provides analysis of VM configuration cost in terms of vCPU, vRAM, storage and the total VM cost.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of virtual infrastructure level and its sub-components to analyze in the report.

* Currency: defines a payment currency.
* Calculate host costs based on: defines how host costs will be calculated in the report. You can select one of the following options:

+ Total host cost — defines the total cost of CPU and memory hardware resources for all hosts included in the report, in the selected currency.
+ Individual host costs — defines the hardware cost of each host separately.

To edit host costs:

1. Click Configure.
2. In the Configure Individual Host Costs window, select the necessary host and click Edit.
3. In the Set Individual Host Cost window, specify the desired cost and click Save.
4. Repeat steps 2–3 for each host cost you want to edit.

* CPU/RAM slider: defines the percentage of cost, or cost share of CPU and memory hardware resources for all hosts included in the report. For example, if the cost of CPU hardware resources make a quarter of the total cost, set the CPU parameter value to 25%. The RAM parameter value will adjust automatically.

* Calculate datastore costs based on: defines how datastore costs will be calculated in the report. You can select one of the following options:

+ Exclude datastores from the calculation — defines to exclude datastores cost details from the report.
+ Total datastore cost — defines the total cost of storage resources in the selected currency.
+ Individual datastore costs — defines the cost of each datastore separately.

To edit datastore costs:

1. Click Configure.
2. In the Configure Individual Datastore Costs window, select the necessary datastore and click Edit.
3. In the Set Individual Datastore Cost window, specify the desired cost and click Save.
4. Repeat steps 2–3 for each datastore cost you want to edit.

* Calculate VM storage hosts based on: defines how VM storage host must be calculated in the report (Provisioned space, Used space).
* Include powered-off VMs in the calculation: defines whether powered-off VMs must be analyzed in the report.
* Show VM details: defines whether the report must include VM cost details.

If this option is enabled, the report will include the Top 10 Most Expensive VMs section and a table that details VMs cost based on VM configuration.

|  |
| --- |
| Note: |
| Building the report may take some time if the chosen reporting period is significant, or if you choose to calculate VM cost for a large virtual infrastructure. |

[View Report Example](./reports/Host%20Configuration%20Chargeback.pdf)

Use Case

IT departments can use the report as a showback instrument to raise awareness within organization and demonstrate costs associated with provisioning VMs. The report helps calculate a budget share of allocated virtual infrastructure resources for each application owner, department or business unit within an organization, justify IT budget and assess the amount of future funding requests.

In combination with Veeam ONE optimization reports, this report can be used to encourage application owners to right size their VMs, prevent VM proliferation and reclaim wasted resources.

Service providers that do not have flat fees on virtual infrastructure resources can use this report as a chargeback instrument to calculate the cost of virtual infrastructure resources allocated to their clients.


