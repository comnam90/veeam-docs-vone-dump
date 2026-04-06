---
title: "License Usage Statistics"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/automatic_usage_logging.html"
last_updated: "8/7/2025"
product_version: "13.0.1.6168"
---

# License Usage Statistics


If you have enabled automatic update of Veeam ONE license, Veeam ONE will collect and send data on license usage automatically by default. For details on how to enable automatic license update, see [Updating License](update_license.md).

As part of this process, Veeam ONE collects statistics on the current license usage and sends it periodically to the Veeam License Update Server. The collected data provides information about the contract ID, license ID, product installation ID, and the maximum number of protected workloads managed by Veeam Backup & Replication over the past week (high watermark), the maximum number of Veeam backup agents managed in Veeam ONE, and the maximum number of workloads protected by other Veeam products integrated with Veeam ONE. The process runs in the background mode, once a week at a random time and day. For details on Veeam products that can be integrated with Veeam ONE, see [About Veeam ONE](about_one.md).

The collected data does not include information on Veeam ONE usage by any individual person identifiable for Veeam, or any data gathered by Veeam ONE.

Veeam may also use collected data for any other internal business purposes it deems appropriate, including (but not limited to) evaluation, improvement and optimization of Veeam licensing models.

|  |
| --- |
| Important! |
| Even after you have enabled automatic license update and Veeam ONE has started sending usage statistics, you are still required to submit license usage to your aggregator. For details, see [Submitting License Usage Report](submit_license_usage_report.md). |

Veeam may also use collected data for any other internal business purposes it deems appropriate, including (but not limited to) evaluation, improvement and optimization of Veeam licensing models. For details on license limits, see [Exceeding License Limit](license_expiry_grace_period.md).

By enabling license auto update you agree with collection, transmission and use of the reporting data. You must not enable license auto update in case you do not agree with such collection, transmission and use.


