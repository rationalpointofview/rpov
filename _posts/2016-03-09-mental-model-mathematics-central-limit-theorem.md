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

**Related Lattice**
Law of large numbers
Invert

#Introductions


The central limit theorom tells you that, if you draw a fix number of samples n ( assume n big enough, we will talk about whats big enough later ) random samples from pool with known standard deviation & mean, but **regardless the distribution shape**, then the sum of these sample values will form a bell curve, which mean of the sum will be true mean x n, and standard deviation of these sum will be pool standard deviation * n^1/2.

Couple of things to notice:

* The base pool distribution can be anything, step/normal, you name it, and it doesn't matter

* How big of n is big enough ? 30 is a good number, while 15 is kind of minimum

This is a simulation of dice roll of 300 times using google spreadsheet, as you can see, the chance of landing of each side ( 1- 6) is equal to 1/6, and roll the dice 300 times, the chance of getting 1 - 6 is even, which is a straight line.

[![300 Dice Roll Results](https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/519d73uu.png)](https://docs.google.com/spreadsheets/d/10LqWsKJhCBxm_281Vt0d2yH8-WYg39OLwXkWY4eLTIg/edit#gid=0)

But if we roll 10 dice together, and record the sum, it look like this, better, but not perfect

[![Sum of 10 Dice Roll, 300 times](http://www.rationalpov.com/wp-content/uploads/2016/03/image-1.png)](https://docs.google.com/spreadsheets/d/10LqWsKJhCBxm_281Vt0d2yH8-WYg39OLwXkWY4eLTIg/edit#gid=626723546)

If we roll 15 dice together, and record the sum, it looks like a normal distribution now.

[![Sum of 15 Dice Roll, 300 times](http://www.rationalpov.com/wp-content/uploads/2016/03/image-2.png)](https://docs.google.com/spreadsheets/d/10LqWsKJhCBxm_281Vt0d2yH8-WYg39OLwXkWY4eLTIg/edit#gid=626723546)

**Why this is important?**

Have you wonder why normal distribution( The bell shape curve) is so widely seen and important ? You see it every where, human hight, student exam scores ..

![Bean Machine Normal Distribution](http://www.rationalpov.com/wp-content/uploads/2016/03/Planche_de_Galton.jpg)

Thats because a lot of things can be think of a black box which has many internal parts, and the output of the system could think of like of a sum of all the internal valuable effects, these values usually has range, so the output the system is a bell curve,

most natural things or complex could be simulated by this.
you can use it to find out the probability of certain event.


For example, Human height is influenced by genes, enviromental effects, nutritions etc.

You can think of the human height as sumation of all the influencing factors of a complex system. so by the prediction of central limit theory, it is a bell curve .


**Bonus: How to Read the Normal Distribution Diagram**

I think I know Normal Distribution Digram, but until I use excel to plot one, I found out actually I don't really understand normal distribtuion digram ! So here is the findings of rediscovering normal distribution diagram.

![Normal Distribution Diagram](http://www.rationalpov.com/wp-content/uploads/2016/03/Empirical_Rule.png)

what is the x-axis ?

the x-axis is the standard deviation from the mean, ( translate , the actual values of the sample)

what is the y-axis ?

y-axis the the probability of geting this value

![Normal Distribution Diagram Explained](http://www.rationalpov.com/wp-content/uploads/2016/03/ji8_ij43.png)


**How to use this mental Model**:

when you know the true mean and standard deviation of a group , and you pull a set of samples from the pool, then you can predict:



**Conditions:**

Three conditions:
- the outcome of this event is finite ( dice, gamble, digital event), but more than 1 possibilities ( 2 is okay ) think throw a dice
- the outcome of sample event is mutually exclusive
- the outcome of sample event is independent
- sample size of sample group >30
- the result is the **sum** of all samples ( could be spatial or temporal ) from that group.


**Predictions:**

* The mean of the samples
* The probability of the mean of the samples higher or lower than a speicified number



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




