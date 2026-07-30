---
title: "Configuring SNMP Traps"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/snmp_traps.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Configuring SNMP Traps


If you use SNMP to monitor applications and devices in the managed infrastructure, you can configure Veeam ONE to report about triggered alarms by means of SNMP traps. When SNMP trap notifications are enabled, Veeam ONE acts as an agent. It generates trap messages when an alarm is triggered, and sends them to SNMP receivers. SNMP receivers can then forward the traps to a management application.

Veeam ONE sends SNMP traps with the following information:

* Date and time the alarm was triggered
* Name of the affected node
* Old alarm status
* New alarm status
* Alarm name
* Alarm summary

Veeam ONE supports SNMP versions 1, 2, and 3. For version 3, Veeam ONE sends traps based on CISCO-SNMP-USM-OIDS-MIB that complies with [RFC 3414](https://datatracker.ietf.org/doc/html/rfc3414).

To configure SNMP traps, perform the following steps:

1. [Configure SNMP receivers and manager](configure_snmp_service.md).
2. [Configure SNMP settings in Veeam ONE](configure_snmp_settings.md).
3. [Change alarm action settings to enable SNMP traps for the necessary alarms](enable_snmp_notifications.md).

Page updated 2026-07-30

