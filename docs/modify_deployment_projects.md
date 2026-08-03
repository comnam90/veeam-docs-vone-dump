---
title: "Modifying Deployment Projects"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/modify_deployment_projects.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Modifying Deployment Projects


You can modify settings of a deployment project that you have not completed yet. For example, you may need to update deployment project settings if the project was calculated with the Failed state.

To modify deployment project settings:

1. Open Veeam ONE Web Client.
2. Open the Deployment Projects section.
3. Select the necessary deployment project in the list and click Edit.
4. Change the deployment project settings as described in [Creating Deployment Projects](create_deployment_projects.md).
5. Save changes.

After you change project settings, you need to calculate the project anew. You may also need to recalculate overlapping or dependent projects. For example, if you change the project due date to an earlier date, Veeam ONE Web Client will offer you to recalculate all projects whose dates overlap with the changed project.

Page updated 2026-08-03

