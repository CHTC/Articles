---
title: HTCondor Withstands CERN’s Massive Stress Test
author: Sophie Dorros

publish_on:  
    - htcondor
    - path
    - osg

type: news

canonical_url: https://htcondor.org/featured-users/2025-12-03-cern-stresstests-htcondor.html

image:  
    path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/cern.jpg"   
    alt: Image of cern

excerpt: HTCondor withstands a massive stress test to prepare the Large Hadron Collider for more data

---

<figure>
<img style="width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/cern.jpg" alt="A computing server corridor in CERN's main data centre. (Image: Anthony Grossir/CERN)"/>
<figcaption>A computing server corridor in CERN's main data centre. (Image: Anthony Grossir/CERN)</figcaption>
</figure>


The CERN IT team carried out a stress test on its [computing infrastructure](https://home.cern/science/computing/data-centre) in October, and injected 16,800 jobs into the system, around 20 times the current average throughput. [HTCondor](https://htcondor.org/) withstood the test, and the average job handling time remained at a reasonable 5 minutes for the scale of jobs.



In 2030, the [Large Hadron Collider](https://home.cern/science/accelerators/large-hadron-collider), the world’s largest and most powerful particle accelerator, will become the [High- Luminosity LHC](https://home.cern/science/accelerators/high-luminosity-lhc) (HL-LHC), creating more particle collisions per second and increasing the amount of data able to be collected. [The European Organization for Nuclear Research](https://home.cern/), or CERN, has begun a series of tests to prepare data infrastructure for the massive amounts of data coming its way from the HL-LHC.



The HTCondor software supports CERN’s data workload management, relying on two main programs that run in the background and perform tasks, called daemons. The collector daemon and the negotiator daemon work together to gather user job requests, track available compute resources in the [OSPool,](https://osg-htc.org/services/ospool/) and match each job with the appropriate machine within CERN’s infrastructure. Overall, HTCondor handles every aspect of running jobs for CERN: queuing jobs, deciding the running order, and assigning jobs to machines that can run them.



Because the HL-LHC will produce so much data, it’s important that current systems can support processing when the time comes. Currently, there are 125,000 running jobs at a time, and the HL-LHC will require that capacity to run almost 500,000.



CERN will continue implementing many other tests until the HL-LHC is up and running, including tests on CERN’s disk-based storage system, which helps to store the huge amounts of data produced by the international scientific community. Click [here](https://home.cern/news/news/computing/when-failure-good-news) to view CERN’s news report on the test.