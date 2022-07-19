# CommentFinder-Replication-Package

This replication package is created for the paper titled "CommentFinder: A Simpler, Faster, More Accurate Code Review
Comments Recommendation"


## Abstract
Code review is an effective quality assurance practice, but can be labor-intensive since developers have to manually review the code and provide written feedback. Recently, a deep learning approach was introduced to automatically recommend code review comments based on changed methods. While the approach showed promising results, it requires expensive computational resource and time which limits its use in practice. To address this limitation, we propose CommentFinder -- a simpler and faster retrieval-based approach to recommend code review comments. Through a empirical evaluation of 151,019 changed methods, we evaluate the effectiveness and efficiency of CommentFinder against prior work. We find that when recommending a Top-1 review comment candidate, our CommentFinder is 32\% better than prior work in recommending the correct code review comment. In addition, CommentFinder is 49 times faster than the prior work. These findings highlight that our CommentFinder could help reviewers to reduce the manual efforts by recommending code review comments, while requiring less computational resources.

## Overview
![A usage scenario of CommentFinder in a code review process](./backGroundFigure.png?style=center)
<p>A code review process consists of five main steps (see Figure).
Broadly speaking, in step 1, a developer will first submit a newly developed code (i.e., new code changes) to the code review tool.
Then, in step 2, to examine the newly developed code, the developer will invite reviewer(s) (i.e., the developers other than the code author) to review the newly developed code.
In step 3, the reviewer(s) will inspect the code.
If the reviewer(s) discover any issues in the submitted code, they will provide feedback (i.e., code review comments) to the specific areas of code.
After that, in step 4, the reviewers will make a decision whether this submitted code can be merged into the code repository.
In step 5, if the reviewers suggest that the submitted code is not ready to be merged and a revision is needed, the developer will revise the code to address the code review comments.
Finally, if the submitted code has sufficient quality, the reviewers will approve the submitted code to be integrated into the code repository.</p>

## Description

The package structure with respect to RQ is as follows:
```
    .
    ├── ...
    ├── dataset                 # Dataset
    ├── RQ1_RQ2                 # Code for RQ1 and RQ2
    ├── RQ3 			        # Code for RQ3 
    └── ...

```  

## Getting Started

### System dependencies
* Ubuntu 20.04.3 LTS

### Package dependencies
|                      | Packages                                                                                                                |
|----------------------|-------------------------------------------------------------------------------------------------------------------------|
| Python               | sklearn, numpy, pandas, scipy, time,  pickle, math, warnings, os, operator, matplotlib, csv, math, strsimpy, nltk, tqdm |



###  Reproduce our work
*Run the jupyter-notebook script from top to bottom.

For RQ1: How effective is the proposed CommentFinder compared to the state-of-the-art? => RQ1_RQ2.ipynb

For RQ2: How efficient is the proposed CommentFinder compared to the state-of-the-art? => RQ1_RQ2.ipynb

For RQ3: What is the impact of similarity techniques on the effectiveness and efficiency of CommentFinder? => RQ3.ipynb
