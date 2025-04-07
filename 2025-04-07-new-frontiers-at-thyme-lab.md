---
title: "Unlocking New Frontiers in Drug Discovery: High-Throughput Computing in the Thyme Lab"
author: Kallen Wank
publish_on:
  - osg
  - path
  - chtc
  - htcondor
type: feature
excerpt: "In 2022, the Thyme Lab faced a computing bottleneck at UAB. Ari Ginsparg, a PhD student, turned to the OSG, gaining access to ten times more resources, which significantly advanced their research."
image:
  path: https://raw.githubusercontent.com/CHTC/Articles/main/images/thyme/structures.png
  alt: "Example of a prospective drug (white) identified by Rosetta in the hypocretin receptor binding pocket. Amino acids identified to interact with the drug are highlighted in pink or brown."
canonical_url: https://osg-htc.org/spotlights/oral-roberts-ospool-integration.html

banner_src: https://raw.githubusercontent.com/CHTC/Articles/main/images/thyme/grid.png
banner_alt: "Footage from a zebrafish behavior experiment, showing larvae in a 96-well plate."
---

In 2022, computing challenges arose at the [Thyme Lab](https://www.umassmed.edu/thymelab/) when the supercomputer at the University of Alabama at Birmingham (UAB) couldn’t handle running enough parallel jobs for the Thyme Lab’s large data pipeline. Seeking a solution to this computing bottleneck, [Ari Ginsparg](https://www.umassmed.edu/bmb/culture/monthly-department-features/monthly-department-features-posts/2023/07/thyme-lab/), a PhD student working in the lab noted that “a person on my thesis committee recommended the [OSG](https://osg-htc.org/), so we started exploring it. With the OSG, I was able to access more resources — about ten times more — which made a huge difference.”

<figure style="float: right; margin: 0 1rem 0 1rem; width: 350px;">
 <img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/thyme/fish.png' height="500" width="350" class="figure-img img-fluid rounded" alt="Erik in the wet lab">
 <figcaption>Top-down and side views of aggregated zebrafish brain images from control and experimental fish. Regions highlighted in pink indicate differences in structure between the control and experimental groups.</figcaption>
</figure>

The [Thyme Lab](https://www.umassmed.edu/thymelab/), led by Summer Thyme, PhD, assistant professor of biochemistry & molecular technology, has since moved in 2023 to [UMass Chan Medical School](https://www.umassmed.edu/), where it continues its work to uncover the molecular basis of complex neurodevelopmental diseases and to develop therapies.

Ginsparg has focused his work on computational drug discovery. His research centers on developing treatments for diseases like narcolepsy and insomnia. With a background in bioinformatics and computational chemistry, he combines computational techniques with experimental biology to design more effective drugs and advance drug discovery for neurodevelopmental disorders.Using [Rosetta](https://rosettacommons.org/software/), a protein modeling software, Ginsparg created an algorithm to predict potential drugs targeting hypocretin receptor 2 (HCRTR2)— a key player in insomnia and narcolepsy.

<figure style="float: left; margin: 0 1rem 1rem 0; width: 315px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/thyme/grid.png' height="210" width="315" class="figure-img img-fluid rounded" alt="Footage from a zebrafish behavior experiment, showing larvae in a 96-well plate.">
<figcaption>Footage from a zebrafish behavior experiment, showing larvae in a 96-well plate.</figcaption>
</figure>

The [Thyme Lab](https://www.umassmed.edu/thymelab/) uses zebrafish as an ideal model organism to study a wide range of neurodevelopmental disorders. Zebrafish are a popular animal model in labs because they share roughly 70 percent of their DNA with humans, progress through their life cycle more quickly, and are more cost-effective to maintain in the large numbers required for rigorous biochemical studies.

The zebrafish are analyzed with a variety of techniques to view the responses to certain stimuli. For example, Ginsparg explained that “we have specialized devices where zebrafish are placed in 96-well plates and filmed while swimming around. We can add stimuli like flashing lights or sounds to observe how they react.” They also use programs to quantify the sizes of different brain regions and compare them to wild-type zebrafish to see if there are any changes. The data is all uploaded to applications that analyze the images and output results.

To learn how to use the [OSPool](https://osg-htc.org/services/open_science_pool.html), a source of computing capacity that is accessible to any researcher affiliated with a US academic institution, Ginsparg relied on the OSG Office Hours. These virtual hours*, led by the Research Computing Facilitators (RCFs), provide guidance and support. When transitioning to OSPool, Ginsparg emphasized “that the office hours and resources from OSG were critical to my success. The amount of resources they provide has been essential for progressing with my thesis project.”

<figure style="float: left; margin: 0 1rem 1rem 0; width: 545px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/thyme/structures.png' height="383" width="545" class="figure-img img-fluid rounded" alt="Example of a prospective drug (white) identified by Rosetta in the hypocretin receptor binding pocket. Amino acids identified to interact with the drug are highlighted in pink or brown.">
<figcaption>Example of a prospective drug (white) identified by Rosetta in the hypocretin receptor binding pocket. Amino acids identified to interact with the drug are highlighted in pink or brown.</figcaption>
</figure>

The Thyme lab’s setup to modify their systems to use the OSPool was a gradual process. Ginsparg had already set up a workflow with their local supercomputer, so to adapt the workflow to use the OSPool and its software suite [HTCondor](https://htcondor.org/), he transitioned to a new software better suited for OSPool.

“We also had to connect the workflow using the OSPool to our data storage system at UAB, which was a bit of a learning process. Once everything was connected, I was able to scale up the workflow,” Ginsparg said. In the Thyme lab, he is the only one currently using OSPool, but commented that it makes a huge difference. In just the past year, the Thyme Lab has run over [4.7 million jobs on the OSPool](https://osg-htc.org/projects.html?project=UAB_Thyme).

With the jobs running on the OSPool, Ginsparg commented that they have not faced problems or wait times to run jobs. When faced with barriers, Ginsparg returns to OSG Office Hours to get answers to any sort of questions. “The biggest challenge was learning how HTCondor works, but once I got past that, there haven’t been any major issues. The limitations are pretty minimal, and nothing has stopped progress.”

Utilizing the OSPool, Ginsparg, and the Thyme Lab have made discoveries in their search to find new drugs for diseases.“Recently I developed a method to predict drugs that can target a specific pocket in a protein. That’s exciting because it adds new functionality to the Lab’s Rosetta program. We’re on track to develop drugs that could help treat insomnia.” A future direction of the lab includes increasing their usage of OSPool to expand their drug discovery pipeline to identify drugs for other targets.

*OSPool virtual hours occur weekly. Learn more [here](https://portal.osg-htc.org/documentation/support_and_training/support/getting-help-from-RCFs/).
