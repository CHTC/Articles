---
title: OSPool and Computing Power Helps Researchers Design New Proteins

author: Sophie Dorros
publish_on:
- htcondor
- path
- osg
- chtc
type: user
canonical_url: "<https://chtc.cs.wisc.edu/OSPool and Computing Power Helps Researchers Design New Proteins.html>"

tag:
- chtc_featured_article

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/protein-design/visual-2-by-1.jpeg"
  alt: Mukul Sherekar pictured with protein structure

excerpt: Where to find freely available GPU and CPU computing resources for their research on diseases like Alzheimers, Parkinsons, and ALS? This challenge faced by labs and researchers is becoming more acute with the increasing use of AI and machine learning (ML) which demand more computing capacity. For Dr. Priyanka Joshi’s Biomolecular Homeostasis and Resilience Lab at Georgetown University, the National Science Foundation (NSF) supported OSPool and its HTCondor system was the answer.

---


Where to find freely available GPU and CPU computing resources for their research on diseases like Alzheimers, Parkinsons, and ALS? This challenge faced by labs and researchers is becoming more acute with the increasing use of AI and machine learning (ML) which demand more computing capacity. For Dr. Priyanka Joshi’s Biomolecular Homeostasis and Resilience Lab at Georgetown University, the National Science Foundation (NSF) supported OSPool and its HTCondor system was the answer.

The Joshi Lab is investigating how the normal balance inside cells starts to break down during aging in neurodegenerative diseases. Their research uses biophysical, biochemical, and machine learning approaches to explore fundamental mechanisms in cellular and organismal biology, focusing on the unpredictable nature of protein misfolding in aging.

<figure style="float: left; margin: 0 1rem 1rem 0;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/protein-design/standing.jpg' height="400" width="300" class="figure-img img-fluid rounded" alt="Erik smiling">
<figcaption style="width:300px">
Pictured: Mukul Sherekar with protein structure in the Joshi Lab.
Credits: Mukul Sherekar
</figcaption>
</figure>

Working in Joshi’s Lab, Mukul Sherekar uses publicly available ML algorithms and protein language models to design new proteins for the lab. Sherekar started working in the Joshi lab as a Protein Designer in August, aiming to use his background in protein science, structural biology, and machine learning to design new proteins. Sherekar established early on that his data set would require a large amount of GPUs, a kind of computer chip that are effective in doing tasks related to machine learning, However, GPUs are both expensive and in demand and campuses have limited GPU resources and capacity.

After reading UW-Madison graduate and current Morgridge Institute for Research ML scientist Sam Gelman’s publication on his research using publicly available OSG resources, Sherekar realized the OSPool would be a good fit for his own work. The OSPool, freely available  to researchers associated with a US institution, provides a much larger GPU infrastructure. Sherekar noted that “For those reasons, I think OSPool perfectly suits people who are in academia and who cannot get access to hardware resources easily.” Sherekar reached out to Gelman, who pointed him in the direction of the Center for High Throughput Computing at UW-Madison, which in partnership with the PATh project, provides the services in support of the OSPool.

<figure style="float: right; margin: 0 1rem 0 1rem;">
 <img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/protein-design/visual.jpg' height="210" width="400" class="figure-img img-fluid rounded" alt="Erik in the wet lab">
<figcaption style="width:400px">
Integrative Analysis of Metabolite-Protein Conformational Landscapes. Credits: Joshi Lab
</figcaption>
</figure>

Since creating an OSPool account in August, the Joshi Lab has run over 254,082 jobs, and logged over 1,126 GPU hours and 1,631,905 core CPU hours in the OSPool.

Sherekar’s two types of jobs; data collection and running protein language models, required the help of two main software suites. The first, HTCondor developed by the CHTC, utilizes the power of a network of clustered computers, splitting tasks into simultaneously running self-contained tasks, providing results that could have taken months to years to complete using a singular system. Then the second, the Rosetta Software Suite, is a protein modeling and design toolkit that uses algorithms to predict protein design structures. Sherekar collects information about his proteins using the Rosetta Software Suite, using a set of tools through which more information about biophysical properties of the proteins is collected. Sherekar then leverages HTCondor to create a workflow at a large scale impossible previously.

The relationships the Facilitation Team are able to build with researchers through office hours and email helped Sherekar navigate using the OSPool. The team, led by lead Christina Koch, jumped in, offering weekly virtual office hours and personalized troubleshooting. Reflecting on navigating GPU usage in the OSPool, Sherekekar noted “There were certain times when I got the GPU and my code to run perfectly.” Other times “I requested GPUs  and [then] realized my code was not running.” Addressing this problem, research computing facilitator Amber Lim suggested using containers, an approach that bundles everything your application needs so it runs the same everywhere. Adding to the use of containers along with some self troubleshooting, Sherekar was able to solve the issue and continue utilizing the GPU capacity he needed. He added: “It's a good way to learn about ….a high throughput computing system, like how things work. So I'm learning every day.” Utilizing both help from the Facilitation Team and his own ML expertise, Sherekar is able to troubleshoot his issues and learn more about throughput computing systems in the process, all while further advancing his research work.

In addition to required GPUs, the protein designing project requires increased availability of CPUs, also accessed through the OSPool. Sherekar states plainly that “I wouldn’t have been able to do my project… or it would have cost [my lab] a lot of money.” Moving forward, Sherekar and the Joshi Lab will continue to use HTCondor and OSPool resources to design novel proteins to address the effects of aging in neurodegenerative diseases.  
