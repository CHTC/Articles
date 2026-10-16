---
title: "No Place Like Home, Part 2:  Connecting to an HTC “supercomputer”"
author: Rob Gardner

publish_on:
  - osg

type: news

canonical_url: "https://osg-htc.org/news/2015/07/27/no-place-like-home-part-2-connecting-to-an-htc-supercomputer/"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-Lincoln.png"
  alt: "Lincoln"

description: |
    In the previous post we discussed the comforts of computing right from “home”, i.e. the place where
    you develop source code, job submission scripts, parameter files, executable binaries, log files,
    data files and datasets large and small, with potentially external library dependencies. Keeping
    work on the remote systems in synch with work on the local system can be a challenge.
excerpt: |
    In the previous post we discussed the comforts of computing right from “home”, i.e. the place where
    you develop source code, job submission scripts, parameter files, executable binaries, log files,
    data files and datasets large and small, with potentially external library dependencies. Keeping
    work on the remote systems in synch with work on the local system can be a challenge.

card_src: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-Lincoln.png"
card_alt: "Lincoln"

---

In the [previous post](http://www.opensciencegrid.org/no-place-like-home-part-1-on-campus-grids-in-the-osg/) we discussed the comforts of computing right from “home”, i.e. the place where you develop source code, job submission scripts, parameter files, executable binaries, log files, data files and datasets large and small, with potentially external library dependencies. Keeping work on the remote systems in synch with work on the local system can be a challenge. Our team at UChicago and the Open Science Grid has been addressing this.

The “Campus Connect Client” is in beta-mode, but ready for early adopters to try out. In the plot, the heavy-side step function shows the moment at which OSG was added to a user’s local campus submission from the [Palmetto](http://citi.clemson.edu/palmetto/) cluster at Clemson University.

<figure>
<img style="max-width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-Lincoln.png" alt="Lincoln"/>
<figcaption>Work Courtesy Lincoln Bryant</figcaption>
</figure>

The following information is from the [OSG Support Helpdesk](http://support.opensciencegrid.org/support/home) authored by David Champion OSG Group @UChicago.

*The [Campus Connect Client](https://support.opensciencegrid.org/support/solutions/5000161595) is a bridge from a campus to OSG’s national grid infrastructure. OSG is a national distributed high-throughput system, not a traditional  [high performance supercomputer](https://en.wikipedia.org/wiki/Supercomputer) located in a single data center. The Campus Connect Client is a set of tools for linking a campus research computing cluster to a CI Connect instance. Users of a campus facility can submit jobs into the Open Science Grid without leaving their institutional working environment.*

*Campus Connect Client provides:*

- *interface for job and data transfer,*
- *synchronization with the OSG Connect server,*
- *interface for remote job management.*

*Experienced [HTCondor](http://research.cs.wisc.edu/htcondor/) users may prefer to use OSG Connect’s login server directly. But many campus researchers already have a comfortable home on their local computational resource, and no need to interact directly with HTCondor. Campus Connect Client targets these users, making it easy to extend local resources with the full national grid.*

OSG works with resource providers to set up Campus Connect Client access at the system level. If the package or module is already installed at your site, you can start using it today.  If not, we can work with your site operations team to provide it, or you can install it for yourself.
