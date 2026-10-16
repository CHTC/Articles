---
title: "OSG Certificates Changing"
author: Mine Altunay

publish_on:
  - osg

type: news

canonical_url: "https://osg-htc.org/news/2015/12/02/osg-certificates-changing/"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/stock_card.jpeg"
  alt: "Open Science Grid"

description: |
    The Open Science Grid (OSG) provides certificates to its community of users and service owners for
    the purposes of authenticating them to one another. The identities of the certificate owners must be
    vetted by a set of trusted agents and protections must be put in place that certificates are only
    dispensed to their rightful owners.
excerpt: |
    The Open Science Grid (OSG) provides certificates to its community of users and service owners for
    the purposes of authenticating them to one another. The identities of the certificate owners must be
    vetted by a set of trusted agents and protections must be put in place that certificates are only
    dispensed to their rightful owners.

---

The Open Science Grid (OSG) provides certificates to its community of users and service owners for the purposes of authenticating them to one another. The identities of the certificate owners must be vetted by a set of trusted agents and protections must be put in place that certificates are only dispensed to their rightful owners. OSG operates a Certificate Authority (CA) and accompanying necessary infrastructure services that enable vetting identities, issuing certificates and renewing or revoking them when needed.

The OSG CA backend operations will undergo an important transition starting December 2015 lasting until the end of June 2016. The CA will change the vendor that operates the backend CA operations from DigiCert to CILogon. The changes will have no impact on the user interfacing services, the OSG CA web sites or the interactions between the end users and the CA Agents. The change will only impact the way the backend server creates and cryptographically signs the requests. Throughout the transition phase, OSG will continue to operate our DigiCert backend and the new CILogon backend. User and service certificates will be transitioned to the new vendor in groups starting with CMS and ATLAS in the winter of 2015. Every month until June 2016, a new set of Virtual Organizations (VOs) will be transitioned to the new vendor.

Users aren’t required to prepare for this transition. Once end users’ certificates are near expiring, they go to OIM to get new certificates. The only change visible to the end user is when they renew their certificate, they will see that it is signed by the new vendor. Instead of DigiCert, the user Distinguished Name (DN) in the certificate will say CILogon OSG CA. From a user’s perspective, the process, the tools and the OIM web site to obtain and renew certificates remains unchanged. However, the new DNs need to be registered in [Virtual Organization Membership Service (VOMS)](https://twiki.grid.iu.edu/bin/view/Documentation/Release3/InstallVoms). OSG already has devised an automated process for registering new DNs with VOMS servers; users do not need to take any action. However, if a user also uses other services such as twiki, docdb, and so on, then they should contact each service provider and register their new DN. Only a small percentage of users are expected to access such services. Details are available at [https://twiki.grid.iu.edu/bin/view/Security/OSGCertificateService](https://twiki.grid.iu.edu/bin/view/Security/OSGCertificateService).

All VOs have a scheduled transition month, with each VO administrator being asked months in advance if the scheduled month is acceptable. Once scheduled, VO administrators will receive a reminder with details one month before their transition. If any unforeseen problems arise during the transition, OSG will revert the VO back to the old vendor immediately and continue providing certificates while fixing the problem.
