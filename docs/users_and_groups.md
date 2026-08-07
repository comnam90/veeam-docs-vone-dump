---
title: "Managing Users and Groups"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/users_and_groups.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Managing Users and Groups


On the Users and Groups tab, you can manage Veeam ONE users and groups — assign roles and define the backup infrastructure scope.

Adding Users and Groups

To add a user or group to limit access to Veeam ONE:

1. Open Veeam ONE Web Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the top right corner of the Veeam ONE Web Client window, click Configuration.
2. In the configuration menu on the left, click Access Management.
3. On the Users and Groups tab, click Add to open the Add Access wizard.
4. At the User or Group step of the wizard:

* From the Identity provider list, select Local Users or a configured identity provider, such as Microsoft Entra ID, Okta, Keycloak, Microsoft ADFS or Custom.
* From the Type list, select User or Group.
* In the Name section, specify the name for the user or group.

[![Managing Users and Groups](images/add_access_user.webp)](images/add_access_user.webp)

1. At the Veeam ONE Role step of the wizard, select the Veeam ONE user role:

* Veeam ONE Administrator
* Veeam ONE Power User
* Veeam ONE Read-Only
* Veeam ONE Backup Administrator

For details on user roles, see [Security Groups](security_groups.md).

[![Managing Users and Groups](images/add_access_role.webp)](images/add_access_role.webp)

1. [Optional] At the Infrastructure Objects step of the wizard, select the backup infrastructure objects available to the user or group. This step applies only if you selected the Veeam ONE Backup Administrator role.

[![Managing Users and Groups](images/add_access_scope.webp)](images/add_access_scope.webp)

1. Review the configuration summary and click Finish.

[![Managing Users and Groups](images/add_access_summary.webp)](images/add_access_summary.webp)

Editing Users and Groups

To edit a user or group:

1. Open Veeam ONE Web Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the top right corner of the Veeam ONE Web Client window, click Configuration.
2. In the configuration menu on the left, click Access Management.
3. On the Users and Groups tab, select the user or group you want to edit, and click Edit.

The wizard opens with the settings you specified when adding the user or group. Edit them as required and click Finish.

Removing Users and Groups

If a user or group no longer needs access to Veeam ONE, you can remove its access entry. This revokes the assigned role but does not delete the user or group.

To remove a user or group:

1. Open Veeam ONE Web Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the top right corner of the Veeam ONE Web Client window, click Configuration.
2. In the configuration menu on the left, click Access Management.
3. On the Users & Groups tab, select the user or group you want to remove, and click Remove.
4. In the Remove Access window, click Confirm.

Enabling or Disabling Users and Groups

You can disable a user or group to temporarily revoke its access to Veeam ONE without removing the access entry. Disabling keeps the assigned role and settings, so you can enable the user or group again to restore access.

To enable or disable a user or group:

1. Open Veeam ONE Web Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the top right corner of the Veeam ONE Web Client window, click Configuration.
2. In the configuration menu on the left, click Access Management.
3. On the Users and Groups tab, select the user or group you want to enable or disable.

To find the necessary user or group, use the search box to search by name or the Type filter to narrow the list by user type.

1. At the top of the user list, click Enable or Disable.
2. In the confirmation window, click Confirm.

[![Users and groups configuration](images/Users_and_groups.webp)](images/Users_and_groups.webp "Users and groups configuration")

Page updated 2026-07-15

