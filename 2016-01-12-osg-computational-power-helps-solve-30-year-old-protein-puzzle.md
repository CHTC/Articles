---
title: "OSG computational power helps solve 30-year old protein puzzle"
author: Greg Moore

publish_on:
  - osg

type: news

canonical_url: "https://osg-htc.org/news/2016/01/12/osg-computational-power-helps-solve-30-year-old-protein-puzzle/"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-huang.png"
  alt: "Po-Ssu Huang"

description: |
    As computational power expands the horizons of protein research, vast new possibilities to design
    proteins for disease treatment are opening up. Thanks to the power of the Open Science Grid (OSG),
    protein researchers recently overcame an obstacle that has vexed scientists for nearly 30 years.
excerpt: |
    As computational power expands the horizons of protein research, vast new possibilities to design
    proteins for disease treatment are opening up. Thanks to the power of the Open Science Grid (OSG),
    protein researchers recently overcame an obstacle that has vexed scientists for nearly 30 years.

card_src: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-huang.png"
card_alt: "Po-Ssu Huang"

---

<figure class="figure float-end" style="margin-left: 1em; width: 250px;">
  <img src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-huang.png" class="figure-img img-fluid rounded" alt="Po-Ssu Huang" width="250px">
  <figcaption class="figure-caption">Po-Ssu Huang. Photo courtesy Po-Ssu Huang.<br/></figcaption>
</figure>

As computational power expands the horizons of protein research, vast new possibilities to design proteins for disease treatment are opening up. Thanks to the power of the Open Science Grid (OSG), protein researchers recently overcame an obstacle that has vexed scientists for nearly 30 years.

The cylindrical TIM-barrel (triosephosphate isomerase-barrel) protein fold occurs widely in enzymes, making it an attractive target for designing similar protein structures *de novo*—that is, designing them using computational models.  An international team of researchers from Baker Lab at the University of Washington, National Autonomous University of Mexico and Hoecker Lab at the Max Planck Institute for Developmental Biology in Germany created a breakthrough computational simulation of a TIM-barrel protein that will be critical to a new generation of custom-designed enzymes. Their results have been published in [Nature Chemical Biology](http://www.nature.com/nchembio/journal/vaop/ncurrent/full/nchembio.1966.html).

<figure class="figure float-start" style="margin-right: 1em; width: 350px;">
  <img src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-protein.png" class="figure-img img-fluid rounded" alt="Image from a calculation used in the design of a TIM-barrel protein" width="350px">
  <figcaption class="figure-caption">Image from a calculation used in the design of a TIM-barrel protein. Image courtesy Po-Ssu Huang.<br/></figcaption>
</figure>

Po-Ssu Huang, one of the lead researchers on the paper and a research scientist at the [Baker Lab](http://www.bakerlab.org/) at the [University of Washington](http://www.washington.edu/), has been part of developing HIV vaccines. He is currently studying the sequence structure relationships of protein folds and building new proteins using computational models. As he explains, “The TIM-barrel computational model is an example of what we do here in the lab to take what we learn to build new proteins for other applications.” Huang earned his PhD in biochemistry and molecular biophysics from the California Institute of Technology (Caltech) and has worked with the Baker Lab as a postdoc and research scientist.

“What we do involves computational algorithms, but at the same time everything we design is actually tested here in the lab,” Huang said. “We take virtual simulations to practical applications—turning these molecules into new functional molecules for the real world.” In addition to designing vaccines and building new enzymes, Huang and his colleagues are interested in developing disease sensors and drug detectors using proteins as binders for small molecules.

A large aspect of their work is understanding proteins and controlling three-dimensional structures to achieve particular goals. Huang specializes in modeling de novo structures and building protein structures from scratch. “The same tools can be used for sculpting naturally occurring proteins,” Huang said. “We can also repurpose proteins—vaccines being an example. We can take a viral protein and hack the structure in a way that reduces an immune response, so a given molecule can be repurposed.”

For the TIM-barrel computational model, Huang used the OSG to scale up his simulations. “In order to build a structure, we have to first define the topology—how the elements come together,” Huang said. “In this case, the structure forms a donut. The ends must meet. To achieve those geometric requirements in practice, we had to set up many different connectivity scenarios and lengths. We then used the OSG to run simulations to find out which ones are viable—we needed a fast way to find the right candidates. The massive computing power of the OSG allowed us to quickly get answers.”

In the past year, the Baker Lab used an average of 46,000 core OSG hours per week for 52 weeks, or a total of around 2.4 million core hours.

Mats Rynge, a computer scientist at the Information Sciences Institute of the University of Southern California and a member of the OSG User Support team described the setup: “Baker Lab has its own local [HTCondor](http://research.cs.wisc.edu/htcondor/) submit host that is connected to the OSG VO’s HTCondor infrastructure. Jobs submitted on the host are automatically scheduled onto available resources across the OSG. The benefit of this setup (submit locally—compute globally) is that the group can maintain its own submit host. It can manage users, access, and upgrades without worrying about maintaining the computing infrastructure.”

In order to make significant progress in disease treatment, the researchers need a comprehensive understanding of protein sequence and structural relationships.

“This area is poorly defined,” Huang said. “We can only dig into a structural database to try to understand protein structures. Taking a snapshot of something in nature doesn’t reveal the rules of how the structure is achieved. Sometimes the physical model we have does not allow us to identify the elements present, and we can never have a good enough simulation to describe the problem. When a chain of amino acids adopts multiple conformations, the energy signature is sometimes not there and this makes it very difficult to understand. The Holy Grail here is to understand enough to build new things. This has implications for neuroscience, industrial applications, biotech, enzymes for drug delivery, vaccines for HIV, and proteins that can inhibit Ebola. It’s a huge field. This is where computer simulation comes in, and the faster the better. The OSG definitely fits the need.”
