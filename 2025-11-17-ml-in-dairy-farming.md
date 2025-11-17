---
title: "One Researcher’s Leap into Throughput Computing: Bringing Machine Learning to Dairy Farm Management"

author: Sophie Dorros

publish_on:
  - htcondor
  - path
  - chtc
  - pelican
  - osg

canonical_url: https://chtc.cs.wisc.edu/ml-in-dairy-farming.html

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/ml-in-dairy-farming.jpg"
  alt: "Collage of photos from HTCondor Week"

    
description: Ariana Negreiro, Ph.D, in the UW-Madison Digital Livestock Lab, discusses her work using images of cows to develop a machine learning application to monitor their health.
excerpt: Ariana Negreiro, Ph.D, in the UW-Madison Digital Livestock Lab, discusses her work using images of cows to develop a machine learning application to monitor their health.

card_src: "https://raw.githubusercontent.com/CHTC/Articles/main/images/ml-in-dairy-farming-card.jpg"
card_alt: "Ariana Negreiro stands with a cow."

type: user

---

**Ariana Negreiro, Ph.D, in the [UW-Madison Digital Livestock Lab](https://dorealab.cals.wisc.edu), discusses her work using images of cows to develop a machine learning application to monitor their health.**

<figure style="float: left; margin: 0 1rem 1rem 0;">
    <img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/ml-in-dairy-farming.jpg' height="420" width="300" class="figure-img img-fluid rounded" alt="Pictured: Ariana Negreiro credits: Ariana Negreiro">
    <figcaption class="figure-caption">Pictured: Ariana Negreiro credits: Ariana Negreiro</figcaption>
</figure>

The goals for Ariana Negreiro’s work were clear: healthier dairy cows with an improved quality of life. Working under the direction of her lab director [Dr. Joao Dorea](https://andysci.wisc.edu/directory/joao-ricardo-reboucas-dorea/), Negreiro’s research utilizes machine learning and deep learning models to develop tools for dairy cattle management. She used an on-site processing system to produce top down, infrared and depth images of the cows, which are then processed and used to monitor the heifers’ health and milk production potential. One strong advantage of the computer vision approach is that it eliminates the need to manually weigh and monitor cattle, which is stressful for the cows and time consuming for the farmers.

Negreiro, however, faced obstacles on several fronts: limited coding experience when she began her Ph.D, huge amounts of data, and complex workflows. Undeterred and with support from her Lab, the [UW–Madison Digital Livestock Lab](https://dorealab.cals.wisc.edu/), and the [UW-Madison Center for High Throughput Computing (CHTC)](https://chtc.cs.wisc.edu/), Negreiro persevered, and succeeded.

The sheer magnitude of her dataset posed one roadblock. She studied 200 cows from the UW herd, and by the end of the imaging process, there were over 15 million images of the cattle and more than 200 TB of data. Negreiro stated, “We really quickly realized that we were in over our heads; there’s no way we had the infrastructure to process this data.” Her lab was somewhat new on campus, and had nowhere near the capacity needed to process this amount of raw data. The Digital Livestock Lab had used CHTC resources in the past, and at the suggestion of her principal investigator Dr. Dorea, Negreiro turned to the CHTC for help.

Adding to the hurdles, before beginning her Ph.D, Negreiro had limited experience with coding and high throughput computing (HTC). Negreiro’s background is in animal science, and she describes her experience with computer science and code languages as “Zero. Basically nothing.” Negreiro began taking intro to Python and machine learning courses at UW-Madison alongside her research, and quickly learned how much she enjoyed Python.

Negreiro developed skills while working in tandem with CHTC staff supporting her in the development of her code. “They taught me about options I didn’t know were available… there's so much information on the CHTC website and I didn’t know what would help me and my specific situation.” Through [office hours](https://chtc.cs.wisc.edu/uw-research-computing/get-help.html) and personalized support, CHTC staff helped supplement her “learn on the fly” coding experience with expert advice, allowing her to perform large scale research without a computer science background.

Another challenge was identifying each cow; individually identifying each cow through the millions of top down images was not feasible. So, Negreiro created a high throughput computing workflow to organize and identify each cow, and worked with CHTC staff to create this custom process: “I was like a crazy person. I had all these diagrams and lines…And they helped me figure it out; let’s make this pipeline.” This workflow uses the [DAGMan](https://chtc.cs.wisc.edu/uw-research-computing/htc/dagman-workflows) utility of [HTCondor](https://htcondor.org/) to run her calculations in the order she wanted without constantly monitoring and managing her job submissions.

Negreiro also had to figure out how to make the 200 TB of data accessible to the computing capacity. CHTC staff helped her with connecting her data storage with CHTC's computing systems. Still, to fully leverage the high throughput computing system, Negreiro needed a way to transfer only parts of the data to the machines doing the calculations. CHTC staff made the data accessible via [Pelican Platform](https://pelicanplatform.org/) software, which has built-in integration with HTCondor. This enabled Negreiro to easily declare the data she needed for each job in the high throughput computing workflow, with HTCondor automatically handling the necessary file transfers.

The numbers show part of Negreiro’s success. Over the past two years using high throughput computing on CHTC resources, she ran 92,941 jobs, using 24,983 GPU hours, 43,105 CPU hours and 1.2 PBs of file transfer!

Negreiro’s research provides tools to eliminate the need to manually weigh and measure cows, which can be labor-intensive for farmers and stressful for the cattle. Her machine learning models can improve the animals’ quality of life while also reducing inefficient costs for farmers. Sharing her work, Ariana Negreiro presented at High Throughput Computing Week 2025, talking about the utilization of [HTCondor](https://htcondor.org/), [Pelican](https://pelicanplatform.org/), and DAGman workflows for high-throughput phenotyping in dairy cattle. Her slides and presentation can be found on the [PATh presentation page](https://path-cc.io/presentations/2025/06/05/utilizing-htcondor-pelican-and/).

Moving forward, the Digital Livestock Lab will continue to use HTC and CHTC resources. Dr. Dorea notes that “CHTC was always open to help the lab, without this I couldn't analyze the data we collected because we don't have the infrastructure to analyze the large datasets available in agriculture.” Negreiro has also already directed her labmates towards CHTC resources: “I’ve introduced other people in my lab to CHTC…helping them with subfiles and setting up jobs. It’s something our lab will keep on using.” Negreiro is excited to continue looking at heifer growth patterns, noting that although heifer growth has been studied before, automatically collecting regular growth data on many animals makes it much easier to understand growth patterns and improve their future success in dairy herds.
