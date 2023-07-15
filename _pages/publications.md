---
title: "Publications"
permalink: /publications/
---

I have had the opportunity to work on a number of interesting research projects during my Ph.D. My research work is focused towards data mining, machine learning, mining software repositories, software engineering, deep learning, data analytics. Here is a summary of some of my research efforts.

## Understanding the Time to First Response In GitHub Pull Requests [MSR'23]

### Authors: Kazi Amit Hasan, Marcos Macedo, Yuan Tian, Bram Adams, Steven Ding

<a href = 'https://arxiv.org/abs/2304.08426'> Paper </a>, <a href = '#'> Replication Package </a>, <a href = 'https://github.com/RISElabQueens/PR-Accelerator'> Tool released </a>


The pull-based development paradigm is widely adopted by modern open-source software
(OSS) projects, enabling a pull request (PR) to pass through multiple validation stages, from PR
assignment and continuous integration testing to the actual code review, before eventually being merged
into the project or rejected. Due to the distributed collaboration characteristics of open-source
projects, PRs often get delayed across the PR stages, including for the first response, slowing down
software development. In this paper, we conduct an exploratory study on the time-to-first-response. By analyzing 111,094
closed pull requests from ten popular OSS projects on GitHub, we find that bots are frequently used to
generate the first response in a PR. The timing of those bot-generated first responses is significantly
different from the human one. We further conduct an empirical study to understand the characteristics of
the bot- and human-generated first responses, including their relationship with the lifetime of a PR.
The results of our study indicate that the presence of a bot is an important factor explaining the
time-to-first-response in the pull-based development paradigm and, thus, has to be separately analyzed
from human responses. Moreover, we also find that projects with a low PR success rate, heavy existing
developer team workload, and newly created projects have a higher correlation with a longer waiting time
for the first human response to a pull request. These findings are important for newcomers to understand
the delays they experience for their pull requests.

**Impact:** We have released <a href = 'https://github.com/RISElabQueens/PR-Accelerator'> PR-Accelerator </a> which includes a set of tools that reports analytics and information regarding pull requests (PRs) and points out the delays in first response. This tool was presented in our paper titled [Understanding the Time to First Response In GitHub Pull Requests](https://arxiv.org/abs/2304.08426) published at the [MSR 2023](https://conf.researchr.org/home/msr-2023) conference.
