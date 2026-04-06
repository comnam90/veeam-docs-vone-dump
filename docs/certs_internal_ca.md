---
title: "Using Certificate Signed by Internal CA"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/certs_internal_ca.html"
last_updated: "3/6/2025"
product_version: "13.0.1.6168"
---

# Using Certificate Signed by Internal CA


If you want to use a certificate signed by your own Certification Authority (CA), consider the following:

* Make sure that Veeam ONE server trusts the CA. That means that the Certification Authority certificate must be added to the Trusted Root Certification Authority store on the Veeam ONE server. Also, Certificate Revocation List (CRL) must be accessible from the Veeam ONE server.
* If you use Windows Server Certification Authority, issue a Veeam ONE certificate based on the built-in Subordinate Certification Authority template or templates similar to it. You can manage templates with the Certificate Templates MMC snap-in.

Veeam ONE Website Certificate Requirements

* The certificate subject is equal to the fully qualified domain name of the Veeam ONE server. For example: oneserver.domain.local.
* The Subject Alternative Name field contains the FQDN of the Veeam ONE server. For example: DNS:oneserver.domain.local.
* The minimum key size is 2048 bits.
* The key usage is Digital Signature, Non-Repudiation, Key Encipherment, Data Encipherment.
* The enhanced key usage is Server Authentication (1.3.6.1.5.5.7.3.1).

Veeam ONE Web API Certificate Requirements

* The certificate subject is equal to the fully qualified domain name of the Veeam ONE server. For example: oneserver.domain.local.
* The Subject Alternative Name field contains the FQDN of the Veeam ONE server. For example: DNS:oneserver.domain.local.
* The minimum key size is 2048 bits.
* The key usage is Digital Signature, Non-Repudiation.
* The enhanced key usage is Server Authentication (1.3.6.1.5.5.7.3.1).


