---
title: "Value of Reliable Services in OSG (and how we make it happen)"

publish_on:
  - osg

type: news

canonical_url: "https://osg-htc.org/news/2015/07/27/value-of-reliable-services-in-osg-and-how-we-make-it-happen/"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-op-status.png"
  alt: "op-status"

description: |
    The OSG recently delivered 22.3 million CPU hours in a single week. In addition to the CPU and
    storage resources needed to deliver computation at this level a large number of services are
    required to support associated tasks.
excerpt: |
    The OSG recently delivered 22.3 million CPU hours in a single week. In addition to the CPU and
    storage resources needed to deliver computation at this level a large number of services are
    required to support associated tasks.

card_src: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-op-status.png"
card_alt: "op-status"

---

The OSG recently delivered 22.3 million CPU hours in a single week. In addition to the CPU and storage resources needed to deliver computation at this level a large number of services are required to support associated tasks.

For a job to

<figure>
<img style="max-width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-op-status.png" alt="op-status"/>
</figure>

run on an OSG resource, users must have a place to submit it and a place to store data and code. They must be able to obtain information about the state of the OSG and its components. These components must communicate their state in an automated manner<br/> to allow detection of inevitable inturruptions. It must be possible to communicate with operators of these systems without any special knowledge of particulars as to who does what and, finally, it must be possible to figure out how to do what the user wants to do.

In systems with many components, the proper and complete functioning of the overall system requires each component to function with an availability higher than required of the larger system. A failure is the failure of any component.

Services offered by the OSG Operations Center fall into all of the categories discussed above and are covered by Service Level Agreements (SLAs) specifying the availability that must be achieved. These specifications vary from service to service, usually requiring 99% availability, but in no case less than 97%. The Operations Center is proud to have delivered services consistent with these SLAs without exception for the last several years and looks forward to continuing to do so.

Scott Teige for the Operations Center
