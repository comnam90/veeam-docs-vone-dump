---
title: "Step 6. Configure Syslog Integration"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/notification_config_syslog_integration.html"
last_updated: "11/13/2025"
product_version: "13.0.1.6168"
---

# Step 6. Configure Syslog Integration


Syslog integration allows you to send pre-built Veeam ONE alarms and data for audit events for reuse within your Syslog server environment.

At the Syslog step of the wizard, specify your Syslog settings used to return alarms to your Syslog instance.

To specify your Syslog integration details:

1. Click the Enable syslog check box.
2. Enter Syslog server details::

* Syslog server — define the IPv4 or IPv6 address of your Syslog instance.
* Syslog facility — define the value used to identify the source of the alarm. By default this is set to mail.
* Syslog transport — define TCP, TCP with TLS, or UDP. By default this is UDP.
* Syslog server port — the port used to connect to your Syslog integration instance. By default this is 514.

1. Select your required Syslog audit events to send to your Syslog integration:

* Access to data
* Changes to data
* Privileged activities
* Login sessions

1. To test the connection settings, click Test syslog integration. This creates a test connection to Syslog and returns a signal confirming a successful connection.

If you select the Enable syslog check box and do not test the connection, Veeam ONE will verify it before saving the notification settings. Additionally, the connection is checked when each Notification Settings item (Mail Server Settings, Email Notifications and so on) changes.

[![Syslog settings](images/syslog_settings.webp)](images/syslog_settings.webp "Syslog settings")

For details on alarm notification settings, see [Configuring Alarm Notifications](configure_alarm_notification.md).


