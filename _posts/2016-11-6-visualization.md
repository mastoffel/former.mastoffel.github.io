---
title: "publication-ready graphs with ggplot2"
layout: post
description: the scatterplot
---

We recently had a discussion seminar in the departement about visualisation for science and the opinions about ggplot2 were quite diverse. Some love it, some don't. Other programs might produce the required graphs quicker, without coding, even interactive. I think with a little bit of training and keeping up to date
with the new developments in ggplot, it will be the last visualization software you have to learn. Moreover,
it will give you freedom of the mind by making it possible to create whatever graphs you want and even get inspired by the newest developments in visualising data. 

Here, I'd like to give a quick overview and an idea about how to produce a publication ready graph.

We are using the iris dataset which contains measurements for three different plant species.


```r
library(ggplot2)
data(iris)
```

Before we start plotting, we load some package which I find make life quite easy to start with
in ggplot. Most people have a hard time customizing the `theme` of a ggplot. The `theme` essentially configures the layout, i.e. things like axes and labels. An excellent package to make this easy and
to have a common theme across all your plot is `ggthemr`. Check out the [ggthemr](https://github.com/cttobin/ggthemr) GitHub repo for a detailed manual.


```r
library(ggthemr)
```

Now we are setting all our layouts once! 

```r
ggthemr(palette = "fresh", layout = "scientific", 
    line_weight = 0.7, text_size = 18, type = "outer")
```

So how does ggplot work? Well, it is not entirely straightforward, which is why some people are not yet using it I guess. We first produce the basis of the plot, i.e. we define the `data.frame` where all the data is stored, and we define the so-called aesthetics (`aes()`). This defines which variables will be plotted. Here we want to have the Sepal.Length on the x-axis and the Petal.Length on the y axis. Let's do it.


```r
p1 <- ggplot(data = iris, aes(x = Sepal.Length, y = Petal.Length)) 
p1
```

<img src="/figure/source/2016-11-6-visualization/unnamed-chunk-4-1.png" title="plot of chunk unnamed-chunk-4" alt="plot of chunk unnamed-chunk-4" style="display: block; margin: auto;" />

No data was plotted! Why is this? It's because we didn't define yet which how the data should be represented. This is the whole point about the layered grammar of graphics! So do we want points, bars, boxplots or what? We have two continous variables, so let's try it with a scatterplot.


```r
p1 +
```

```
## Error: <text>:2:0: unexpected end of input
## 1: p1 +
##    ^
```
