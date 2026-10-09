---
title: "Migration to HTTP from GridFTP for Data Transfers"

publish_on:
  - osg

# Migrated from the `_news` collection in osg-htc.github.io, which was
# local to that repository and so was lost when the site moved off Jekyll.
# `news` is chosen to keep the article at its original
# /news/YYYY/MM/DD/ URL rather than as a strict read of the category --
# some of these read more like user stories, but moving them would mean
# adding a redirect for each one.
type: news

canonical_url: "https://osg-htc.org/news/2021/03/20/Migration-HTTPS-from-GridFTP-for-Data-Transfers.html"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/stock_card.jpeg"
  alt: "Open Science Grid"

card_src: "https://raw.githubusercontent.com/CHTC/Articles/main/images/stock_card.jpeg"
card_alt: "Open Science Grid"

excerpt: "The OSG consortium is nearing the completion of migrating its software stack to the WebDAV data transfer protocol - a widely used, industry-compatible and secure protocol. The WebDAV protocol which is an extension of the well-known HTTP allows Third-Party-Copy transfers which are commonly used to move bulk data..."
---

The OSG consortium is nearing the completion of migrating its software stack to the WebDAV data transfer protocol - a widely used, industry-compatible and secure protocol. The WebDAV protocol which is an extension of the well-known HTTP allows Third-Party-Copy transfers which are commonly used to move bulk data between storage systems worldwide. Moreover, WebDav is compatible with the OAuth2 mechanism for authentication. 

This migration started in 2017 when the Globus project moved away from releasing and supporting its GridFTP and GSI software under an open-source license. Since that time OSG has been working with the global cyberinfrastructure community [on plans](https://osg-htc.org/technology/policy/gridftp-gsi-migration/) to migrate the software stack to an open, non-proprietary, protocol for data transfer. In August 2017, the OSG Council approved the adoption of GridFTP and GSI source code support while developing migration plans. Two years later, in August 2019, the migration began with the OSG 3.5 series release, which included HTTPS support via WebDav implemented in the XRootD server. In December 2019, [detailed documentation](https://osg-htc.org/technology/policy/gridftp-gsi-migration/) was published for its user community. In February 2021, OSG released software series 3.6, without dependencies on either GridFTP or GSI. The end of support for release 3.5 is presently scheduled for February 2022. 

For researchers who access the Open Science Pool via the [OSG Connect access points](https://connect.osg-htc.org/), this change is transparent and has no impact whatsoever. The environment for transferring data and conducting their research will not change.  

Similarly, most campuses that use the OSG services will also be unaffected. Campuses that do use GridFTP today can migrate now, as OSG 3.5 includes the HTTPS solution in addition to the legacy GridFTP. If a site has a GridFTP server, the campus can add the HTTPS service on the same hardware, and decommission GridFTP when no longer in use, all within the same OSG 3.5 release.

Notice that GridFTP and WebDAV are not compatible, and consequently, there will be a period during which campuses may be required to support both protocols until all of their science communities have transitioned. 

The OSG consortium validated that the migration to HTTPS would not have a negative impact on data transfer performance, an important consideration given the volume of data transfers supported by the OSG. A paper that compares GridFTP and HTTPS in their respective third-party copy mode was recently submitted for publication. It reports up to 30% better performance for the HTTPS implementation than the GridFTP implementation. 

Individuals interested in more details on how a large community executes this transition can find more information in the [frequently asked questions and documentation](https://osg-htc.org/technology/policy/gridftp-gsi-migration/) for the  [Worldwide LHC Computing Grid](https://wlcg.web.cern.ch/) (WLCG) and US-LHC. In addition, Diego Davila, OSG senior developer, reported at the 2021 OSG All-Hands Meeting on ["HTTP Third-Party Copy: Getting rid of GridFTP.”](https://indico.fnal.gov/event/47040/contributions/208459/) Davila discussed the Compact Muon Solenoid (CMS) migration steps to WebDAV. Both [ATLAS](https://atlas.cern/) and [CMS](https://home.cern/science/experiments/cms) are hoping to complete their global transition to HTPPS by June 2021. 
