---
title: Tip of the Month - Set your jobs' priority
author: Facilitation Team

publish_on:  
    - htcondor

type: tech-blog

canonical_url: "https://htcondor.org/featured-users/2026-11-03-tip-set-your-jobs-priority.html"

excerpt: You can set which of your jobs HTCondor will prioritize. If you want new jobs to run before jobs already in the queue, you can increase their priority!

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/stock_card.jpeg"
  alt: "Stock image with purple fabric of dots on a field of rolling black hills"
---

You can set which of your jobs HTCondor will prioritize. For example, if you want to submit some new jobs that are more important than jobs that are currently in the queue, you can increase their priority. *This does not affect your overall priority relative to other users.*

The default job priority is 0. You can pick any integer — in this example, we use +10/-10.

For jobs you want to prioritize, in the submit file, add:

```
priority = 10
```

For jobs you want to deprioritize, add:

```
priority = -10
```

Also consider using [`condor_prio`](https://htcondor.readthedocs.io/en/latest/man-pages/condor_prio.html) to modify the priorities of jobs currently in the queue!
