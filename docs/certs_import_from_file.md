---
title: "Importing Certificate from PFX Files"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/certs_import_from_file.html"
last_updated: "3/6/2025"
product_version: "13.0.1.6168"
---

# Importing Certificate from PFX Files


You can import the following certificates in the PFX format:

* A TLS certificate used by your organization and signed by a CA.
* A self-signed TLS certificate generated with a third-party tool.

|  |
| --- |
| Note: |
| Consider the following:   * The TLS certificate must pass validation on Veeam ONE Server. Otherwise, you will not be able to import the TLS certificate. * If a PFX file contains a certificate chain, only the end entity certificate will be imported. |

To import a TLS certificate from a PFX file, do the following on the machine where Veeam ONE server component is installed:

1. Run the Veeam ONE Settings utility.

For more information, see [Veeam ONE Settings Utility](appendix.md).

1. In the Server section, open the Web API Certificate tab.
2. To import the certificate, click Import and browse the certificate file.

[![Security Certificate Settings](images/utility_certificate.webp)](images/utility_certificate.webp "Security Certificate Settings")


