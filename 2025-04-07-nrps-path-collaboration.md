---
title: Bringing The National Research Platform Capacity to the HTC Community
author: Jordan Sklar and Kallen Wank
publish_on:
    - chtc
    - htcondor
    - osg
    - path
type: user
excerpt: "The National Research Platform (NRP) uses PATh resources to create an open cyberinfrastructure."
canonical_url: https://path-cc.io/news/2025-04-07-nrps-path-collaboration/
image: 
  path: https://raw.githubusercontent.com/CHTC/Articles/main/images/nrp/sdsc.jpg
  alt: "San Diego Supercomputer Center, home of NRP"
---

<figure>
<img style="width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/nrp/sdsc.jpg" alt="The San Diego Supercomputer Center, home of NRP."/>
<figcaption>The San Diego Supercomputer Center, home of NRP.</figcaption>
</figure>

## NRP’s Collaboration with PATh

“Creating an open infrastructure that supports both horizontal and vertical growth is the goal,” of [National Research Platform](https://nationalresearchplatform.org/)’s collaboration with [the Partnership to Advance Throughput Computing (PATh)](https://path-cc.io/), reported [Frank Wuerthwein](https://www.sdsc.edu/research/experts/wuerthwein_frank.html), Principal Investigator of NRP and Executive Director of the [OSG](https://osg-htc.org/). Supported by the [National Science Foundation (NSF)](https://www.nsf.gov/)’s [Office of Advanced Cyberinfrastructure (OAC)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2112167&HistoricalAwards=false) award among other funding sources, NRP is a growing community focused on creating an open cyberinfrastructure. NRP aims to provide accessible and scalable computing resources by enabling institutions to share their hardware, which fosters collaboration and advances scientific research across diverse research communities. It also serves as a way to engage with the [OSPool](https://osg-htc.org/services/open_science_pool.html), a source of computing capacity that is accessible to any researcher affiliated with a US academic institution.



In an interview with [Frank Wuerthwein](https://www.sdsc.edu/research/experts/wuerthwein_frank.html), he spoke about the NRP's collaboration with [PATh](https://path-cc.io/). Expanding on the goal of the collaboration, he described horizontal growth as the expansion of the network by allowing different individuals and campuses to share and integrate their hardware resources, which increases the overall computing capacity. Vertical growth, on the other hand, refers to building on this shared infrastructure by adding new services, tools, and applications that can address the unique needs of different research communities. “You can deploy an entire service infrastructure that totally does something new for a different community on top of what we provide,” Wurthwein added.



NRP supports a ‘bring your own resource’ model and continues to expand across campuses nationwide. The NRP has tripled the computing resources available to the community, since the beginning of its NSF funded operations in 2023. Research groups such as the [IceCube Neutrino Observatory](https://icecube.wisc.edu/), [the National Radio Astronomy Observatory (NRAO)](https://public.nrao.edu/), and others contribute to computing capacity. Wuerthwein explained that “when someone contributes to the OSPool through the NRP, they don’t need to manage their own cluster systems. Instead, they can hand over control to the NRP team.”



### How Does NRP Work?

<figure style="float: right; margin: 0 1rem 0 1rem;">
 <img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/nrp/frank.jpg' height="300" width="200" class="figure-img img-fluid rounded" alt="Frank presenting at HTCXX Conference">
</figure>

One of the biggest benefits of working with the NRP is that it simplifies the process of contributing to OSPool, allowing for more accessibility. When a project like IceCube submits a job to OSPool, they can leverage NRP services, which function like a single campus cluster. “Under this hood is hardware from more than 70 different locations supporting the infrastructure,” Wuerthwein said, which allows the NRP to install the software for the specific group.

Wuerthwein also mentioned that the NRP integrates their global Kubernetes infrastructure, which is like a "smart manager" for application containers. [Kubernetes](https://kubernetes.io/docs/tutorials/kubernetes-basics/) can be deployed, scaled, and managed across multiple servers (called nodes) in a cluster and automatically can handle things like restarts, updates, and load balancing, so you don't have to intervene manually. The NRP uses Kubernetes to “build services on top of it, as it is a container deployment tool.” Kubernetes also increases the flexibility and scalability of the infrastructure, making it easier for the NRP to manage. “The amount of effort required to join the OSPool via the NRP is vastly smaller than it would be otherwise be because NRP provides a lot of the system infrastructure, e.g. operating and batch systems, that the hardware owner no longer needs to operate,” Wuerthwein stated when describing how the relationship with OSG Consortium comes into play.

### PATh and NRP Working Together

PATh and the NRP share similar goals and work together to achieve them. The NRP contributes resources to PATh that are integrated into the OSPool, and also share their global NRP Kubernetes cluster for PATh to deploy the [Open Science Data Federation (OSDF)](https://osg-htc.org/services/osdf.html) into. PATh thus uses the vertical openness of NRP to deploy OSDF on top of NRP. This sharing of resources allows the OSDF to more easily achieve a global footprint by building on the global footprint of NRP.

Wuerthwein also elaborated on how the NRP leverages PATh’s [Pelican services](https://pelicanplatform.org/). “We offer OSDF to the NRP community of researchers. OSDF is instantiated using Pelican software, deployed as services by PATh on NRP operated hardware worldwide. OSDF is thus available to both the NRP and the OSPool communities of researchers.” Wurthwein said.

In addition to contributing to the OSPool, the NRP also uses its infrastructure for direct computing services. Wurthwein explained that users accessing the NRP through different mechanisms, like JupyterHub or Kubectl, can still gain access to the OSDF, facilitated by the Pelican platform.

### Impact

The NRP works with all types of campuses and groups, offering tailored support based on each institution’s resources and capabilities. “Four-year and teaching colleges with limited research portfolios often lack the infrastructure for research computing, so we allow them to own hardware without having to operate that hardware beyond connecting it to power and networking,” Wurthwein explained.

“What we [NRP] do is lower the bar for entry so that even institutions who don’t necessarily have the investment capabilities or location to find skilled system administrators can still offer their faculty and students the hardware infrastructure,” Wurthwein commented. The NRP welcomes campuses to contribute capacity regardless of how big or small they are, and this leads to a more open infrastructure and community. In addition to empowering smaller educational institutions, it also integrates hardware at regional research and education networking (REN) organizations. Operating compute clusters is typically outside of the scope of the RENs. By working with NRP, the RENs across the USA can offer compute and storage hardware hosting to smaller colleges within their regional communities. The collaboration of REN, NRP and PATh is a very powerful enabler of even the smallest colleges across the USA.

Wuerthwein spoke of NRP’s goals to spread across the whole community. He noted that NRP bridges the gaps between small institutions and access to resources and funding for clusters. Wurthwein explained that NRP helps close these disparities by providing operation and hardware support.

### Community

Working as a community is one of the NRP’s biggest strengths, and Wurthwein explained how this helps them reach their goals. “There are about 3900 institutions of higher learning in just the US, and in order to make research and education accessible to all, you have to work together and use scaling rules to minimize costs,” Wuerthwein stated. The NRP has built their community on collaborative hardware and networks, which in turn allow these smaller campuses to get involved. He compared small campuses to larger ones, “there is an efficiency of scale argument to be made with adding hardware, so we are able to allow many smaller institutions to own hardware as if they were a University of Wisconsin, for example,” Wuerthwein said.

The NRP is able to leverage resources and costs for all types of institutions, allowing for small-teaching colleges to operate hardware like larger ones. Wuerthwein explained that as well as increasing access to resources, NRP navigates and lowers costs as “none of them need the resources all the time,” but as a collective on the NRP, will help increase cyberinfrastructure capacity nationwide.

“In the end, we are building an open infrastructure for the community, owned and built by the community” Wuerthwein concluded.
