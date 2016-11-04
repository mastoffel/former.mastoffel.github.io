---
title: "on the reproducibility of statistical results"
layout: post
date:   2015-10-25 
description: a short intro
---



Now and then one observes waves of indignation about what has been termed the [reproducibility crisis](https://en.wikipedia.org/wiki/Replication_crisis). The causes are many and definitely not limited to the field of [psychology](http://science.sciencemag.org/content/349/6251/aac4716), where a recent large scale
attempt to replicate results revealed the flaws of the modern scientific process. 

What I want to focus on in this post is the replicability of the statistical analysis. These thought's
aren't new, the guys at Johns Hopkins University even made a whole [course](https://www.coursera.org/learn/reproducible-research) on it, however I find that these ideas haven't yet made their way into the scientific collective awareness.

**So when *is* a statistical analysis reproducible?** Well, when someone else gets the raw data and your
code and is able to get to the same results and figures like you. My colleagues and I started 
using [literate statistical programming](https://en.wikipedia.org/wiki/Literate_programming) to publish
our code along with a proper human readable explanation (which are not sourrounded by weird symbols like # or % such
as in traditional ways of publishing code). You can check out how this looks like for [Emily's](https://static-content.springer.com/esm/art%3A10.1186%2Fs13104-016-2209-x/MediaObjects/13104_2016_2209_MOESM1_ESM.html),
[Luke's](https://github.com/leberhartphillips/killdeer_foraging/blob/master/Rcode_Killdeer_foraging.pdf) or
[my](https://github.com/mastoffel/seal_chemical_fingerprints/blob/master/analysis_markdown.pdf)
recent paper's. We are all using the faboulous [RMarkdown](http://rmarkdown.rstudio.com/) for this. 

**Advantages of creating RMarkdown files**
- Most of all: Research integrity. You allow others to excactly see and reproduce what you did,
to comment, critisize and 


