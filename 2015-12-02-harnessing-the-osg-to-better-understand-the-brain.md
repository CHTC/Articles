---
title: "Harnessing the OSG to better understand the brain"
author: Greg Moore

publish_on:
  - osg

type: news

canonical_url: "https://osg-htc.org/news/2015/12/02/harnessing-the-osg-to-better-understand-the-brain/"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-mECoG.jpeg"
  alt: "mECoG"

description: |
    Using electrical information recorded outside the brain, Ricardo Pizarro at the University of
    Wisconsin-Madison (UW-Madison) is trying to estimate network models in rodent brains. This research
    may one day help people with artificial limbs move a robotic arm using a real-life application
    called a brain-computer interface.
excerpt: |
    Using electrical information recorded outside the brain, Ricardo Pizarro at the University of
    Wisconsin-Madison (UW-Madison) is trying to estimate network models in rodent brains. This research
    may one day help people with artificial limbs move a robotic arm using a real-life application
    called a brain-computer interface.

card_src: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-mECoG.jpeg"
card_alt: "mECoG"

---

Using electrical information recorded outside the brain, Ricardo Pizarro at the University of Wisconsin-Madison (UW-Madison) is trying to estimate network models in rodent brains. This research may one day help people with artificial limbs move a robotic arm using a real-life application called a brain-computer interface. The technology is also aimed at helping those who have suffered a cerebral stroke and are unable to move a side of their body.

Pizarro works in the NITRO lab (Neural Interface Technology Research and Optimization, part of the Department of Biomedical Engineering at UW-Madison) led by Dr. Justin Williams. Their network models are computationally expensive, so Pizarro and the lab use the Open Science Grid (OSG) to do large simulations. UW-Madison is a key OSG site—in 2014 alone, the Center for High Throughput Computing (CHTC) provided an additional 22 million CPU hours to campus researchers via the OSG.

*Figure 1, below, Photo of a micro-ECoG; courtesy Ricardo Pizarro*

<figure>
<img style="max-width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-mECoG.jpeg" alt="mECoG"/>
</figure>

The NITRO lab designs and surgically implants small electronic sensors to record local field potentials from a small population of neurons in the brain. The sensors are similar to Electrocorticography (ECoG) arrays but 100 times smaller.

“Putting it in perspective, Electroencephalogram sensors (EEGs) sit outside the skull,” says Pizarro. “EEGs are noninvasive, which is great—but you don’t get good spatial resolution like you do with ECoGs that are surgically implanted below the skull but above the dura, making them minimally invasive. We use cutting-edge micro-ECoG technology that requires even smaller craniotomies and records higher quality signals because we record from a smaller area with higher density electrodes.”

<figure>
<img style="max-width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-setup.jpeg" alt="setup"/>
<figcaption>Figure 2, right, NITRO lab uses cutting-edge micro-ECoG technology that requires even smaller craniotomies and records higher quality signals because they record from a smaller area with higher density electrodes. Illustration courtesy Ricardo Pizarro.</figcaption>
</figure>

The effective network model NITRO uses to see how brain regions are connected is called a dynamic causal model. “First, we stimulate and measure potentials from the brain using micro-ECoG sensors. The novel network model takes that information and tries to predict how these cortical regions are connected,” explains Pizarro. “The algorithm looks for a set of parameters that will try to estimate a network and quantify how well the network explains the data being recorded. Before using the OSG and CHTC, we had difficulties with the algorithm. Now, we can initialize the algorithm with different starting points—up to 10,000 different points, let it run, and find out which one is best, using an objective measure.”

This brute force method shows which network pattern is most likely to match the data being revealed. In addition to possible starting points, the researchers use over 50 parameters to estimate connectivity from two brain regions—extrinsic connections between regions, and intrinsic connections within a region.

“With the OSG, we can explore all 50 parameters, make sure we are not missing anything, and use the 10,000 different starting points to make sure we’ve covered all the ground we need to,” says Pizarro. “You can imagine how difficult it was previously using a desktop computer. Running just 1,000 initial conditions would take a whole week. On the OSG/CHTC, running 10,000 parameters takes two days. This empowers us to optimize our methods and algorithms so we can explore more efficiently and ask more questions.”

<figure>
<img style="max-width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-4layer-CMC-2populations.jpeg" alt="4layer-CMC-2populations"/>
<figcaption>Figure 3 illustrates a network model. The canonical microcircuit (CMC) is implemented as a dynamic causal model (DCM).  Extrinsic connections of the CMC are shown for two cortical columns. The forward and backward connections are illustrated as solid and dashed lines, respectively.  Illustration courtesy of Ricardo Pizarro.</figcaption>
</figure>

Pizarro needed to modify his code to run on OSG/CHTC resources, but he got help from CHTC’s Lauren Michael. “Once we had that figured out, the return was much greater than the expenditure of time,” says Pizarro. “We are able to do so much more than on a desktop. We run these 10,000 initialization conditions in parallel using OSG, saving orders of magnitude in time. Using OSG allows me to iteratively explore our algorithm more thoroughly and efficiently. The OSG is ideal for scientists running computations in parallel.” In addition to developing the new sensors, the NITRO lab is attempting to make them safe enough for human use and durable enough to be long-term implants. The ultimate goal is for the sensors to be useful in clinical situations, helping people with motor disabilities communicate with and control prosthetic devices using the brain-computer interface. OSG computing resources are accelerating the process.
