---
title: "Configuring Multi-Factor Authentication"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/users_mfa.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Configuring Multi-Factor Authentication


Multi-factor authentication (MFA) provides an additional layer of security for Veeam ONE user accounts. When MFA is enabled, users confirm their identity with a one-time password (OTP) generated in a mobile authenticator application, in addition to their user name and password. On the Multi-Factor Authentication tab of the Access Management section, you can enable or disable MFA for all users, enable or disable MFA for individual users, and reset MFA for a user.

MFA applies when users log in to Veeam ONE through both Veeam ONE Web Client and Veeam ONE Client. For details, see [Accessing Veeam ONE Components](access.md).

Required Permissions

To configure MFA, a user must have the Veeam ONE Administrator role. For details on user roles, see [Security](credentials_manager.md).

Enabling or Disabling MFA for All Users

To enable or disable multi-factor authentication for all Veeam ONE users:

1. Open Veeam ONE Web Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the top right corner of the Veeam ONE Web Client window, click Configuration.
2. In the configuration menu on the left, click Access Management.
3. On the Multi-Factor Authentication tab at the top of the user list, click Configuration.
4. In the MFA Configuration window, set the Multi-factor authentication (MFA) toggle to enable or disable MFA for all users.
5. Click OK.

|  |
| --- |
| Note |
| When you enable MFA for all users, each user is prompted to set up MFA in a TOTP authenticator application at the next login. |

Enabling or Disabling MFA for Individual Users

The MFA status you set for an individual user overrides the global MFA setting. For example, if MFA is enabled for all users, you can disable it for a specific user so that this user can log in without MFA.

To enable or disable multi-factor authentication for an individual user:

1. Open Veeam ONE Web Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the top right corner of the Veeam ONE Web Client window, click Configuration.
2. In the configuration menu on the left, click Access Management.
3. On the Multi-Factor Authentication tab, select the user whose MFA status you want to change.
4. At the top of the user list, click Enable or Disable.
5. Click Confirm.

Resetting MFA

If the user can no longer pass multi-factor authentication — for example, the user lost access to the authenticator app or replaced the device — you can reset MFA for this user.

To reset multi-factor authentication for a user:

1. Open Veeam ONE Web Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the top right corner of the Veeam ONE Web Client window, click Configuration.
2. In the configuration menu on the left, click Access Management.
3. On the Multi-Factor Authentication tab, select the user whose MFA you want to reset.
4. At the top of the user list, click Reset.
5. Click OK.

After you reset MFA, the current MFA setup for the user is cleared. At the next login, the user is prompted to set up MFA again.

[![MFA configuration](images/mfa_configuration.webp)](images/mfa_configuration.webp "MFA configuration")

Page updated 2026-07-13

