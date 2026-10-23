---
title: "The Quest to Find Rare Neutron Star Mergers: A Computing Challenge"
author: Sophie Dorros
publish_on:
  - chtc
  - osg
  - htcondor
  - fabaid
type: user
canonical_url: "https://chtc.cs.wisc.edu/neutron-stars-and-computing-challenges.html"
image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/coughlin-htc26-slide.jpg"
  alt: "Slide titled A Golden Era for Astrophysics showing the Vera Rubin Observatory, JWST, LIGO/Virgo/KAGRA and IceCube"
excerpt: |
  Dr. Michael Coughlin explains how computing challenges in gravitational wave detection are being solved using
  high throughput computing in his HTC26 keynote address.
---

Astrophysics is in a “golden era, with many many different instruments coming online,” remarked Dr. Michael Coughlin in his Keynote address at [High Throughput Computing Week 2026](https://agenda.hep.wisc.edu/event/2432/) (HTC26). Multi-messenger astrophysics, which combines different signal types (gravitational waves, light, neutrinos) from the same cosmic event, is where this exciting science is happening. This new era for the astronomy community was the subject of Coughlin's keynote presentation and a theme at HTC26, the annual multi-day gathering that brings together researchers, system administrators and others interested in high throughput computing and the science it enables.

<figure>
<img style="width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/coughlin-htc26-slide.jpg" alt="Slide titled A Golden Era for Astrophysics showing the Vera Rubin Observatory, JWST, LIGO/Virgo/KAGRA and IceCube"/>
<figcaption>Examples of gravitational wave detectors. Credits: Michael Coughlin</figcaption>
</figure>

Coughlin is an astrophysicist at the University of Minnesota who works on the [LIGO-Virgo-KAGRA](https://www.ligo.caltech.edu/page/ligo-scientific-collaboration) (LVK) collaboration studying gravitational-wave detection. Gravitational waves are ripples in spacetime caused by extreme events like merging black holes or neutron stars, predicted by Einstein's general relativity. Detection of these gravitational waves uses interferometers, a kind of precision measurement device, from various detectors: LIGO (Hanford, WA and Livingston, LA), Virgo (Italy), KAGRA (Japan), and a future LIGO detector under construction in India. These detect gravitational waves by measuring tiny changes in laser light bounced between mirrors kilometers apart. Multiple detectors are needed to confirm a signal is real and not just local noise and to pinpoint where in the sky it came from.

By advancing both the sensitivity and speed at which neutron star mergers can be measured, Coughlin and his team are helping advance the field of astronomy through computing. This science matters for understanding nuclear physics, cosmology, and the origin of heavy elements on the periodic table. The main challenge they face is that these neutron star merging events are rare and difficult to catch. Binary black hole mergers are common in the data but usually produce no light, but binary neutron star mergers are rarer and produce light, including a "kilonova," where neutron-rich material ejected in the merger undergoes rapid radioactive decay, forming heavy elements (like gold) and glowing in a detectable way.

Despite improving detectors, LVK’s most recent observing run found zero new neutron star mergers, and expected rates going forward are only around five per year. "[These are] the expectations… for how many neutron star mergers we should have found in the last observing run we did. I'll give you a hint: we found none. So that's not so good." Kilonovae fade fast and are much dimmer than supernovae, making them a uniquely hard "time domain" astronomy problem that needs a reaction time within hours, not weeks. Meanwhile, data volumes are exploding: the upcoming [Rubin Observatory](https://rubinobservatory.org/) alone will generate around 20 terabytes a day and 20 million alerts per night.

<figure style="float: right; margin: 0 0 1rem 1rem; width: 300px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/coughlin-headshot.jpg' class="figure-img img-fluid rounded" alt="Dr. Michael Coughlin">
<figcaption>Pictured: Dr. Michael Coughlin. Credits: Michael Coughlin</figcaption>
</figure>

To evaluate this massive amount of data and at the speed required to process it, Coughlin and his team are implementing high throughput computing and machine learning techniques. Machine learning is already speeding up detection pipelines, with Coughlin’s team's model detecting one event 5 seconds faster than competing pipelines, with the field's goal of alerting the world within 10 seconds of detection. "We would like to find ways to minimize this so that people can spend more time doing the science," noted Coughlin.

Not all of this work can run on shared computing resources. The pipelines that send alerts within seconds run on dedicated hardware, Coughlin said, because they can't wait in a queue. But much of the field's computing isn't time-sensitive: training machine learning models, running large simulation campaigns to measure how often pipelines raise false alarms, and reprocessing a full observing run's data to produce the final catalog of detections, which comes out about a year later. That work is where high throughput computing fits, and Coughlin said his team is starting to use it to prepare for the next observing run.

Coughlin’s goal is to let astronomers launch computationally expensive analyses directly from the web tools they already use, with the jobs distributed through the [OSG](https://osg-htc.org/) and the results returned automatically. Some LVK researchers already submit jobs to the [OSPool](https://osg-htc.org/services/ospool/) through [HTCondor](https://htcondor.org/), but Coughlin said only a subset of graduate students are comfortable doing so. "Enabling a lot of this through frontends is going to be the way to get more people access to Rubin and LIGO," he said.

Coughlin's full presentation from HTC26 can be viewed [here](https://www.youtube.com/watch?v=CSqCnAk7AYw).
