---
title: New Framework Scales Data-Heavy Tools
author: Sophie Dorros 
publish_on:
  - chtc
  - osg
  - path
type: news
canonical_url: "https://path-cc.io/news/2026-08-04-new-framework-scales-data-heavy-tools/"
excerpt: |
  PATh team members show that AlphaFold3 can run efficiently on distributed
  high-throughput computing infrastructure, opening the door for other
  data-heavy scientific tools.
---

Demonstrating that large scientific software like AlphaFold3 can run efficiently on distributed computing networks, [PATh Project](https://path-cc.io/) team members published the paper “[Running AlphaFold3 on Distributed High-Throughput Computing Infrastructure: Scaling Workloads and Enabling Ultra-Large Predictions](https://dl.acm.org/doi/10.1145/3785462.3815874).” This work, accepted by this year's Practice and Experience in Advanced Research Computing (PEARC) Conference, was authored by PATh team members Research Computing Facilitator Danny Morales, OSG Software Area Coordinator Brian Lin, PATh Project Systems Integrator Mats Rynge, Lead Research Computing Facilitator Christina Koch, FoCaS Co-lead Brian Bockelman, and CHTC Director Miron Livny.

AlphaFold3 is a tool that predicts the 3D shape of proteins and other biomolecules, but it needs about 750 GB of reference data to run, and that data traditionally has to live on the same shared computer system as the actual computing power. High-throughput computing (HTC) systems like the OSPool don't have that kind of shared storage, so AlphaFold3 wasn't a natural fit for this kind of distributed setup. So, the team split the AlphaFold3 process into two stages: a data pipeline and the prediction phase, showing that this framework could be applied to help other data-heavy scientific tools run on similar infrastructure.
