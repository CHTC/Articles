---
title: "The OSG Release Management Process and How it Affects our Community"

publish_on:
  - osg

type: news

canonical_url: "https://osg-htc.org/news/2015/06/01/the-osg-release-management-process-and-how-it-affects-our-community/"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/stock_card.jpeg"
  alt: "Open Science Grid"

description: |
    The OSG community relies on the OSG Software Stack which is composed of grid middleware and the
    OSG-specific configuration scripts. The distribution contains configuration scripts to apply OSG
    recommended settings and a Virtual Organization (VO) package. This package has the list of VOs,
    their authorization, and authentication services.
excerpt: |
    The OSG community relies on the OSG Software Stack which is composed of grid middleware and the
    OSG-specific configuration scripts. The distribution contains configuration scripts to apply OSG
    recommended settings and a Virtual Organization (VO) package. This package has the list of VOs,
    their authorization, and authentication services.

---

The OSG community relies on the OSG Software Stack which is composed of grid middleware and the OSG-specific configuration scripts. The distribution contains configuration scripts to apply OSG recommended settings and a Virtual Organization (VO) package. This package has the list of VOs, their authorization, and authentication services.

Each month a new version of the OSG Software Stack is released. The software contains many individual components that are brought together into a cohesive software release. Although developers have tested their changes, the OSG Release Team verifies the entire release by double-checking that the new changes work as desired. In addition, the OSG Release Team runs acceptance tests to ensure that the software works as a whole.

In each release cycle, a small percentage of tickets (less than 10%) are sent back to developers for rework. On occasion, the OSG Release Team notes areas for improvement and submits a ticket for further work. Components are tested in isolation and in near-production environments. There are two Integration Test Bed (ITB) sites used by the team. If the OSG Release Team doesn’t have access to the requisite environment, they call on OSG system administrators to test an update.

The final check before release tests the entire distribution as a whole over all platforms using automated test tools developed by the software team. The OSG Release Team does its best to deliver a software stack that can be depended on.

Now here’s the viewpoint of a software ticket:

> I am a ticket in the JIRA ticket tracking system. The developer has just marked me “Ready for Testing.” I wonder what kind of testing will be done. The developer has already tried out his changes and run me through the automated tests. I have just been assigned to a tester. The tester has installed my software on a fermicloud VM. He is following a testing recipe that is pushing me in a lot of different directions. I hope that everything still works. I would hate to be one of the few tickets sent back for rework. He has finished following the recipe. Is he done? No, he is trying a couple of new things that haven’t been tried before. Whew, I passed. Wait, now I’m on an ITB site. He wants to see me work in an environment that mirrors the production environment. I’ll have to wait a while to see if I do anything unusual. Finally, the testing is finished. I accumulated quite a history. All the tests and results have been added to my record. One final review hurdle is coming. The release manager is reviewing the tests and results. I hope everything is covered. Whew, he marked me “Ready for Release.” Yay! I get to be part of the next release!

> – Tim Theisen
