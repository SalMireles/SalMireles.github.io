---
layout: posts
title: "Some Useful ML Techniques"
excerpt: "Some techniques to keep in your back pocket"
author: sal
tags: machine learning
mathjax: "true"
---

#### Examples borrowed from "Hands-On Machine Learning with Scikit-Learn & Tensorflow" by Aurelien Geron

# Stratified Sampling

When your dataset isn't considerably larger than the number of attributes you must consider the effect of stratified sampling to
avoid introducing sampling bias from random sampling.

For example, the following diagram illustrates a good stratified sampling approach by analyzing the raw data and extracting a representative amount of strata and including sufficient instances in each. The table highlights the decrease in sampling bias in the test sets generated using a stratified sampling approach. This methods category proportions are almost identical to the actual proportions in the dataset.
![alt]({{ site.url }}{{ site.baseurl }}/images/stratified_sampling.jpg)



# Another technique coming soon
$$z=x+y$$
