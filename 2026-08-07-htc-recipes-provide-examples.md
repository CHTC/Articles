---
title: HTC Recipes Provide Ready-to-Go Examples for Researchers
author: Sophie Dorros
publish_on:
  - chtc
  - osg
  - htcondor 
type: news
canonical_url: "https://chtc.cs.wisc.edu/htc-recipes-provide-ready-to-go-examples-for-researchers.html"
excerpt: |
  CHTC's Facilitation Team offers ready-to-go recipes for running software
  like AlphaFold3 and PyTorch on CHTC and the OSPool, helping researchers
  skip the guesswork of building HTC workflows from scratch.
---

If you have ever wanted to execute research computing and submit jobs on [Center for High Throughput Computing](https://chtc.cs.wisc.edu/) (CHTC) or the [OSPool](https://osg-htc.org/services/ospool/) but don't want to start from scratch or lack experience in using high throughput computing (HTC) tools, CHTC recipes might be for you. Provided by the CHTC [Facilitation Team](https://chtc.cs.wisc.edu/uw-research-computing/facilitation-team), recipes are ready-to-go examples of how to use a software or complete a computational task. CHTC recipes can help you install and run jobs on software like AlphaFold3, Conda, MATLAB, Python, and PyTorch, and submit jobs on CHTC or the OSPool.

As an example, researchers utilizing PyTorch, a popular deep-learning library used as a framework for developing machine learning and AI workflows and software, have access to a [step-by-step recipe and supporting documentation](https://github.com/CHTC/tutorial-pytorch-catdog) so that users who've never run PyTorch on an HTC system could try the example for themselves without needing prior knowledge of how to run a job. More experienced users have the option to use the scripts and submit files as templates for adapting their own PyTorch workflows on an HTC system. "Some researchers have used machine learning models to identify areas of interest in medical images. Another researcher used large-language models (LLMs) to translate and transcribe foreign languages. In the chemical sciences, some are using these tools to develop new parameters for improved molecular and protein simulations," remarked Facilitator Amber Lim.

<figure style="float: left; margin: 0 1rem 1rem 0; width: 300px;">
<img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/alphafold-recipe-example.png' height="420" width="300" class="figure-img img-fluid rounded" alt="AlphaFold Recipe">
<figcaption>Example of an AlphaFold3 Recipe</figcaption>
</figure>

AlphaFold3 workflows, a protein structure prediction tool used by researchers to model proteins, nucleic acids, and other biomolecular complexes, can be difficult to run on shared computing systems because they combine large reference databases, CPU-intensive data preparation, GPU-based inference, and substantial storage requirements. Facilitator Danny Morales developed a [recipe](https://github.com/CHTC/recipes/tree/main/software/AlphaFold) that provides step-by-step documentation, example input files, wrapper scripts, and [HTCondor](https://htcondor.org/) submit files so that researchers can run AlphaFold3 on OSG resources without needing to build the workflow from scratch. The recipe is designed to support both new and experienced HTC users. Researchers who are new to distributed computing can follow the example as a guided starting point for submitting AlphaFold3 jobs, while more advanced users can adapt the scripts and submit files for larger-scale protein structure prediction campaigns. The recipe also demonstrates how large scientific datasets, such as AlphaFold3 reference databases, can be treated as shared infrastructure rather than repeatedly transferred by individual users. By combining pre-staged databases, GPU scheduling, and reusable workflow templates, the AlphaFold3 recipe helps make high-throughput protein structure prediction more accessible to researchers working across biology, chemistry, medicine, and computational science.

In addition to PyTorch and AlphaFold3, researchers have access to a growing number of software-based recipes, including Gurobi, Julia, SLEAP, R, and MATLAB. "We're seeing more and more researchers considering how they can apply machine learning tools to their field, so it's important for us at CHTC to support the researchers who can use these tools to help further their discoveries and work," noted Lim.

A full overview of all CHTC recipes and supporting documentation can be found [here](https://github.com/CHTC/recipes/tree/main). Users interested in contributing their own recipes, or who believe a specific recipe could help their research community, can reach out to the Facilitation Team at [chtc@cs.wisc.edu](mailto:chtc@cs.wisc.edu).
