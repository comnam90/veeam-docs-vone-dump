---
title: "Data Protection"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_data_protection.html"
last_updated: "10/13/2023"
product_version: "13.0.1.6168"
---

# Data Protection


Veeam ONE Client allows you to track jobs and policies configured to protect the following workloads:

* [Virtual Machines](backup_jobs.md)
* [Computers](agent_jobs.md)
* [Unstructured Data](file_jobs.md)
* [Databases](protected_data_databases.md)
* [Networks](protected_data_networks.md)

By analyzing job details, you can reveal potential problems with the efficiency of data protection operations.

For example, if job duration has significantly increased in comparison with the average monthly duration value, while there are no noticeable changes to the amount of transferred data, you may need to investigate the root cause. Such a behavior may evidence that the job has to wait for proxy resources, which increases the backup window.


