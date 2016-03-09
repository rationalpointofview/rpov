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

#Introductions


The central limit theorom tells you that, if you draw a fix number of samples n ( assume n big enough, we will talk about whats big enough later ) random samples from pool with known standard deviation & mean, then the sum of these sample values will form a bell curve, which mean of the sum will be true mean x n, and standard deviation of these sum will be pool standard deviation * n^1/2.

Couple of things to notice:

* The base pool distribution can be anything, step/normal, you name it, and it doesn't matter

* How big of n is big enough ? 30 is a good number


<iframe width="600" height="371" seamless frameborder="0" scrolling="no" src="https://docs.google.com/spreadsheets/d/10LqWsKJhCBxm_281Vt0d2yH8-WYg39OLwXkWY4eLTIg/pubchart?oid=593388338&amp;format=interactive"></iframe>


**How to use this mental Model**:

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

![Sample Bell Curve](https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/bryi_5g3.png)

by using Normdist function in google spreadsheet(=normdist(230,211,9.2,true)), we know the probability of group average below 230 is 0.98

Thus the probability of the sample average be above 230 is 1-0.98 = 2%




