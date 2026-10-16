---
title: "Using Open Science Grid to prepare for ‘the next big thing’ at Brookhaven"
author: Greg Moore

publish_on:
  - osg

type: news

canonical_url: "https://osg-htc.org/news/2015/06/25/using-open-science-grid-to-prepare-for-the-next-big-thing-at-brookhaven/"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-Martin.jpg"
  alt: "Martin"

description: |
    In November 2014, the PHENIX ( P ioneering H igh E nergy N uclear I nteraction e X periment)
    collaboration, that conducts research in heavy ion collisions, updated its 2010 proposal to upgrade
    the PHENIX detector at the Relativistic Heavy Ion Collider (RHIC) at Brookhaven National Laboratory
    (BNL).
excerpt: |
    In November 2014, the PHENIX ( P ioneering H igh E nergy N uclear I nteraction e X periment)
    collaboration, that conducts research in heavy ion collisions, updated its 2010 proposal to upgrade
    the PHENIX detector at the Relativistic Heavy Ion Collider (RHIC) at Brookhaven National Laboratory
    (BNL).

card_src: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-Martin.jpg"
card_alt: "Martin"

---

<figure>
<img style="max-width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-Martin.jpg" alt="Martin"/>
</figure>

In November 2014, the PHENIX (**P**ioneering **H**igh **E**nergy **N**uclear **I**nteraction e**X**periment) collaboration, that conducts research in heavy ion collisions, updated its 2010 proposal to upgrade the PHENIX detector at the Relativistic Heavy Ion Collider (RHIC) at Brookhaven National Laboratory (BNL). The detector recorded its first relativistic heavy ion collision in 2000, and now records many different particles emerging from collisions at RHIC. As in every year, PHENIX will stop running around the end of June due to power consumption and maintenance needs. After that, the collaboration will gear up for one final run in 2016, starting preparations after Thanksgiving and running through about June 2016.

*Photo Martin Purschke*

BNL’s Martin Purschke is actively planning the next version of PHENIX—currently known by the working name sPHENIX, or SuperPHENIX. “PHENIX was designed in the early 90s and has mostly fulfilled its purpose,” says Purschke. “We have learned a lot of new things similar to the evolution you see with the Large Hadron Collider at CERN. Physicists are always preparing for the next big thing, which here at Brookhaven is sPHENIX.” The name may change since they are still in the proposal stage of the project, but they are looking to bring the detector online in the 2020-22 timeframe. Meanwhile, Purschke is running simulations on the Open Science Grid (OSG) to help determine the design.

sPHENIX will reuse much of the existing PHENIX infrastructure, but the challenge now, according to Purschke, is moving from detecting single particles to detecting jets. “The next big thing will be measuring ‘jets,’ which are like a spray of particles moving in a very narrow cone. This calls for a different detector design. We received a super-conducting magnet from SLAC National Accelerator Laboratory, which we already have on site. It is the core of the new experiment,” says Purschke. Just shy of three meters in diameter and about four meters long, the cylinder will be instrumented with detectors such as calorimeters. “Collisions will happen in the center of the cylinder, and the particles will come out every which way, even to the edges of the cylinder. Particles will no longer be coming straight into the detector modules, but will hit the modules at the edge of the cylinder at significant angles.”

<figure>
<img style="max-width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-sPHENIX.png" alt="sPHENIX"/>
<figcaption>An engineering drawing of sPHENIX by Richard Ruggiero, courtesy Brookhaven National Laboratory.</figcaption>
</figure>

The detector will have a different response to particles coming in at an angle, so right now Purschke is running simulations on the OSG to help determine that particular design aspect. “We are trying to optimize detector performance with as little angle and tilt as we can get away with and still get decent performance,” he says. “We have quite a laundry list of simulations to run. We need to know how many particles to expect and build the detector accordingly.”

Even carefully choosing which jobs to run, Purschke says he is using a lot of OSG processing power—about 5 million hours in April and May alone, and 5.4 million hours since the start of the year. He intentionally selects OSG simulation projects with a good ratio of CPU time to input/output (IO), and so far has produced about 30 to 32 terabytes of data.

“Generally speaking, many of the simulations produce too much data to make it worthwhile to run them on the OSG, so I’m picking about five simulations out of the 60 or so that could be run on the OSG,” says Purschke. “I have had a single one running in April and May. When it’s done I will move on to the next—I have a couple more waiting in the pipeline. Left to only the computing resources here at BNL, we simply don’t have enough computing power for these types of simulations and wouldn’t be able to run them at all. OSG is a fantastic resource.”

Purschke may be able to drill deeper depending on what he finds, but he is committed to being a good citizen on the OSG. “I’m currently running about 5,000 billion (5 trillion) simulated collisions,” he says. “Ninety nine percent of the about half-million total jobs complete just fine. I always have some failures—that is normal—so I look for the optimal number of jobs versus success. I don’t want to make them too long or too small. Each job is running around eight hours and that is optimal. After I set them up, they are pretty much on autopilot and I check on them twice a week. On the whole, it has been fantastically smooth sailing. If I had to look at individual jobs, I couldn’t do it.”

As its name suggests, the PHENIX apparatus has been a pioneering experiment. “At the time, no one knew what collisions at this energy level would look like,” says Purschke. “We put detectors in place to measure as many aspects of the collisions as possible because no one knew what to expect. Now we want to move on from individual particle measurements.”

sPHENIX will help address questions about the nature of strongly coupled [quark-gluon plasma](http://en.wikipedia.org/wiki/Quark%E2%80%93gluon_plasma) (QGP), and how and why it behaves as a perfect fluid—questions that can only be addressed by a detector that can measure jet production. “The challenge now is measuring these jets in a heavy ion experiment,” says Purschke. “It is a big mess because of how many particles there are. We are very glad to have resources like the OSG to test our design. It helps us save enormous amounts in engineering costs.”
