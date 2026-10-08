---
title: "Behind Nobel-winning IceCube discoveries, decades of high-throughput computing"

author: Emma Frankham and Rudy Molinek

publish_on:
  - chtc
  - htcondor
  - osg
  - path
  - pelican

type: news

canonical_url: "https://morgridge.org/story/behind-nobel-winning-icecube-discoveries-decades-of-high-throughput-computing/"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/icecube-nobel/icl-night.jpg"
  alt: "The IceCube Neutrino Observatory at night. Credit: John Hardin, CC-BY4.0"

excerpt: |
  UW–Madison physicist Francis Halzen has been named a 2026 Nobel laureate in physics for his work as principal
  investigator of the IceCube Neutrino Observatory. Over the course of that work, IceCube researchers have developed a
  longstanding collaboration with the Center for High Throughput Computing.
---

<figure>
<img style="width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/icecube-nobel/icl-night.jpg" alt="The IceCube Neutrino Observatory at night. Credit: John Hardin, CC-BY4.0"/>
<figcaption>The IceCube Neutrino Observatory at night. Credit: John Hardin, CC-BY4.0</figcaption>
</figure>

<figure style="float: right; margin: 0 0 1rem 1rem; width: 200px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/icecube-nobel/francis-halzen.jpg' height="300" width="200" class="figure-img img-fluid rounded" alt="Francis Halzen">
<figcaption>Francis Halzen</figcaption>
</figure>

University of Wisconsin–Madison physicist Francis Halzen has been [named a 2026 Nobel laureate in physics](https://news.wisc.edu/university-of-wisconsin-madison-professor-francis-halzen-named-2026-nobel-laureate-in-physics/), marking a major recognition for his work as principal investigator of the IceCube Neutrino Observatory, the world’s largest neutrino telescope, and the discovery of high-energy neutrinos of astrophysical origin. Over the course of that work, IceCube researchers have developed a longstanding collaboration with the [Center for High Throughput Computing](https://chtc.cs.wisc.edu/) (CHTC), a joint endeavor of the Morgridge Institute for Research and the Department of Computer Sciences within UW–Madison’s College of Computing & Artificial Intelligence.

Every day, the [IceCube Neutrino Observatory](https://icecube.wisc.edu/), located in Antarctica, uses 5,000 optical sensors buried in glacial ice to capture over 200 million cosmic rays. This generates a terabyte of data daily, of which about 100 gigabytes are transmitted via satellite for analysis. Hidden within this array of background noise are rare collisions of neutrinos with atomic nuclei, events that provide insights into phenomena including supermassive black holes and exploding stars. Processing these observations involves large-scale simulations that require substantial computing power, helping researchers identify meaningful signals among the complex information.

> “Without CHTC and OSPool resources, we would simply be unable to make any of IceCube’s groundbreaking discoveries.”
>
> — Francis Halzen, Nobel laureate

To meet those ever-growing computing workloads, IceCube researchers have relied on technologies and services provided by the CHTC. That includes access to computing capacity harnessed from across the world, which is managed by the CHTC on the Madison campus, and across the US via the Open Science Pool (OSPool). To do this, researchers use the CHTC’s HTCondor Software Suite and the Pelican Platform to distribute millions of computational tasks and data across available resources.

For example, in a 2019 NSF-funded effort, these technologies enabled IceCube to harness more than 51,000 GPUs provided by three commercial cloud providers for two hours — representing 5 percent of the annual IceCube simulation workload. In the past year alone, IceCube ran over 53 million jobs using CHTC and OSPool resources, totaling over 79 million CPU hours and 2 million GPU hours involving 11 million gigabytes of data.

<figure style="float: left; margin: 0 1rem 1rem 0; width: 200px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/icecube-nobel/miron-livny-2021.jpg' height="300" width="200" class="figure-img img-fluid rounded" alt="Miron Livny">
<figcaption>Miron Livny</figcaption>
</figure>

UW–Madison computing support for Halzen’s research predates both IceCube and the CHTC. In the late 1990s, [Terry Millar](https://news.wisc.edu/millar-remembered-for-contributions-to-mathematical-logic-science-education/), then a mathematician at UW–Madison and associate dean for physical sciences, contacted [Miron Livny](https://morgridge.org/profile/miron-livny/) to help with computing needs in the hunt for neutrinos. Livny, now the John P. Morgridge professor of computer science and Morgridge’s chief technology officer, developed the distributed computing software that underlies much of the CHTC’s work. Eventually, these computing resources helped support [AMANDA](https://icecube.wisc.edu/data-releases/2008/09/amanda-7-year-data/), the Antarctic Muon and Neutrino Detector Array experiment led by Halzen and collaborators that demonstrated the potential for using Antarctic ice to detect high-energy neutrinos produced by cosmic phenomena. As that work grew into IceCube, the CHTC continued to provide the computing capacity and technologies needed to analyze increasingly large and complex datasets.

“Francis Halzen and the IceCube team have accomplished something extraordinary, and we are incredibly excited to see their work recognized with a Nobel Prize,” said Remzi Arpaci-Dusseau, founding dean of the College of Computing & Artificial Intelligence. “It’s also rewarding to know that CHTC played a role in supporting this work over many years. IceCube is a powerful example of the impact of research computing and translational computer science — building the tools and infrastructure that make discovery possible across disciplines.”

That work has been sustained by long-term support from the National Science Foundation, UW–Madison, and the Morgridge Institute for Research, with funding from the Wisconsin Alumni Research Foundation also playing a critical role.

The relationship with IceCube is an exemplar of the CHTC’s broader translational computer science work: innovating computing methodologies, building and operating services, and putting them in the hands of visionary researchers to work on complex scientific problems. “The job of the domain scientist is to challenge us to do things that we cannot currently do, so they can take their science to the next level. Halzen and the IceCube team have been continuously challenging us to do more computing with the available effort and computing capacity,” said Livny. “This Nobel Prize motivates us to push forward and make sure that our campus is ready for the next Francis.”

<figure style="float: right; margin: 0 0 1rem 1rem; width: 200px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/icecube-nobel/BrianBockelman.jpg' height="300" width="200" class="figure-img img-fluid rounded" alt="Brian Bockelman">
<figcaption>Brian Bockelman</figcaption>
</figure>

Research supported by the CHTC has now contributed to four Nobel Prize-winning efforts. In addition to IceCube, this includes the discovery of the Higgs boson particle in [2013](https://www.nobelprize.org/prizes/physics/2013/summary/), the detection of gravitational waves in [2017](https://www.nobelprize.org/prizes/physics/2017/press-release/), and computational protein design in [2024](https://www.nobelprize.org/prizes/chemistry/2024/press-release/).

“At the computing level, we have the capability to enable a broad spectrum of science,” said [Brian Bockelman](https://morgridge.org/profile/brian-bockelman/), a Morgridge investigator and part of CHTC’s leadership. “Three or four of these ideas might win the Nobel Prize, but it’s the same underlying technology, the same ideas, and the same philosophy that’s used by researchers across the campus and around the nation.”

<div style="clear: both;"></div>

You can also read this story [here](https://cai.wisc.edu/2026/10/07/high-throughput-computing-behind-nobel-winning-icecube-discoveries/) from the College of Computing & Artificial Intelligence.
