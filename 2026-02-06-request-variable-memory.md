---
title: Tip of the month - Request variable memory with retry_request_memory
author: Facilitation Team

publish_on:  
    - htcondor

type: tech-blog

canonical_url: "https://htcondor.org/2026-02-06-request-variable-memory.html"

excerpt: Have your jobs ever gone on hold because of spikes in memory usage? You could over-request memory, but this decreases your job throughput and also wastes memory resources that could be used for other jobs.

---

Have your jobs ever gone on hold because of spikes in memory usage? You could over-request memory, but this decreases your job throughput and also wastes memory resources that could be used for other jobs.

Instead of submitting a batch of jobs that over-request memory, use `retry_request_memory`!

For example, if you add this to your submit file:

```
request_memory = 1GB
retry_request_memory = 4GB
Every job will request 1 GB of memory. If the job is evicted because it exceeds 1 GB of memory, the job will be restarted with 4 GB of memory.
```

For more complex options, expressions, and examples, check out the [HTCondor manual](https://htcondor.readthedocs.io/en/main/man-pages/condor_submit.html#retry_request_memory)!
