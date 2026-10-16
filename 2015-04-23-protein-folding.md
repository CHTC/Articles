---
title: "Studying Protein Folding Benefits from Computational Power"
author: Greg Moore

publish_on:
  - osg

type: news

canonical_url: "https://osg-htc.org/news/2015/04/23/protein-folding/"

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-jinbo_xu.jpeg"
  alt: "Picture of Jinbo Xu"

description: |
    Proteins are key to our bodies functioning properly, while abnormal modifications of proteins or
    improperly functioning proteins are often a cause of pathological and disease conditions. Proteins
    also interact with other molecules to make our bodies function properly or, at times, improperly.
excerpt: |
    Proteins are key to our bodies functioning properly, while abnormal modifications of proteins or
    improperly functioning proteins are often a cause of pathological and disease conditions. Proteins
    also interact with other molecules to make our bodies function properly or, at times, improperly.

card_src: "https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-jinbo_xu.jpeg"
card_alt: "Picture of Jinbo Xu"

---

Proteins are key to our bodies functioning properly, while abnormal modifications of proteins or improperly functioning proteins are often a cause of pathological and disease conditions. Proteins also interact with other molecules to make our bodies function properly or, at times, improperly.

<figure>
<img style="max-width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-jinbo_xu.jpeg" alt="Picture of Jinbo Xu"/>
</figure>

Professor Jinbo Xu studies protein folding—how a protein takes on its functional shape—at the [Toyota Technological Institute at Chicago](http://www.ttic.edu/) (TTI, endowed by Toyota and affiliated with the [University of Chicago](http://www.uchicago.edu/)). For many years, Xu has used the Open Science Grid (OSG) to computationally simulate protein structures. Computational predictions can supplement costly and time-consuming experimental methods such as nuclear magnetic resonance spectroscopy. And because predictions can be run simultaneously and independently, the OSG is an ideal computational environment.

Inside the cell, most proteins fold into a compact three-dimensional structure. Failure to fold into the proper structure can produce inactive proteins. Misfolded proteins can be toxic and result in neurodegenerative diseases like Parkinson’s and Alzheimer’s. Sometimes even allergies can be caused by incorrect protein folding.

*Photo Courtesy of Jinbo Xu*

“Studying how protein sequences fold requires a lot of computational power,” said Xu. “Proteins consist of a few hundred amino acids, which fold into their three-dimensional shape. We want to figure out how a protein sequence will fold into its three-dimensional space.”

Xu says it’s better to know the three-dimensional structure. “Proteins fold naturally,” Xu noted. “Once we know the sequence, in principle we should be able to fold it with computer modeling, but we still don’t have computer algorithms to know for sure. That’s my research. It’s very expensive and time consuming and may take months or even years to figure out the structure using experimental techniques.”

<figure>
<img style="max-width:100%" src="https://raw.githubusercontent.com/CHTC/Articles/main/images/osg-osg-may.png" alt="Picture of protein folding "/>
<figcaption>Illustration of protein folding.  Image Credit: Wikimedia Commons, in the public domain.</figcaption>
</figure>

Xu makes use of information in the [Protein Data Bank](http://www.rcsb.org/pdb/home/home.do) (PDB) for insights into protein sequences. “For a protein sequence, there may be many possible conformations to search,” said Xu. “We rely on two major methods when we search through the conformation space. For a protein without a known structure, we may find a similar match in the PDB. Our challenge is how to determine if two proteins are homologous—having a similar structure—or not. The computational challenge is searching through the whole PDB. The other technique is to predict a structure for a protein that doesn’t have a structure in the PDB. In this case, we have to search all possible conformations. It is very time consuming and needs a lot of computational power because we are creating our predictions from scratch.”

Structure-based drug design has become essential in drug discovery, so another key tool in Xu’s arsenal is molecular modeling software he and colleagues developed called RAPTOR (short for Rapid Protein Threading Predictor). Its successor, [RaptorX](http://raptorx.uchicago.edu/), predicts three-dimensional structures for protein sequences that do not have close matches in the PDB. Xu and co-author Jian Peng explain more about RaptorX’s results [in a previously published paper](http://onlinelibrary.wiley.com/doi/10.1002/prot.23175/abstract).

“The OSG will be critical for us when we scale up our computation again,” said Xu. “For example, we have used the OSG for [protein conformation sampling](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC2881378/) and the evaluation of our energy functions. It shortens our simulation times enormously.” In past years, Xu has run thousands of small protein (under 100 amino acids) simulations on the OSG.
