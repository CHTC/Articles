---
title: Tip of the Month - New Feature for Submitting Jobs with HTCondor
author: Facilitaiton Team

publish_on:  
    - htcondor
    - path
    - osg

type: tech-blog

canonical_url: https://htcondor.org/2025-12-09-tip-submitting-jobs-with-HTCondor.html

excerpt: There’s a new feature for submitting jobs with HTCondor. Now you can use shell = <your script> instead of using executable and arguments!


---
**Tip of the Month**

There’s a new feature for submitting jobs with HTCondor. 
Now you can use shell = <your script> instead of using executable and arguments!

<span style="background-color:#f0f0f0;">
Before:
executable = hello-world.sh
arguments = $(Process)
</span>

<span style="background-color:#f0f0f0;">
After: 
shell = ./hello-world.sh $(Process)
</span>

**Notable differences**

1. You will have to add your executable (i.e., hello-world.sh to your list of files in transfer_input_files), since HTCondor can’t automatically detect your executable.

2. Your executable must have executable permissions. You can achieve this by running the chmod +x command, i.e., chmod +x hello-world.sh. This will prevent a “Permission denied” error.

3. An alternate solution to (2): Use shell = bash hello-world.sh$(Process).


**Read more and try it!**

* Read about the new shell option in our guides: [Practice: Submit HTC Jobs using HTCondor](https://chtc.cs.wisc.edu/uw-research-computing/htcondor-job-submission#use-shell-or-executablearguments-in-your-submit-file)

* Try using shell and let us know how it goes for you! Happy computing!


