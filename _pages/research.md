---
title: "Developed Software/Tools for SE Research"
permalink: /research/
---

I have had the opportunity to work on a number of interesting research projects during my Ph.D. My research work is focused towards data mining, machine learning, mining software repositories, software engineering, deep learning, data analytics.

<ul>
  <li>
    <strong>T1. PR-Accelerator</strong> <span style="float:right;">May 2023</span><br>
    <em>Associated with "Understanding the Time to First Response In GitHub Pull Requests" (MSR 2023)</em> — reports analytics and information regarding pull requests (PRs) and points out the delays in first response.
  </li>
  <li>
    <strong>T2. PR-Stats</strong> <span style="float:right;">January 2023</span><br>
    An open-source Python library which brings different stats about pull requests.
  </li>
  <li>
    <strong>T3. Data Inspector</strong> <span style="float:right;">August 2021</span><br>
    A tool which brings a total of 15 essential exploratory data analysis, data cleaning automation to make a dataset understandable.
  </li>
</ul>

<!-- Here is a summary of some of my research efforts.

## Understanding Abandonment and Slowdown Dynamics in the Maven Ecosystem [MSR 2025]
### Kazi Amit Hasan, Jerin Yasmin, Huizi Hao, Yuan Tian, Safwat Hassan, Steven Ding

The sustainability of libraries is critical for modern software development, yet many libraries face abandonment, posing significant risks to dependent projects. This study explores the prevalence and patterns of library abandonment in the Maven ecosystem. We investigate abandonment trends over the past decade, revealing that approximately one in four libraries fail to survive beyond their creation year. We also analyze the release activities of libraries, focusing on their lifespan and release speed, and analyze the evolution of these metrics within the lifespan of libraries. We find that while slow release speed and relatively long periods of inactivity are often precursors to abandonment, some abandoned libraries exhibit bursts of high frequent release activity late in their life cycle. Our findings contribute to a new understanding of library abandonment dynamics and offer insights for practitioners to identify and mitigate risks in software ecosystems.



## A First Look at Self-Admitted Miscommunications in GitHub Issues [HSCE&CS 2024]
### Kazi Amit Hasan, Vu Thanh Loc Mai, Cynthia Wang, Yuan Tian, Steven H. H. Ding 

Effective communication is crucial for the success of open-source software development, particularly within distributed and asynchronous working environments on collaborative coding supporting platforms like GitHub. However, these environments often present significant communication challenges due to various factors, leading to project delays and wasted efforts. Despite prior research on collaboration challenges in software teams, there is a notable gap in understanding what, when, and where miscommunications occur in open-source projects. To address this gap, we mined 6,444 GitHub issues where developers explicitly admitted to miscommunication (using keywords such as ``miscommunication'') and manually analyzed the types, timing, and root causes of these self-admitted instances on a statistically significant sample set (363). Our findings are: (1) we developed a taxonomy of 12 issue types where miscommunications frequently occur, with bug reporting and feature requests being the most common; (2) we identified that most miscommunications occur before issue closure, but post-closure miscommunications, though less frequent, pose significant challenges; and (3) we uncovered five primary root causes of miscommunications, with technical misunderstandings being the most prevalent. This study provides the first comprehensive examination of miscommunication in open-source software development, offering insights and recommendations for researchers and practitioners to improve communication practices in GitHub issue discussions.

## An Empirical Study on Developers' Shared Conversations with ChatGPT in GitHub Pull Requests and Issues [EMSE]
### Huizi Hao, Kazi Amit Hasan, Hong Qin, Marcos Macedo, Yuan Tian, Steven H. H. Ding , Ahmed E. Hassan

ChatGPT has significantly impacted software development practices, providing substantial assistance to developers in a variety of tasks, including coding, testing, and debugging. Despite its widespread adoption, the impact of ChatGPT as an assistant in collaborative coding remains largely unexplored. In this paper, we analyze a dataset of 210 and 370 developers shared conversations with ChatGPT in GitHub pull requests (PRs) and issues. We manually examined the content of the conversations and characterized the dynamics of the sharing behavior, i.e., understanding the rationale behind the sharing, identifying the locations where the conversations were shared, and determining the roles of the developers who shared them. Our main observations are: (1) Developers seek ChatGPT assistance across 16 types of software engineering inquiries. In both conversations shared in PRs and issues, the most frequently encountered inquiry categories include code generation, conceptual questions, how-to guides, issue resolution, and code review. (2) Developers frequently engage with ChatGPT via multi-turn conversations where each prompt can fulfill various roles, such as unveiling initial or new tasks, iterative follow-up, and prompt refinement. Multi-turn conversations account for 33.2% of the conversations shared in PRs and 36.9% in issues. (3) In collaborative coding, developers leverage shared conversations with ChatGPT to facilitate their role-specific contributions, whether as authors of PRs or issues, code reviewers, or collaborators on issues. Our work serves as the first step towards understanding the dynamics between developers and ChatGPT in collaborative software development and opens up new directions for future research on the topic.



## Vulnerability of Open-source Face Recognition Systems to Blackbox Attacks: A Case Study With InsightFace [SSCI'23]
### Authors: Nafiz Sadman, Kazi Amit Hasan, Elyas Rashno, Furkan Alaca, Yuan Tian, and Farhana Zulkernine

This paper presents a comprehensive analysis of the security aspects of the InsightFace project (a popular open-source face recognition system) focusing on its susceptibility to three distinct black box attacks: Face Swap, Morphing, and Presentation. Open-source face recognition models are used in commercial applications, thereby motivating our security analysis. Our investigation entails a meticulous evaluation of the susceptibility of the project to false authentication when subjected to the three attacks. We observed from our experiments that InsightFace was not able to differentiate between legitimate images and manipulated images. The principal aim of this research is to draw attention to the security challenges inherent in open-source face recognition systems, often integrated into various public applications.


**Related resources:** <a href = 'https://ieeexplore.ieee.org/abstract/document/10371801/'> Paper </a>


## Understanding the Time to First Response In GitHub Pull Requests [MSR'23]
### Authors: Kazi Amit Hasan, Marcos Macedo, Yuan Tian, Bram Adams, Steven Ding

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

**Related resources:** <a href = 'https://arxiv.org/abs/2304.08426'> Paper </a>, <a href = '#'> Replication Package </a>, <a href = 'https://github.com/RISElabQueens/PR-Accelerator'> Tool released </a> -->