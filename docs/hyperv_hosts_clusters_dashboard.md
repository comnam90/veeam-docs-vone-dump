---
title: "Hyper-V Hosts and Clusters"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/hyperv_hosts_clusters_dashboard.html"
last_updated: "9/18/2025"
product_version: "13.0.1.6168"
---

# Hyper-V Hosts and Clusters


The Hyper-V Hosts and Clusters dashboard helps you evaluate host and cluster performance in the Microsoft Hyper-V infrastructure. The dashboard displays statistics on CPU, memory, disk and network utilization, and helps you identify hosts and clusters with performance issues.

You can access the Hyper-V Hosts and Clusters dashboard from the Dashboard tab in Veeam ONE Web Client.

[![Hyper-V Hosts and Clusters Dashboard](images/hyperv_hosts_clusters_dashboard.webp)](images/hyperv_hosts_clusters_dashboard.webp "Hyper-V Hosts and Clusters Dashboard")

Widgets Included

Memory Pressure by Cluster

This widget shows how the average memory pressure for all VMs on all hosts in the cluster has been changing during the week.

Network Usage by Cluster

This widget shows how the average rate at which bytes are transferred to and from the cluster disk during I/O operations has been changing during the week.

Disk Usage by Cluster

This widget shows how the average rate at which data is read from and written to the cluster disk has been changing during the week.

Top Hosts by CPU

This widget displays weekly CPU utilization data for the top 5 most loaded hosts in your infrastructure.

Arrows on the right show whether the average CPU usage value has changed over the previous week\*.

Top Hosts by Memory

This widget displays a list of hosts with the highest level of memory consumption.

Arrows on the right show whether the average memory usage value has changed over the previous week\*.

Top Hosts by Network

This widget displays a list of hosts with the highest level of network usage.

Arrows on the right show whether the average network throughput value has changed over the previous week\*.

\*The arrows allow you to compare the results of this week to the results of the previous week, and to track how the trend has evolved. For example, a grey arrow pointing right next to the CPU Usage value means that CPU utilization has not changed over the past week, a green arrow pointing down means that CPU utilization has decreased, while a red arrow pointing up means that CPU utilization has increased.


