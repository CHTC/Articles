---
title: "Three Scientists from the Vera C. Rubin Observatory Astronomy Community Present at HTC Week 2026"
author: Sophie Dorros
publish_on:
  - chtc
  - htcondor
  - path
type: news
canonical_url: "https://chtc.cs.wisc.edu/vera-c-rubin-community-presents-at-htc-week-2026.html"
tag:
- chtc_featured_article
image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/Trifid and Lagoon (Image).jpeg"
  alt: "Image of Trifid and Lagoon Nebulas from the Vera C. Rubin Observatory. Credits: NSF–DOE Vera C. Rubin Observatory"
banner_src: "https://raw.githubusercontent.com/CHTC/Articles/main/images/Trifid and Lagoon (Image).jpeg"
banner_alt: "Image of Trifid and Lagoon Nebulas from the Vera C. Rubin Observatory. Credits: NSF–DOE Vera C. Rubin Observatory"
excerpt: |
  Last June, the first images from the Vera C. Rubin Observatory were revealed, processed using HTCondor. This June, three members of the Rubin astronomy community presented at Throughput Computing Week 2026, sharing how HTCondor powers their massive data workflows.
---
Last June the [first images from the Vera C. Rubin Observatory](https://rubinobservatory.org/news/rubin-first-look), a facility jointly funded by the [National Science Foundation](https://www.nsf.gov/) and the [U.S. Department of Energy's Office of Science](https://www.energy.gov/science/office-science), were revealed. Located atop Cerro Pachón in Chile, the Rubin Observatory is equipped with the largest digital camera ever built and produces high-resolution imagery of our solar system. These first images were of the Virgo Cluster and the Trifid and Lagoon Nebulas. The processing required to generate these deep-field images is massive, and this was accomplished through the use of [HTCondor](https://htcondor.org/), a workload management and job scheduling system developed by the [Center for High Throughput Computing](https://chtc.cs.wisc.edu/).

<figure>
<img style="width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/Trifid and Lagoon (Image).jpeg" alt="Image of Trifid and Lagoon Nebulas from the Vera C. Rubin Observatory"/>
<figcaption>Image of Trifid and Lagoon from the Rubin Observatory. Credits: NSF–DOE Vera C. Rubin Observatory</figcaption>
</figure>

This June, three members of the Rubin Observatory astronomy community presented at [Throughput Computing Week 2026](https://agenda.hep.wisc.edu/event/2432/). Colin Slater, Head of Data Production at the Rubin Observatory, shared Rubin's thanks to HTCondor in one of his slides in his presentation "[Processing Every Image: Rubin Observatory's Data Release Production](https://agenda.hep.wisc.edu/event/2432/contributions/37879/)." Slater's presentation noted that the Rubin Observatory's 3.2 GPix camera takes a new image around every 40 seconds throughout the night. This results in 600 to 800 images per night, producing around 10 TB per night of raw data. The largest challenge lies in the sheer amount of raw data collected, as the Rubin Observatory thinks about how to distribute these images to users as it scales.

<figure style="float: left; margin: 0 1rem 1rem 0; width: 226px;">
<img style="width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/TCondor-supported-rubin-data.png"  height="300" width="226" alt="Slide from Colin Slater's HTC Week 2026 talk"/>
<figcaption>Slide from Colin Slater's HTC Week 2026 talk. Credits: Colin Slater</figcaption>
</figure>

Slater noted the observatory's goal to annually publish their "best" data set, incorporating everything they've observed with around six months of processing time. This data release production requires "calibrating every single image, combining all images that overlap a given patch of sky ('stacking'), and measuring every object on that combined image." And then finally going back to each individual image to measure the history of each object.

<figure style="float: right; margin: 0 1rem 0 1rem; width: 200px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/colin-slater-htc26.jpg' height="300" width="200" class="figure-img img-fluid rounded" alt="Colin Slater at HTC Week 2026">
<figcaption>Pictured: Colin Slater at HTC Week 2026. Credits: Jeff Peterson</figcaption>
</figure>

In his talk "[Rubin Observatory: Scaling towards Data Release Production using HTCondor](https://agenda.hep.wisc.edu/event/2432/contributions/37884/)," Gregory Daues, Senior Research Software Engineer at the National Center for Supercomputing Applications (NCSA), gave an overview of the kinds of work the Rubin Observatory is doing, including the steps that go into image processing, and how HTCondor is being leveraged in their workflows. Daues reports that processing just a single year's data into a data release involves around 100 distinct pipeline tasks with hundreds of millions of individual job instances, requiring a system that can coordinate jobs while managing dependencies between tasks. The Rubin Observatory uses small placeholders, called glideins, that run on machines worldwide and connect back to a central HTCondor system, allowing for the collection of separate resources to run on a unified pool scientists can submit their processing work to.

<figure style="float: left; margin: 0 1rem 1rem 0; width: 200px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/Greg htc26.jpg' height="300" width="200" class="figure-img img-fluid rounded" alt="Greg Daues at HTC Week 2026">
<figcaption>Pictured: Greg Daues at HTC Week 2026. Credits: Jeff Peterson</figcaption>
</figure>

Shreya Anand, Legacy Survey of Space and Time - Discovery Alliance (LSST-DA) Catalyst Fellow at Stanford University, also shared details about the Rubin Target of Opportunity (ToO) program, focusing on gravitational wave searches in her talk "[Computing hurdles in wide-field target-of-opportunity searches with Rubin and ZTF](https://agenda.hep.wisc.edu/event/2432/contributions/37854/)." She noted challenges that they are grappling with: conducting archival queries on updated skymaps, and filtering results to have a digestible number of candidates ahead of an upcoming six-month observational run for data collection. Her presentation pointed to successful test runs, including a black hole merger where nine telescope positions covered 94% of the probable sky region, and a low-mass merger candidate where Rubin mapped around 800 square degrees in just three hours.

<figure style="float: right; margin: 0 1rem 0 1rem; width: 239px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/headshot_sanand.jpeg' height="300" width="239" class="figure-img img-fluid rounded" alt="Shreya Anand">
<figcaption>Pictured: Shreya Anand</figcaption>
</figure>

HTCondor core developer Greg Thain remarked that "Processing the imagery from the Rubin Observatory is a multi-national effort: Data is collected on one continent, then sent to multiple processing sites worldwide. The distributed approach is a natural fit for the distributed nature of the HTCondor Software Suite."
