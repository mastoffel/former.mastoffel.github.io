---
title: "Using RMarkdown for reproducible research"
layout: post
date:   2015-10-25 
description: some thoughts and how to start
---



Now and then one observes waves of indignation about what has been termed the [reproducibility crisis](https://en.wikipedia.org/wiki/Replication_crisis). The causes are many and definitely not limited to the field of [psychology](http://science.sciencemag.org/content/349/6251/aac4716), where a recent large scale
attempt to replicate results revealed the flaws of the modern scientific process. 

What I want to focus on in this post is the replicability of the statistical analysis. These thoughts
aren't new, the guys at Johns Hopkins University even made a whole [course](https://www.coursera.org/learn/reproducible-research) on it, however I find that these ideas haven't yet made their way into the scientific collective awareness.

**So when *is* a statistical analysis reproducible?** Well, when someone else gets the raw data and your
code and is able to get to the same results and figures like you. My colleagues and I started 
using [literate statistical programming](https://en.wikipedia.org/wiki/Literate_programming) to publish
our code along with a proper human readable explanation (which are not sourrounded by weird symbols like # or % such
as in traditional ways of publishing code). You can check out how this looks like for [Emily's](https://static-content.springer.com/esm/art%3A10.1186%2Fs13104-016-2209-x/MediaObjects/13104_2016_2209_MOESM1_ESM.html),
[Luke's](https://github.com/leberhartphillips/killdeer_foraging/blob/master/Rcode_Killdeer_foraging.pdf) or
[my](https://github.com/mastoffel/seal_chemical_fingerprints/blob/master/analysis_markdown.pdf)
recent paper's. We are all using the faboulous [RMarkdown](http://rmarkdown.rstudio.com/) for this. One of the essences of RMarkdown is that the complete code has to work for the document to be compiled, which ensures that you are always sure to publish the correct analysis.

**Advantages of creating RMarkdown files**

*  *Research integrity* -- You allow others to excactly see and reproduce what you did,
to comment and to critisize. Much more so then just writing a paragraph in the Methods section of a paper.
* *Code usability* -- Clean, commented code allows to build on it. When you come back to your project years later, 
you will still understand what excactly you did. And not just you, everyone can build on your 
work and use your code. I´m sure this will facilitate collaborations, citations and standardization
across research projects.
* *Code clarity* -- When writing a Rmarkdown file you want your code to look good. This is why you have to force yourself to avoid duplication and write the code as clear as possible. This conscious post-processing
will help finding bugs and reinforce the trust in what you did.

**How to start**

1. Don't use Point&Click programs, but code in R or any other language. This is probably the hardest part. All steps of the analysis have to be written as code to be properly included in the RMarkdown file. As R is developing rapidly, there will be a package for everything you want to do, especially if it's some kind of established analysis. However, having some parts of the analysis in the RMarkdown file is much better then not showing any code. 
2. Download the newest version of [RStudio](https://www.rstudio.com/)  
3. Open RStudio and click on the little symbol in the left upper corner and open up a new RMarkdown file, or even cooler the new RNotebook (Which is essentially an RMarkdown file with some more interactivity)
4. Look up how to write in [RMarkdown](http://rmarkdown.rstudio.com/lesson-1.html), it is really easy. Use ctrl+alt+i to open up a new code chunk and place your code in there. Click on the little `Knit` button at the top to compile your document as html, pdf or word document. 
5. Once you have an idea and some confidence in RMarkdown, you can not just produce reproducible, code heavy documents to accompany papers, but you can create presentations, interactive documents, websites and much more. Have a look at the RMarkdown [gallery](http://rmarkdown.rstudio.com/gallery.html) to see what's possible.


    
**A last thought about the impact of literate statistical programming on science**

Science gets more data intense and statistical analyses get more complicated. New methods and ideas are developed all the time, and just reading about them in a methods section makes them unusable. In addition, many Methods sections in papers allow for just a few paragraphs and outsourcing them to the supplementary material makes them even less accesible, controlled, and read. I think RMarkdown is a great tool to not just reinforce integrity, but to actually replace the traditional statistical methods section.



