---
title: "Advanced Alarm Options"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/advanced_options.html"
last_updated: "2/3/2025"
product_version: "13.0.1.6168"
---

# Advanced Alarm Options


To avoid alarm storms and ensure that critical issues are not overlooked, you can use advanced alarm configuration options — alarm suppression and alarm modeling.

* Alarm suppression is used to disregard events and prevent sending alarms when specific activities are performed. For example, during backup Veeam ONE may send a great number of alarms informing about potential problems or increased resource pressure. Alarm suppressing allows you to pause specific alarms during such activities, or at a specific period of time when you plan to perform resource-consuming operations.
* Alarm modeling is used to verify the created alarm scheme and estimate the need for adjusting alarm settings. During alarm modeling, Veeam ONE applies alarm settings to collected historical data and produces a forecast on the number of alarms that will be sent over a specific period of time. If the number of alarms is too high, alarm thresholds may need to be changed to avoid numerous useless alarms. If the number is too low, the sensitivity of alarms may need to be increased so that you do not miss important issues.

Related Topics

* [Suppressing Alarms](suppress_alarms.md)
* [Modeling Alarm Number](model_alarms.md)


