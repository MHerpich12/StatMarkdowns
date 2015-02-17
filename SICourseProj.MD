---
title: "StatisticalInference_CourseProj"
author: "Herpich"
date: "Monday, November 17, 2014"
output: word_document
---

```{r}
plot(cars)
```

The first part of the course project examines an exponential distribution, whose pdf takes the form f(x;lambda) = lambda * e ^ (-lambda * x) for x >= 0.  In this assignment, we assume lambda = 0.2.  We know that for an exponential distribution, the mean and standard deviation both equal 1/lambda.

We first start with running 1,000 randomly generated values to plot a histogram of the basic distribution.


```{r}
var = NULL
for (i in 1:1000) var = c(var,rexp(1,0.2))
plot(var)
```

