---
ID: 132
post_title: >
  Mental Model, Mathematics, Central Limit
  Theorem
author: Rational POV
post_date: 2016-03-09 00:31:12
post_excerpt: ""
layout: post
permalink: >
  http://www.rationalpov.com/blog/mental-model-mathematics-central-limit-theorem/
published: true
---
**Mental Model Name:Central Limit Theorem** 
**Discipline:Mathematics** 
**Lattice Rank :7**

Introductions

****How to use this mental Model****:

The central limit theorom tells you that, if you draw a fix number of samples n ( assump big enough ) random samples from pool with known standard deviation & mean, then the sum of these sample values will form a bell curve, which mean of the sum will be true mean x n, and standard deviation of these sum will be pool standard deviation * n^1/2


**Conditions:**

**Predictions:**

___
 
[Example: Sampling distribution of serum cholesterol](http://web.as.uky.edu/statistics/users/pbreheny/580-f10/notes/9.pdf)

According the National Center for Health Statistics, the distribution of serum cholesterol levels for 20- to 74-year-old males living in the United States has mean 211 mg/dl, and a standard deviation of 46 mg/dl We are planning to collect a sample of 25 individuals and measure their cholesterol levels What is the probability that our sample average will be above 230?

The group true mean is 211mg/dl
The group SD is 46 mg/dl

So by CLT, if we run the 25 sample test many times, the sum of these samples will form a bell curve, with the following characteristic

group sum mean: = 25* 211 = 5275
group sum SD = 46 * 25^1/2 = 46*5 = 230
group average: = 211
group average S = 230/25 = 9.2


{{%[wolframalphawidget id="69d658d0b2859e32cd4dc3b970c8496c" output="iframe"]}}

