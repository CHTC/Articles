---
title: "ATLAS and BNL Bring Amazon EC2 Online"
author: John Hover

publish_on:
  - osg

type: news

canonical_url: "https://osg-htc.org/news/2016/02/01/atlas-and-bnl-bring-amazon-ec2-online/"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-run203602_evt82614360_ID_LAR_Atlantis_hres.png"
  alt: "ATLAS event display"

description: |
    Four years ago the ATLAS and CMS experiments at the LHC successfully found the Higgs particle. In
    the US, most processing was performed on resources owned by the LHC collaborations, knit together
    and managed as part of the Open Science Grid. Since then the LHC experiments continue to explore the
    properties of the Higgs, and expand their studies beyond it.
excerpt: |
    Four years ago the ATLAS and CMS experiments at the LHC successfully found the Higgs particle. In
    the US, most processing was performed on resources owned by the LHC collaborations, knit together
    and managed as part of the Open Science Grid. Since then the LHC experiments continue to explore the
    properties of the Higgs, and expand their studies beyond it.

card_src: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-run203602_evt82614360_ID_LAR_Atlantis_hres.png"
card_alt: "ATLAS event display"

---

Four years ago the ATLAS and CMS experiments at the LHC successfully found the Higgs particle. In the US, most processing was performed on resources owned by the LHC collaborations, knit together and managed as part of the Open Science Grid. Since then the LHC experiments continue to explore the properties of the Higgs, and expand their studies beyond it. Alas, the budgets for maintaining dedicated data centers are flat or falling, but the scientific need for compute power remains.

<figure class="figure float-end" style="margin-left: 1em">
  <img src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-run203602_evt82614360_ID_LAR_Atlantis_hres.png" class="figure-img img-fluid rounded" alt="ATLAS event display" width="350px">
</figure>

Three technical barriers have stood in the way of ATLAS economically using commercial clouds.

First, the need to use Amazon’s Elastic Compute Cloud (EC2) spot market. Computing on the spot market is 1/10 to ¼ the cost of on-demand instances, resulting in core/hour costs comparable (or even cheaper) than dedicated ATLAS-owned data centers.  But nodes acquired on the spot market can be terminated at any time, meaning workload needs to be interruptable. The second barrier is the need to automatically and safely manage the acquisition and shutdown of large numbers of virtual machines (VMs). Handling this scale manually is not possible. The third barrier is the need to avoid slow data movement and costly data egress fees.

Over the last 18 months, the RHIC/ATLAS Computing Facility (RACF) at Brookhaven National Laboratory has been collaborating with Amazon on a pilot project to solve these problems, and move the usage of the Amazon Web Services (AWS) and the EC2 Spot market from theoretical possibility to a practical, production-grade, 100,000-core platform for doing science.

ATLAS had already been developing an enhancement to PanDA (Production and Distributed Analysis), their workload management system, that offers an *event-based* processing model rather than a job-based approach. This *Event Service* allows a worker process to complete one event at a time, uploading output when it is complete. Since events take much less time to analyze than jobs (which might process hundreds of events), if a worker is killed very little work is lost. The feature is ideal for use on EC2 spot, where nodes can be terminated whenever the spot price exceeds the user’s bid price.

To address the VM management problem, ATLAS adapted their existing HTCondor-G based pilot submission tool, AutoPyFactory, to also handle the VM lifecycle. When it detects waiting jobs in the ATLAS queues, it launches an appropriate number of VMs, maintains the number as nodes are terminated, and shuts them down as work is completed.

Addressing the data movement problem required two changes. First, the ATLAS workload system had to be adjusted to enable the usage of object-based storage so that it could natively leverage the Amazon Simple Storage Service (S3). Some related work was already being done for the Event Service in this direction. Other work toward making object stores first-class ATLAS storage endpoints is still underway.

Second, to avoid causing data flows between BNL and Amazon to travel over the public internet (which is costly for Amazon), ESNet has put in place high bandwidth (20-100GB), direct network peering between the DOE research network and AWS. Because usage of these peering points is not costing Amazon extra, they are willing to waive the customary egress charges as long as substantial compute resources are being purchased.

<figure class="figure float-start" style="margin-right: 1em">
  <img src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-EC2-Data-Movement-OSG1.png" class="figure-img img-fluid rounded" alt="ATLAS EC2 data movement" width="350px">
  <figcaption class="figure-caption">ATLAS EC2 Data Movement<br/></figcaption>
</figure>

Last September, RACF and ATLAS performed a ~40,000-core, 7-day scaling run (~5000 8-core VMs). This run performed useful ATLAS analysis, using real data, on the EC2 Eastern region, on two instance types.

A final 100,000-core run is planned for mid-February. This run will utilize all three EC2 US regions, using (at least) 5 instance types, with all job data movement using native S3. A successful run will demonstrate the ability to economically provide, when needed, computing resources twice the size of the existing US ATLAS data centers (~50,000 cores).
