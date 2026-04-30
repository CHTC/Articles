---
title: How one Researcher Uses CHTC To Fill in the Gaps in AI
author: Sophie Dorros

publish_on:
- htcondor
- path
- osg
- chtc

type: feature

canonical_url: https://chtc.cs.wisc.edu/sonia-cromp-filling-gap-of-ai.html

image:
    path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/sonia/box-card.png"
    alt: Cromp Pictured during her time at NASA working on GeoDES

excerpt: Observing gaps in Large Language Models’ (LLMs’) abilities to process tabular data motivated UW-Madison Computer Sciences PhD candidate Sonia Cromp to develop Tabby, an architecture modification  to LLMs that improves how they handle structured data.
---

Observing gaps in Large Language Models’ (LLMs’) abilities to process tabular data motivated UW-Madison Computer Sciences PhD candidate [Sonia Cromp](https://socromp.github.io/) to develop Tabby, an architecture modification  to LLMs that improves how they handle structured data. Cromp began working on Tabby two and a half years ago, after realizing there were weaknesses in generative modeling, particularly for tabular data, within LLMs. Cromp notes that currently, “capabilities to generate examples of [tabular data] are really lagging behind these other modalities like image and text. And so the goal with Tabby was to take the advancements that we've been able to make with Large Language Models and transfer those into generating tabular data.”


<figure style="float: left; margin: 0 1rem 1rem 0; width: 260px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/sonia/sonia-13x20.jpg' height="400" width="260" class="figure-img img-fluid rounded" alt="Pictured: UW Madison CS PhD candidate Sonia Cromp">
<figcaption>Pictured: UW Madison CS PhD candidate Sonia Cromp</figcaption>
</figure>

Traditional LLMs read data as loose sequences of text, so they don’t uphold the strict column structure that tables require. As a result, they can “blur” which values belong to which columns, leading to errors. If you have ever tried to upload a spreadsheet or JSON file to an LLM like ChatGPT and asked it to continue adding to it, you may have noticed the LLM will reorder or even omit rows or columns, failing to give you a cohesive spreadsheet like you requested. Tabby fixes the blurring issue by assigning each column its own dedicated “Expert” so features stay separated. These experts still interact, letting the model learn relationships between columns without mixing them up.

Needing more GPU capacity than her lab had available, Cromp turned to CHTC. Cromp first used CHTC resources to work on a grad school course project at UW-Madison, and two years later, with a Tabby deadline looming, she rediscovered [CHTC](https://chtc.cs.wisc.edu/) to run her jobs and provide GPU compute power: “I had a deadline coming up and I didn't have enough compute to get all of the experiments ran just in my lab. We have our own GPUs that we own, but it's nothing compared to CHTC. So I was racking my brain, I had one week to get this done. And then I remembered I had a CHTC account and I was able to log in and that was a lifesaver”, remarked Cromp. For Cromp’s experiment, she needed to compare how Tabby performed with different LLMs depending on the number of parameters they had. Parameters within LLMs can range from in the millions all the way to the trillions. Cromp’s CHTC-run experiments looked at the performance of differently sized LLMs to generate tabular data, with or without Tabby. Cromp mainly needed GPU access for Tabby, running a total of 406 GPU hours at CHTC over the course of the project.

<figure style="float: right; margin: 0 1rem 0 1rem; width: 300px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/sonia/box-10x7.png' height="210" width="300" class="figure-img img-fluid rounded" alt="Tabby Logo, credits: Sonia Cromp">
<figcaption>Tabby Logo, credits: Sonia Cromp</figcaption>
</figure>

Working on a tabular data project within a community focused on image and text generation was one of the largest hurdles Cromp had to overcome with this project. She noted that “I had trouble getting it accepted within the ML community. A lot of people are focused on image and text, and when you want to work on things that are outside of that, they ask you why. The thing I want to see different within this field, is I think that there should be more attention being put towards tabular and just not image and text data.” Cromp was ultimately able to publish her work, “[Tabby: A Language Model Architecture for Tabular and Structured Data Synthesis](https://openreview.net/pdf?id=b9FPVnb0Bn)” that appeared in Transactions on Machine Learning Research (TMLR) 2026.

Cromp’s journey with the CHTC continued, and she is currently working on another project as part of her work with NASA called GeoDES (Geospatial Diffusion-based Evolution Synthesis), which is a model that generates examples of extratropical cyclone storms (these storms are similar to hurricanes, but form at more northern latitudes). Synthetic extreme storms help fill data gaps, improving both storm research and forecasting model evaluation. Cromp runs her experiments for GeoDES through the CHTC, running models even larger than the ones she ran for Tabby. So far, GeoDES has submitted 638 job requests and logged 2,790 GPU hours.

<figure style="float: right; margin: 0 1rem 0 1rem; width: 280px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/sonia/nasa-14x16.jpg' height="320" width="280" class="figure-img img-fluid rounded" alt="Cromp Pictured during her time at NASA working on GeoDES">
<figcaption>Cromp Pictured during her time at NASA working on GeoDES</figcaption>
</figure>

Cromp’s work with both Tabby and GeoDES underscores the importance of researching gaps that machine learning models may be failing to fill. Cromp remarked: “These modalities are not getting the attention that they need, and I feel like people already are amazing at processing image data, text data, We're not so good at processing these very huge spreadsheets and atmospheric data that have different levels of the atmosphere with 50 different variables at each level.” As LLMs and generative AI continue to advance in scope and ability, it’s important to note the areas where they still need improvement.

Working with the CHTC allowed Cromp to perform compute-intensive experiments she may not otherwise have been able to run. Speaking on her Tabby experiment run on CHTC, Cromp remarked, “that's a very compute-heavy experiment, but it adds useful information to your paper about how your method performs. So making those sorts of experiments more feasible to be performed for people that are doing research like mine, I think is really useful.” Going forward, Cromp will continue to use CHTC resources to run her GeoDES experiments, and her success with Tabby has also inspired some of her labmates to start using the CHTC to complete their own research work.
