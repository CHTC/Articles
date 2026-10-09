---
title: Tip of the Month - Transfer a list of files that changes with each job
author: Facilitation Team

publish_on:  
    - htcondor

type: tech-blog

canonical_url: "https://htcondor.org/2026-07-28-tip-transfer-a-changing-list-of-files.html"

excerpt: How do you transfer a list of files that changes with each job? Using the queue <variable> from <list> syntax, you can!

image:
  path: "https://raw.githubusercontent.com/CHTC/Articles/main/images/stock_card.jpeg"
  alt: "Open Science Grid"
---

How do you transfer a list of files that changes with each job?

Using the `queue <variable> from <list>` syntax, you can!

For example, create `parameters.txt` with your list of files as the last few parameters:

```
1995, 2000, illinois.data
1995, 2000, illinois.data, nebraska.data
1995, 2000, illinois.data, wisconsin.data
1995, 2000, illinois.data, nebraska.data, wisconsin.data
```

Modify your submit file:

```
transfer_input_files = $(files)

queue start, end, files from parameters.txt
```

Now, `$(files)` will take on the values of the third item to the end of the line, and we use `transfer_input_files` to transfer all the `.data` files to our job.
