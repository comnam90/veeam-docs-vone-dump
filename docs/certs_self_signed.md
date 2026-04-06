---
title: "Generating Self-Signed Certificates"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/certs_self_signed.html"
last_updated: "3/6/2025"
product_version: "13.0.1.6168"
---

# Generating Self-Signed Certificates


To generate self-signed TLS certificates, Veeam ONE uses RSA algorithm with a 2048-bit key length and SHA-2 hashing algorithm. The created TLS certificate is saved to the Shared certificate store. The following types of users can access the generated TLS certificate:

* User who created the TLS certificate
* LocalSystem user account
* Local Administrators group

|  |
| --- |
| Note: |
| When you generate a self-signed TLS certificate with Veeam ONE, you cannot include several aliases to the certificate and specify a custom value in the Subject field. The Subject field value is taken from the Veeam ONE license installed on Veeam ONE Server. |

To generate a new self-signed TLS certificate, do the following:

1. Run the Veeam ONE Settings utility.

For more information, see [Veeam ONE Settings Utility](appendix.md).

1. In the Server section, open the Web API Certificate tab.
2. Click Generate.
3. To use a newly generated certificate, in the displayed window, click Yes.

[![Security Certificate Settings](images/utility_certificate.webp)](images/utility_certificate.webp "Security Certificate Settings")

|  |
| --- |
| Note: |
| If you replace the default certificate with another self-signed certificate, you must configure a trusted connection between the Veeam ONE Web Client and a web browser later. For details, see [Accessing Veeam ONE Components](access.md). |


