---
title: "Mu2e Simulations on the OSG"
author: Hanah Chang

publish_on:
  - osg

type: news

canonical_url: "https://osg-htc.org/news/2015/07/09/mu2e-simulations-on-the-osg/"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-mu2e.png"
  alt: "Chart of Mu2e computing hours at Fermilab and on the OSG"

description: |
    The Mu2e high energy physics collaboration received Critical Decision (CD) 2/3b from DOE in March of
    2015 and is preparing for the next set of needed reviews before they are approved to completely
    build the experiment and take data. Before that review, the scientists will be validating and
    refining the existing design of the particle detector to scale up their detector and event data
    simulation.
excerpt: |
    The Mu2e high energy physics collaboration received Critical Decision (CD) 2/3b from DOE in March of
    2015 and is preparing for the next set of needed reviews before they are approved to completely
    build the experiment and take data. Before that review, the scientists will be validating and
    refining the existing design of the particle detector to scale up their detector and event data
    simulation.

card_src: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-mu2e.png"
card_alt: "Chart of Mu2e computing hours at Fermilab and on the OSG"

---

The [Mu2e](http://mu2e.fnal.gov/) high energy physics collaboration received Critical Decision (CD) 2/3b from DOE in March of 2015 and is preparing for the next set of needed reviews before they are approved to completely build the experiment and take data. Before that review, the scientists will be validating and refining the existing design of the particle detector to scale up their detector and event data simulation. The Mu2e scientists have designed a new “simulation campaign.” To complete this plan in time for the next review, the team estimated that they would need the computing capacity of 4,000 CPUs for 4-5 months (followed by a much smaller need for the rest of the year.) Due to the enormity of the campaign and the limited amount of resources, Mu2e adapted their workflow and data management systems to run a majority of the simulations at sites other than Fermilab – across the Open Science Grid (OSG) distributed high-throughput computing facilities.

Mu2e scientist Andrei Gaponenko explained that last year, Mu2e utilized more than their allocation of computing by using any and all available CPU cycles not used by other experiments locally on FermiGrid. The experiment decided to continue this concept on the OSG by running “opportunistically” on as many available remote computing resources as possible. He further said, “there were some technical hurdles to overcome. For example, the scripts running the Mu2e software needed to make sure all the necessary disk spaces were available at more than 25 remote sites and that the local operating system software was compatible. A lot of people worked very hard to make this possible.” Members of the OSG Production Support team helped support this endeavor – making the sites available to Mu2e, helping debug problems with the job and data processing, etc. Members of the Fermilab Scientific Computing Division supported the experiment’s underlying scripts, software and data management tools.

<figure class="figure float-end" style="margin-left: 1em; width: 350px;">
  <img src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-mu2e.png" class="figure-img img-fluid rounded" alt="Chart of Mu2e computing hours at Fermilab and on the OSG" width="350px">
  <figcaption class="figure-caption">Chart Courtesy Bo Jayatilaka<br/></figcaption>
</figure>

The move to use OSG was productive and provided extensive benefits to the experiment. As shown in the above chart, from March 1 through July 10, Mu2e has used 3.3M hours at their home institution and 11.2M hours on OSG for a total of 14.5M hours. Rob Kutschke, Mu2e analysis coordinator said, “We (Mu2e experimenters) are pilot users on OSG and we are grabbing cycles opportunistically whenever we can. We had issues, but we solved them. While we did not expect things to work perfectly the first time, very quickly we were able to get many hundreds of thousands of CPU hours.” Ray Culbertson, Mu2e production coordinator, agreed. “We exceeded our baseline goals, met the stretch goals and will continue to maintain schedule.” As Mu2e begins new big pushes over the next few years, he hopes that OSG is here to stay. In terms of the future, everyone believes that Mu2e will continue to use OSG resources. Indeed, Ken Herner, member of the support team in the Fermilab Scientific Computing Division that helped the experimenters port their applications to the OSG, hopes that Mu2e will serve as an example for more experiments that currently do their event processing computing locally at Fermilab. He said, “From my point of view, the more important thing is demonstrating to other experiments here that it can work and it can work really well. Ideally, this sort of running should become the norm. What you really want is to just submit the job, and if it runs on-site, great and if it runs off-site, great, just give me as many resources as possible.”

Above all, the experimenters are thankful for everyone’s hard work and dedication to make this happen.
