---
title: "License Types and Packages"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/license_types.html"
last_updated: "3/23/2026"
product_version: "13.0.1.6168"
---

# License Types and Packages


Veeam Software offers paid and free licenses for Veeam ONE.

Paid Licenses

Veeam Software offers the following types of paid licenses for Veeam ONE:

* Perpetual license is a permanent full license. The perpetual license does not have an expiration date and allows using Veeam ONE versions issued before support expiration date.

* Subscription license is a full license that expires at the end of the subscription term. The subscription license term is normally 1–3 years from the license issue date.

* Rental license is a full license intended for Veeam Cloud & Service Providers (VCSP). The license expiration date is set according to the chosen rental program (normally 1–12 months from the license issue date).

For details on Veeam ONE licensing for Veeam Cloud & Service Providers (VCSP), see section [Veeam ONE](https://helpcenter.veeam.com/docs/vcsp/refguide/veeam_one.html) of the Veeam Rental Licensing and Usage Reporting Guide.

The following terms apply to Veeam ONE paid licenses:

Paid Licenses

| License Type | Licensing |
| Perpetual license | Per socket/Per instance |
| Subscription license | Per socket/Per instance |
| Rental license | Per point |

Free Licenses

Veeam Software offers the following types of free licenses for Veeam ONE:

* Evaluation license is a full license that can be used for product evaluation. The trial license is valid for 30 days from the moment of product download.
* Community Edition license is a license with a limited set of features\* but with no restrictions on the number of virtualization hosts, management servers and failover clusters you can monitor and report on. The community license includes 10 Veeam Backup & Replication monitored instances free of charge and does not have an expiration date. The community version does not require a license file during installation.
* NFR license is a full license that can be used for product demonstration, training and education. This license is not for resale or commercial use.

\*For details on Veeam ONE Community Edition limitations, see [Feature Comparison](https://www.veeam.com/products-edition-comparison.html?ad=in-text-link#ONE).

License Packages

Veeam ONE accepts licenses of the following packages:

* ONE
* Essentials
* Suite
* Advanced
* Premium

|  |
| --- |
| Note: |
| The Suite package matches Veeam Data Platform Advanced from the Pricing and Packaging page. |

For details on license packages, see [Pricing and Packaging](https://www.veeam.com/backup-solution-pricing.html).

Compatibility with Veeam Backup & Replication Licenses

Veeam ONE allows monitoring of Veeam Backup & Replication servers if the following conditions are met for Subscription and Perpetual licenses:

Compatibility with Veeam Backup & Replication Licenses

|  | | | Veeam ONE License | | |
| Per Socket | Per Instance | |
| Package = Suite / Essentials / Advanced / Premium | Package = ONE |
| Veeam Backup & Replication License | Per Socket | Package = Backup / Foundation | All workloads[1](#1) | All workloads | All workloads |
| Package = Suite / Essentials / Advanced / Premium | All workloads[1](#1) | All workloads | All workloads |
| Per Instance | Package = Backup / Foundation | Cannot add to Veeam ONE | Cannot add to Veeam ONE | Cannot add to Veeam ONE |
| Package = Suite / Essentials / Advanced / Premium | All workloads[2](#2) | All workloads | Cannot add to Veeam ONE |
| Merged | Sockets (Package = Backup / Foundation)  Instances (Package = Backup / Foundation) | VM workloads only | Cannot add to Veeam ONE | All workloads |
| Sockets (Package = Suite / Essentials / Advanced / Premium)  Instances (Package = Backup / Foundation) | VM workloads only | VM workloads only | All workloads |
| Sockets (Package = Backup / Foundation)  Instances (Package = Suite / Essentials / Advanced / Premium) | All workloads[2](#2) | Non-VM workloads only | All workloads |
| Sockets (Package = Suite / Essentials / Advanced / Premium)  Instances (Package = Suite / Essentials / Advanced / Premium) | All workloads[2](#2) | All workloads | All workloads |

where:

* VM workloads only — include VMs protected by the monitored Veeam Backup & Replication servers and VMs included in the monitoring and reporting scope with Veeam ONE inclusion rules.
* Non-VM workloads only — include other workloads protected by Veeam Backup & Replication servers that you connect to Veeam ONE: computers protected with Veeam Agent for Windows, Veeam Agent for Linux, Veeam Agent for Mac, Veeam Agent for IBM AIX, Veeam Agent for Oracle Solaris, file shares, Nutanix AHV VMs, Microsoft Azure VMs, AWS EC2 instances and Google Cloud Platform VMs.

1. Includes free instances that can be used for monitoring non-VM workloads.
2. Veeam ONE does not consume free instances included in the license file.

|  |
| --- |
| Note: |
| Veeam ONE does not accept merged license files. If you install a merged socket and instance license, it behaves as a per socket license. |

Compatibility with Veeam Backup for Microsoft 365 Licenses

Veeam ONE allows monitoring of Veeam Backup for Microsoft 365 servers if the following conditions are met for the licenses:

Compatibility with Veeam Backup for Microsoft 365 Licenses

|  | | | Veeam ONE License | | | | | |
| Rental | Subscription | Perpetual | Community | NFR | Evaluation |
| Veeam Backup for Microsoft 365 License | Subscription | Package = M365 | ✕ | ✕ | ✕ | ✕ | ✕ | ✓ |
| Package = M365Suite | ✓ | ✓ | ✓ | ✓ | ✕ | ✓ |
| Rental | Package = M365 | ✓ | ✕ | ✕ | ✕ | ✕ | ✓ |
| Evaluation | Package = M365Suite | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Community | Package = M365Suite | ✕ | ✓ | ✓ | ✕ | ✓ | ✓ |
| NFR | Package = M365 | ✕ | ✕ | ✕ | ✕ | ✕ | ✕ |
| Package = M365Suite | ✕ | ✕ | ✕ | ✓ | ✓ | ✓ |


