---
title: "No Place Like Home, Part 1: On Campus Grids in the OSG"
author: Rob Gardner

publish_on:
  - osg

type: news

canonical_url: "https://osg-htc.org/news/2015/06/01/no-place-like-home-part-1-on-campus-grids-in-the-osg/"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/stock_card.jpeg"
  alt: "Open Science Grid"

description: |
    OSG Connect was introduced last year as a simple access solution for the Open Science Grid.
excerpt: |
    OSG Connect was introduced last year as a simple access solution for the Open Science Grid.

---

[OSG Connect](http://osgconnect.net/) was introduced last year as a simple access solution for the Open Science Grid. OSG Connect provides a login server with an HTCondor scheduling service that submits jobs to:

- the OSG VO glidein system, which sends jobs to all grid sites supporting the OSG VO community;
- and to shared campus grids, such as OrangeGrid at Syracuse University and UC3 at the University of Chicago.

An account derived from a user’s institutional identity (via CI-Logon, the campus hosted  Shibboleth service, and Globus) provides simple access for researchers not already affiliated with an existing VO.  To use the system one obviously must login to an “off campus” server, which to some users and campus research computing support staff seems unnatural. Why is that?

Well, at most universities the campus research computing center is a focal point of support with research groups and individual investigators.  For many users, the campus HPC cluster is the first stop for research computing. Often new faculty invest their startup funding in [condominium clusters](http://citi.clemson.edu/arcc/) in which resources are pooled and managed centrally.  The center will provide training, workshops, consultancy services and extensive user documentation to effectively use their resources.  This is where “home” is and typically has all the expected comforts: a campus network ID, local support resources, institution-specific web-based training materials, project storage, the local login host, a local batch queue, a good connection to Internet2 or ESnet, and quite literally the **/home** server where users manage their  work.

For research groups seeking to transform their science by using distributed high throughput computing resources off campus, i.e. those accessible via OSG services – whether grid or cloud, the question becomes one of convenience.  How does one manage the minutiae of Unix shell-based computing for jobs which use those remote resources?  These typically include source code, job submission scripts, parameter files, executable binaries, log files, data files and datasets large and small, and potentially external library dependencies.  How does one keep work on the remote systems in synch with work on the local system?

This argues for deploying a suitably configured grid-enabled HTCondor job submission server at the campus HPC center, so as to locally mount the user’s work environment and minimize the switch between local and remote computing.  A small number of campuses interface to the OSG this way, but it typically requires having some local expertise in operating an HTCondor service, a server capable of scaling to the anticipated workloads, and a commitment to support the service by the research computing director.  Depending on the available manpower, this may not always be feasible or natural for campuses which use local batch schedulers other than HTCondor.  Another approach is to use the Bosco desktop application from the campus login server; this works well so long as the number of simultaneous users is small and the number of jobs kept to a number commensurate with local file system capabilities.

In Part 2 of this article I  will describe an approach whereby a light-weight client is used from the campus login host to interact with the OSG Connect server which does the heavy lifting for distributed job scheduling.  A [preview](https://indico.fnal.gov/contributionDisplay.py?contribId=52&confId=8580) of the “campus connect client” was given by David Champion at the Northwestern OSG All Hands meeting in March.  For those interested in testing out the latest version the software is available in [Github](https://github.com/CI-Connect/connect-client).
