---
title: "Alarm Assignment Options"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/assignment_options.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Alarm Assignment Options


You can assign Veeam ONE alarms to objects of the backup or virtual infrastructure. There are several options to assign alarms:

* Object-level assignment — you can assign an alarm to a single object.

This type of assignment can be useful if you need to customize alarms for specific objects, like separate hosts, VMs or backup infrastructure components.

* Group-level assignment — you can assign an alarm to a group of objects (for example, to an infrastructure container or Business View group).

This type of assignment can be useful if you need to assign an alarm to all objects under a specific parent entity. For example, to all VMs residing on a host or to all backup proxies connected to a backup server.

* Infrastructure-level assignment — you can assign an alarm to all objects of a particular type in the entire managed environment.

This is the default type of assignment used for all predefined alarms.

You can combine various assignment options. For example, you can assign an alarm to all VMs running on a chosen host, to all VMs in a Business View group and to a few single VMs at the same time.

In addition to flexible alarm assignment options, Veeam ONE offers a possibility to exclude specific objects or object groups from the assignment scope. Thus, you can easily point out what part of your environment the alarm must ignore.

Page updated 2026-08-05

