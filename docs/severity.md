---
title: "Alarm Severity"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/severity.html"
last_updated: "7/8/2026"
product_version: "13.0.2.6723"
---

# Alarm Severity


Every alarm rule is associated with a specific severity level. The severity level defines how serious the state or event is and how badly it can affect an object health state.

There are four severity levels that are color-coded as follows:

* Error (red) indicates a critical situation or a major problem that requires immediate action.
* Warning (yellow) indicates a potential problem or non-critical issue that needs your attention. If the issue is left without attention, it can potentially cause a major problem.
* Resolved (green) indicates that the issue was eliminated because of the changed conditions, or shows that the alarm was resolved manually.
* Information (blue) indicates general information about a specific condition or health state of an object.

You can define different severity levels for conditions of different intensity. For example, if the level of memory usage must not exceed 75%, you can create the following alarm rules:

* If the memory usage is over 70%, an alarm with the Warning severity level must be triggered.
* If the memory usage is over 75%, an alarm with the Error severity level must be triggered.

In such situation, if the memory usage level is constantly growing and exceeds 70%, Veeam ONE will trigger a warning alarm, notifying about a potentially dangerous situation. If the memory usage level keeps on growing and exceeds the level of 75%, Veeam ONE will trigger an error alarm notifying about the severe danger.


