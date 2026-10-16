---
title: "OSG Networking Services Up and Running"
author: Shawn McKee

publish_on:
  - osg

type: news

canonical_url: "https://osg-htc.org/news/2015/12/02/osg-networking-services-up-and-running/"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-OSG-USATLAS-latency-mesh.png"
  alt: "OSG-USATLAS-latency-mesh"

description: |
    Knowing how the networks that connect you to OSG are working is a critical question when things are
    behaving badly and network problems are a possible reason. Since September 14, 2015, the Open
    Science Grid Networking Service can answer network-related questions.
excerpt: |
    Knowing how the networks that connect you to OSG are working is a critical question when things are
    behaving badly and network problems are a possible reason. Since September 14, 2015, the Open
    Science Grid Networking Service can answer network-related questions.

card_src: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-OSG-USATLAS-latency-mesh.png"
card_alt: "OSG-USATLAS-latency-mesh"

---

Knowing how the networks that connect you to OSG are working is a critical question when things are behaving badly and network problems are a possible reason. Since September 14, 2015, the Open Science Grid Networking Service can answer network-related questions.

One component of OSG Networking Services is perfSONAR measurements of network metrics between OSG and Worldwide LHC Computing Grid (WLCG) sites that are gathered by specially crafted Resource and Service Validation (RSV) probes. Results are stored in the Energy-Sciences Monitoring Database (ESmond) developed by ESnet. As the metrics are stored in OSG, they are also published to an Active Message Queue at CERN that allows users to easily subscribe to any or all of the metrics.

OSG runs a version of MaDDash (Monitoring and Diagnostic Dashboard) to summarize and visualize the metrics measured between sites. The mesh shown in MaDDash organizes sources for tests along the rows and destinations along the columns. Clicking on a cell takes you to a graph of the measurement history and details of the measurements. This data has proven critical in identifying and resolving network problems between Langston and Oklahoma University and with the ATLAS Tier-2 sites in Michigan and Indiana.

<figure>
<img style="max-width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-OSG-USATLAS-latency-mesh.png" alt="OSG-USATLAS-latency-mesh"/>
<figcaption>Figure courtesy of Shawn McKee. Shown is the MaDDash view of the USATLAS latency mesh colored coded by the amount of packet-loss observed. Green is OK.</figcaption>
</figure>

In addition to MaDDash, OSG provides an API to allow programmatic access to all the data collected including network latency, packet-loss, useable bandwidth and path information. Since the end of October, Ilija Vukotic, University of Chicago, has been routing the data sent to Active Message Queue into an ElasticSearch instance. This beta-version analytics platform allows the perfSONAR data to be visualized and analyzed via Kibana4. Users are welcome to create their own dashboards by visiting http://cl-analytics.mwt2.org:5601

Still to come is a network alerting and alarming capability in spring 2016 to notify site users and administrators of potential network problems impacting their site, as well as new tools to manage perfSONAR testing meshes and to visualize network topologies. For further details see https://twiki.opensciencegrid.org/bin/view/Documentation/NetworkingInOSG
