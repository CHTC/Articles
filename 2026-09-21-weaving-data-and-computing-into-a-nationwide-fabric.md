---
title: "Weaving data and computing into a nationwide fabric supporting science"

author: Rudy Molinek

publish_on:
  - chtc
  - osg
  - path
  - htcondor
  - fabaid

type: news

canonical_url: "https://morgridge.org/story/weaving-data-and-computing-into-a-nationwide-fabric-supporting-science/"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/fabaid-featured/fabaid-featured.webp"
  alt: "Map of the United States with pins. Illustration: Eleanor Campbell"

banner_src: "https://raw.githubusercontent.com/CHTC/Articles/main/images/fabaid-featured/fabaid-featured.webp"
banner_alt: "Map of the United States with pins. Illustration: Eleanor Campbell"

excerpt: |
  The NSF-funded Fabric for AI-Driven Science (FabAID) builds on decades of CHTC experience in distributed computing to
  connect data repositories, computing capacity, and services for researchers at institutions large and small across
  the nation.
---

<figure>
<img style="width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/fabaid-featured/fabaid-featured.webp" alt="Map of the United States with pins. Illustration: Eleanor Campbell"/>
<figcaption>Illustration: Eleanor Campbell</figcaption>
</figure>

<figure style="float: right; margin: 0 0 1rem 1rem; width: 300px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/anthony-gitter.jpg' class="figure-img img-fluid rounded" style="max-width: 100%; height: auto;" alt="Anthony Gitter">
<figcaption>Anthony Gitter</figcaption>
</figure>

Like other investigators at the Morgridge Institute for Research, [Anthony Gitter's](https://morgridge.org/research/labs/gitter/) research doesn't fit neatly into defined categories. Among other work, Gitter develops computational methods and machine learning models to help him, and his collaborators working in wet labs, engineer proteins that perform chemical reactions in the process of making medicines. To do this work at the highest levels, Gitter needs data — lots of data — along with the computing power to apply that data to biological problems.

Computing-intensive science with large datasets is nothing new, but the rapid expansion of AI has opened up new possibilities to solve problems that were previously hard to tackle for computational analysis. Cutting-edge science in biology and beyond therefore increasingly relies on vast access to computing capacity. That sea change is one reason why Gitter set up his lab within the Morgridge Institute, just down the hall from the [Center for High-Throughput Computing](https://chtc.cs.wisc.edu/), or CHTC.

"There's a difference between CHTC and other computational centers. That difference, in part, is why my lab is housed at Morgridge. Both CHTC and Morgridge have this goal of taking lessons learned, then sharing them out and deploying them — and putting a lot of effort into that piece," says Gitter. "Sometimes in computer science the focus might be on 'what's the machine learning innovation?' My end goal is how can I take these AI methods to do new things and learn about the world."

Now, Gitter is joining a team led by fellow Morgridge investigator [Brian Bockelman](https://morgridge.org/profile/brian-bockelman/) and including Morgridge's [Miron Livny](https://morgridge.org/profile/miron-livny/), [AnHai Doan](https://pages.cs.wisc.edu/~anhai/) from the University of Wisconsin–Madison Department of Computer Sciences, and [Jason Simms](https://www.swarthmore.edu/profile/jason-simms) of Swarthmore College as co-principal investigators on the recently announced project to build a nationwide Fabric for AI-Driven Science, or [FabAID](https://fabaid.io/). This summer, the National Science Foundation [granted FabAID $24.5 million](https://morgridge.org/story/nsf-announces-investment-to-shape-the-nations-future-data-backbone/) over 5 years as part of $83 million in investment in building a data-intensive, AI-capable backbone for national cyberinfrastructure.

<figure style="float: left; margin: 0 1rem 1rem 0; width: 200px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/miron-livny-2021.jpeg' height="300" width="200" class="figure-img img-fluid rounded" alt="Miron Livny">
<figcaption>Miron Livny</figcaption>
</figure>

FabAID, which is led by the CHTC and includes several partner institutions, focuses on bringing access to integrated data systems, computing capacity, and services for researchers at institutions large and small across the nation. The project builds on decades of the CHTC's unique experience in facilitating distributed computing, a process that allows scientists across the country to access computing power remotely and make scientific advances regardless of the on-site computing capabilities their institution offers.

For Livny, research like that done in the Gitter Lab exemplifies both the Morgridge Institute's emphasis on supporting impactful science as well as the scientific value of weaving together data repositories and computing capacity amidst the backdrop of an AI revolution.

"Lots of people are working on speeding up the AI models," says Livny, Morgridge's chief technology officer and John Morgridge professor of computer science at UW–Madison. "The value of Tony is that he really thinks about how to train a model that makes predictions that are tested in elaborate lab efforts."

AI also has the potential to further separate computing "haves" from "have nots." Training AI models for specific scientific applications is [limited by the computing resources](https://nairrpilot.org/projects/highlights/breaking-gpu-bottleneck) available to a scientist, which often depends on their institution. Access to distributed computing levels that playing field and expands the national talent pool of researchers who might make the next big discovery.

## Connecting the threads

FabAID leverages the CHTC's decades-long experience connecting researchers to the computing resources they need to solve pressing problems — from creating [high-tech dairy barns](https://dorealab.cals.wisc.edu/) that monitor animal health and productivity to interpreting [signals from the furthest reaches of the universe](https://www.ligo.caltech.edu/).

The systems are rooted in Livny's pioneering work on distributed computing, which uses software to connect users to available computing capacity. The program, called [HTCondor](https://htcondor.org/), manages and prioritizes computing jobs, sending them wherever computing resources are available to carry them out. For example, a lab at UW–Madison might get priority on their own servers but instead of sitting dormant when not being used locally, a job entered by a researcher at Swarthmore could swoop in and run on those resources until requested by a local user.

<figure style="float: right; margin: 0 0 1rem 1rem; width: 200px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/christina-koch-square.jpg' class="figure-img img-fluid rounded" style="max-width: 100%; height: auto;" alt="Christina Koch">
<figcaption>Christina Koch</figcaption>
</figure>

While choreographing this intricate dance, and ensuring it goes on even when unexpected obstacles arise, is a fundamental problem in computer science that's interesting in its own right, CHTC translates it to software tools that are putting it into practice.

"I think of it as how much science can we do with a given set of computers and have the biggest impact over time," says Bockelman. "If I give you a GPU, if I give you a cluster, how much high-quality science can you do?"

[Christina Koch](https://www.cs.wisc.edu/staff/koch-christina/), lead research computing facilitator at the CHTC, adds that "we're advancing the state-of-the-art of high-throughput computing as a discipline of its own, but also as a tool that people use to do core science."

Such work relies not just on technical capacity and acumen, but on the community of researchers and institutions willing to share resources. Successfully running a distributed computing system is as much about people as it is about machines. To that end, CHTC has long led several nationwide services, like [OSPool](https://osg-htc.org/services/ospool/) that's built with HTCondor and the [Open Science Data Federation](https://osg-htc.org/services/osdf) that's powered by the CHTC's [Pelican Platform](https://pelicanplatform.org/). Previously, these efforts were united under the NSF-funded [Partnership to Advance Throughput Computing](https://path-cc.io/), or PATh, which provides the organizational and technological foundation for FabAID.

"Not every campus is going to run a 100,000-core supercomputer — that's not needed everywhere," says Koch. "There's a point where it's really important to use the principle that we can do more together than we can individually."

In other words, FabAID is built on the commitment of the two organizations that form the PATh partnership — CHTC and the [OSG Consortium](https://osg-htc.org/) — to the idea that a nationwide computing fabric can support science more strongly than disconnected threads.

## "Data is really the revolution"

FabAID is designed to leverage high-throughput computing methods and technologies to meet the rapidly rising use of AI in science. Building and training AI models that move science forward certainly benefits from the services provided by HTCondor and the computing capacity offered by the OSPool, but the task also requires a foundation of high-quality data like that reachable through the OSDF to create reliable outcomes.

"Data is the life stream of any potential for AI to deliver value to science," says Livny. "Our ability to collect and process data is really the revolution."

<figure style="float: left; margin: 0 1rem 1rem 0; width: 200px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/BrianBockelman.jpeg' height="300" width="200" class="figure-img img-fluid rounded" alt="Brian Bockelman">
<figcaption>Brian Bockelman</figcaption>
</figure>

> "I want all these advanced cyberinfrastructure tools to become simple enough, become straightforward enough, that they can have a presence at a university of any size."
>
> — Brian Bockelman

As advancing technologies — be it a camera system in a dairy barn or a cosmic detector buried deep [within the South Pole's ice](https://icecube.wisc.edu/about-us/overview/) — continuously generate streams of data, the linkages between those trillions of bytes of information and the computer chips researchers use to process them are increasingly important. In many cases, it's not feasible to have the necessary data stored on the same machine that will process and analyze them.

"Often in computing people think of a dichotomy between data and computing, and those are treated separately," says Bockelman. "But for the most part, they're really intertwined. You can't create an AI model without the data to train it on. So, we want to design services that provide connectivity to both."

"We're creating a fabric that connects data and compute capacity seamlessly," adds Simms.

In addition to supporting new AI models that push science forward, the FabAID team aims to use AI-based interfaces, similar to familiar ones like ChatGPT or Claude, to help researchers get up and running on high-throughput computing without needing specialized, hands-on training or extended startup times.

"In some cases, AI is itself the science that you're doing. In others, the AI is there as a tool to do your science better," says Bockelman.

## Including every institution in FabAID design

<figure style="float: right; margin: 0 0 1rem 1rem; width: 200px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/fabaid-featured/jason-simms.jpg' height="300" width="200" class="figure-img img-fluid rounded" alt="Jason Simms">
<figcaption>Jason Simms</figcaption>
</figure>

In the United States, the [vast majority](https://www.equityinhighered.org/indicators/enrollment-in-undergraduate-education/undergraduate-enrollment-across-sectors-and-carnegie-classifications/) of undergraduate students attend non-[research 1](https://carnegieclassifications.acenet.edu/carnegie-classification/classification-methodology/2025-research-activity-designations/), so-called "R1," institutions, which are less likely to operate extensive computing resources. FabAID is built on the idea that supporting the most state-of-the-art computing tools in every educational and research setting, including institutions like liberal arts or community colleges, is an important part of developing a modern workforce and training a data-literate public for an age of AI.

"I want all these advanced cyberinfrastructure tools to become simple enough, become straightforward enough, that they can have a presence at a university of any size," says Bockelman. "I don't want to tell people there's this great computing power, this wonderful thing called FabAID, and all you have to do is come to UW–Madison. I don't think that's enabling or empowering."

Another advantage of expanding to include small institutions is that it's easier to scale a project up than to run a system designed for the most highly resourced researchers in a classroom. With FabAID, the team hopes this bottom-up approach, which includes connection from Simms to small institutions across the country, will help faculty everywhere use computing to blur the distinctions between education and science — something many of them already do.

"At small institutions, the line between teaching and research is essentially nonexistent," says Simms. "Faculty bring their research into the classroom and that becomes part of the pedagogical experience."

But, as exploring questions with real-world implications and value requires ever-larger datasets, instructors sometimes find themselves compromising to stay within their institution's computing capacity. "What often ends up happening is that they have to use more trivial datasets — subsets or fake data," adds Simms. "By leveraging tools like what we're developing with FabAID, it makes it more possible to engage in research and teaching while making the experience a lot more real and meaningful for the students."

A computing approach that lowers the barrier to entry could also unlock the scientific potential held by the students who attend these smaller institutions. Gitter has experienced this firsthand in his own research partnerships.

"I've seen that with some of my collaborators who are at primarily undergraduate institutions research really ramps up in the summer, so they don't want to spend a month and a half learning how to use a supercomputer system," says Gitter. "CHTC has a lot of partners like this already; I've worked with them. It's now a question of taking those good things and making them even stronger."
