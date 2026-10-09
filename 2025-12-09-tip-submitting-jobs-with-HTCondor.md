---
title: Tip of the Month - New Feature for Submitting Jobs with HTCondor
author: Facilitation Team

publish_on:  
    - htcondor

type: tech-blog

canonical_url: "https://htcondor.org/2025-12-09-tip-submitting-jobs-with-HTCondor.html"

excerpt: There’s a new feature for submitting jobs with HTCondor. Now you can use shell = <your script> instead of using executable and arguments!

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/stock_card.jpeg"
  alt: "Open Science Grid"
---

**There’s a new feature for submitting jobs with HTCondor.** 
Now you can use shell = <your script> instead of using executable and arguments!

Before:

```
executable = hello-world.sh
arguments = $(Process)
```


After: 

```
shell = ./hello-world.sh $(Process)
```


**Notable differences**

1. You will have to add your executable (i.e., hello-world.sh to your list of files in transfer_input_files), since HTCondor can’t automatically detect your executable.

2. Your executable must have executable permissions. You can achieve this by running the `chmod +x` command, i.e., `chmod +x hello-world.sh`. This will prevent a “Permission denied” error.

3. An alternate solution to (2): Use `shell = bash hello-world.sh $(Process)`.


**Read more and try it!**

* Read about the new shell option in our guides: [Practice: Submit HTC Jobs using HTCondor](https://chtc.cs.wisc.edu/uw-research-computing/htcondor-job-submission#use-shell-or-executablearguments-in-your-submit-file)

* Try using shell and let us know how it goes for you! Happy computing!


