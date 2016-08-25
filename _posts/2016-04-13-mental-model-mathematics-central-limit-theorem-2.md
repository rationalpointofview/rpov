---
ID: 59
post_title: >
  Mental Model, Mathematics, Central Limit
  Theorem
author: Rational POV
post_date: 2016-04-13 00:56:17
post_excerpt: ""
layout: post
permalink: >
  http://www.rationalpov.com/mental-model-mathematics-central-limit-theorem-2/
published: true
---
**Mental Model Name:Central Limit Theorem** 
**Discipline:Mathematics** 

**Related Lattice:**

Law of large numbers

# Introductions

The central limit theorom:

__The condition:__

* if you draw a fix number of random samples __many times__ ( assuming this fix number n is big enough, we will talk about whats big enough later ) from a pool of numbers with **known standard deviation & mean**.
 
    - The base pool distribution can be anything, step/normal, you name it, and it doesn't matter

    - How big of n is big enough ? 30 is a good number, while 15 is stretch minimum.
    
__The prediction:__

The sum of these sample values from each draw will form a bell curve


* The mean of the bell curve be µ x n:
* The standard deviation of these sum will be base standard deviation * sqrt(n)

If you want to use the average;

sample group mean average = µ

sample standard deviation = σ/sqrt(n)



**Why this is important?**

CLT is in the heart of modern statistics, and you probably saw it but don't know it is CLT.

One Example will be The Famous Bell Curve;

Have you wonder why normal distribution( The bell shape curve) is so widely seen and important ? 


Thats because a lot of things can be think of a black box, which consist of  many internal parts, and the output of the system could think of a sum of all the internal valuable, these values usually has range, so the output the system is a bell curve,

You see it every where, for example, ![human height](http://i.kinja-img.com/gawker-media/image/upload/s--z9tyvHx3--/c_scale,fl_progressive,q_80,w_800/17iprmfy286axjpg.jpg).


For example, Human height is influenced by genes, enviromental effects, nutritions etc. The final result(Height) can be think of as sumation of all the influencing factors of a complex system. so by the prediction of central limit theory, it is a bell curve .

**Why this is useful?**

Because if you know the shape of the distribution and standard deviation of the distribution, you can compute a lot of things 

Eg. you can reverse look up the probability of a given data point.


**When it does'n apply ?**

One of the drawback of CLT is , it is statistics, and statistics..

> There are three kinds of lies: lies, damned lies, and statistics
>   - Benjamin Disraeli

It is often the lesser reliable ones in science. 

 * The Central Limit Theorem only applies to the estimated means of a population parameter when sampled randomly and independently. 

 Thats why polling results is often seems less reliable than the cited "99%" confidence level. Because human being is subject to social proof and ofen can't think independently.

* The central limit theorem fails when there is an infinite variance

* The internal factor of is of this blackbox not complete independent, and some times has strong correctlation with each other, and there could be possibly has positive/negative feedback into then, which will create extreme outcomes.

An Excellent illustration is explained by [Danielle Fong](http://daniellefong.com/2008/01/28/outliers-why-the-central-limit-theorem-is-typically-off/)

* The Sample group needs to be large enough

General Speaking, 30 is good, and 15 is a stretch minimum.


# How to use this mental Model:

*   Gather following data by statistics,combination/permutations or approximations, or proability theory
    
    *   Gather/compute the true mean µ
    *   Gather/compute Group true standard deviation σ
    *   get the sample size

From the data point above, you can calculate the probability of a given sample data point.

the most difficult part of the process is ususally gathing the base rate true mean and standard deviation. Fortunately, we can quickly get the data point if the problem is yes/no type.

## Central Limit Theorem **Approximation** for Binomial Distribution

In real life, find out the base standard deviation is usually difficult.

Fortunately, if your data is one or zero type ( Thinking Polling Results), it fits the [Bernoulli Distribution](https://en.wikipedia.org/wiki/Bernoulli_distribution) definition, and we can use know the standard deviation easily:

[CLT for binomial distribution](http://ocw.mit.edu/courses/sloan-school-of-management/15-063-communicating-with-data-summer-2003/lecture-notes/lecture10.pdf)

Variance = ![variance](https://wikimedia.org/api/rest_v1/media/math/render/svg/7e589c8d7ab029b2bf46af46c93b2385f4709107)

then we can apply the special case of [applying CLT when the base pool is Binomial distriubtion](https://www.stat.auckland.ac.nz/~wild/ChanceEnc/Ch07.propCLT.pdf), and quickly caculate the standard deviation.

if we assign value of head = 1, and value of tail = 0, and the probability of getting a head is p, then σ(x):

![formular for binomial distribution](https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/jnid2wrn.png)

p is also our group mean:

![CLT of binomial distribution](https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/l5xsvj_7.png)


The rule of thumb is that nn should be large enough for np≥5np≥5 and n(1−p)≥5n(1−p)≥5

* Compute the sample group mean/sum mean and standard deviation from CLT

    * Caution: You can't use one sample group data standard deviation to calculate population standard deviation.
    
    as the CLT only says: sample group average σ' = σ/(n)^0.5

    The σ' standard deviation of sample group average, not the stand deviation within the samples.


* Use Normdist function of google spreadsheet to find out the probability, if needed.

*   Compute the sample group mean/sum mean and standard deviation from CLT

*   Use Normdist function of google spreadsheet to find out the probability, if needed.


**Check the assumptions**


Three conditions: 
    + the outcome of this event is finite ( dice, gamble, digital event), but more than 1 possibilities ( 2 is okay ) think throw a dice - the outcome of sample event is mutually exclusive 
    + the outcome of sample event is independent - sample size of sample group >30 
    + the result is the **sum** of all samples ( could be spatial or temporal ) from that group.

**Predictions:**

*   The mean of the samples
*   The probability of the mean of the samples higher or lower than a speicified number

* * *

[Example: Sampling distribution of serum cholesterol][11]

According the National Center for Health Statistics, the distribution of serum cholesterol levels for 20- to 74-year-old males living in the United States has mean 211 mg/dl, and a standard deviation of 46 mg/dl We are planning to collect a sample of 25 individuals and measure their cholesterol levels What is the probability that our sample average will be above 230?


The group µ is 211mg/dl
The group σ is 46 mg/dl

So by CLT, if we run the 25 sample test many times, the sum of these samples will form a bell curve, with the following characteristic

group sum mean: = 25* 211 = 5275
group sum σ = 46 * 25^1/2 = 46*5 = 230
group average: = 211
group average S = 230/25 = 9.2
The group true mean is 211mg/dl The group SD is 46 mg/dl


![Sample Bell Curve][12]

by using Normdist function in google spreadsheet(=normdist(230,211,9.2,true)), we know the probability of group average below 230 is 0.98

Thus the probability of the sample average be above 230 is 1-0.98 = 2%

___

[Example: Slot Machine][13]

> Suppose that we play a slot machine such you can either double your bet or lose your bet. If there is a 45% chance of winning, what is the probability of the Gambler will not lose by playing 100 times ?

*   The Group mean of expected payout:

= 45% * 1 + 55% * -1 =-0.1

*   The Group standard deviation:

The Group Standard Deviation:

sqr(0.45*(1-(-1))^2+0.55*(-1-(-0.1))^2/100)

= 0.0995

not losing probability=1-normdist(0,-0.1,0.0995,true)= 1-0.84263= 15.7%

We can also use the CLT for binomial distribution:

![CLT of binomial distribution](https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/l5xsvj_7.png)

The win rate p=0.45

p=µ=0.45

and the sample σ Standard Deviation: = sqr((1-0.45)*0.45/100) = 0.0497

n= 100

Now we have all the data we need:

sample mean = 0.45
σ(sample) = sqrt(0.45*(1-0.55)/100)= 0.0497
and the break even mark is 0.5

so the probablity of not losing = 1- normdist(0.5,0.45,0.0497,true) = 1-0.843 =15.7%

***

[Example: SUV Recall][13]

The new Endeavor SUV has been recalled because 5% of the cars experience brake failure. The Tahoe dealership has sold 200 of these cars. What is the probability that fewer than 4% of the cars from Tahoe experience brake failure?

You can think of the problem is a casino game too, break failure is a payout of -1, and withouth break failure is a payout of 1

and probability of break failure = 5%

so the mean is = 0.95*1 + 0.05*(-1)= 0.95-0.05= 0.9

and the standard deviation is:

(0.95*0\.01+0.05*3\.61)^(1/2)= 0.435

the 200 sample group mean = 0.9

and group mean standard deviation = (200)^(1/2)* 0.435/200 = 0.031

now we want to know what is the probability of has fewer than 4% of the break failure.

so the value of 4% breakfailure = 1*0\.96+(-1)*0\.04= 0.92

the value of fewer than 4% break failure =1-normdist(0.92,0.9,0.031,true) = 1-0.74 = 26%

if we use the CLT for binomial distrubtion

we can definte:

break failure = 1 no break failure = 0

chance of getting break faiulre (p) = 0.05

mean = 0.05
 σ = ((1-0.05)0.05)^0.5=0.2179

and group σ of 200 samples = 0.2179/(200^0.5)= 0.01556

and getting 4% failure rate:

=normdist(0.04,0.05,0.01556,true)

= 0.2602, about 26%

___

[Example: Opinion Polls, explained from popularsocialscience.com ][16]

![house of the cards][17]

Let us say that we want to know whether Candidate Obama or Candidate Underwood will win the next presidential election.

Since there is only two possible outcomes, we could applying CLT for Binomial distriubtion.

Say we do the hard leg work , and conduct a survey of 1000 persons and ask if they prefer the candidate Obama or candidate Underwood . Then We find that in this poll, 54 percent of those we ask will vote for Obama.

Is that safe to use these 1000 voters to proxy what all US voter think?

lets assign value of voter vote for Obama = p;

by using CLT for binomail distribution, 

![SD(x)][10]

we can know if we do this polling 1000 times, it will form a bell curve and with the following standard deviation

![standard deviation](https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/l5xsvj_7.png)







! [σ(x)](http://www.rationalpov.com/wp-content/uploads/2016/04/gn6xmnvy.png)
 σ'= 0.4983

from the CLT

the population standard deviation:
 σ = σ'
Then for the whole population:


SD = SD' Then for the whole population:

Let's plug the numbers into binomial CLT

p'=0.54 , ie 54% prefer Obama

Group σ(X)= (0.54*(1-0.54)/1000)^0.5 = 0.0157

p'+ σ = 0.54+2\*0.0157=0.5714
p'- σ = 0.054-2\*0.0157 = 0.5086

p'+2sd = 0.54+2*0\.0157=0.5714 p'-2sd = 0.054-2*0\.0157 = 0.5086

![Polling Diagram][18]

All we care is: What is will the µ value greater than 0.5? ie. will more than 50% of voter will vote for Obama ?

By CLT, we know that when we do the 1000 people poll, the average of the poll results will form a bell curve around the µ p( The bell curve on the left of the diagram) , and with standard deviation of σ.

by inverting the CLT, if we have one 1000 people poll results with known p' and σ'( the bell curve on the right) , we can say that there is 95% chance the µ is within 2 σ' away from our sample mean.

In the worse case scenario( within these 95% chance), the µ is -2 σ' from the sample mean, 

we have the µ = p'- σ = 0.054-2*0.0157 = 0.5086, which is still greater than 0.5 
In the worse case scenario( within these 95% chance), the true mean is -2 SD' from the sample mean,

we have the true mean = p'-2sd = 0.054-2*0.0157 = 0.5086, which is still greater than 0.5

so we can say that the µ lies in region 1 ( The turf where Obama will win is 95% + 2.5% = 97.5%

Couple of things to use this with causion:

* There is a **non-zero** probability of the µ lies in region 2, ( where Obama will lose), and it is not so uncommon as the numbers suggest. 

* In this example, we assume sample σ = Population σ /N^0.5, which is an assumption.
*   There is a **non-zero** probability of the true mean lies in region 2, ( where Obama will lose), and it is not so uncommon as the numbers suggest.

*   In this example, we assume sample SD = Population SD /N^0.5, which is an assumption.

If the µ is say 0.47, the group σ is (0.47*(1-0.47)/1000)^0.5=0.01578, which is reasonability close to our sample group σ.

but if the µ is actually 0.1 or 0.9 the group σ is 0.009, which is very different from our sample group σ .

So this polling technique is largely not reliable is the opinion is hugely one sided.


___

[Example Salary Survey](https://historiesofcatastrophicdreaming.wordpress.com/quantitative-methods/third-and-final-exam-qm/the-central-limit-theorem/practical-applications-of-the-central-limit-theorem/)


>The mean salary of the 9,000 employees at Holley.com is µ = 26,000 with a standard deviation of σ = 2420.  A pollster samples 400 randomly selected employees and finds that the mean salary of the sample is 26 650. Is it likely that the pollster would get these results by chance, or does the discrepancy suggest that the pollster’s results are suspect?

Step of Analysis:

* Gather following data by statistics,combination/permutations or approximations, or proability theory

Group true mean:
µ = 26000

Group standard deviation:
σ = 2420

Compute the sample group mean/sum mean and standard deviation from CLT

the sample group of 400 standard deviation:
σ' = 2420/20 = 121

so the mean salary of the sample is 5σ' away, which is raise a big question mark, so the pollster's result could by a suspect.


___

[Example Hypothesis Testing](http://people.math.gatech.edu/~ecroot/3215/central_limit_apps.pdf)

> Problem. You read in a newspaper that 20% of Georgians smoke, and you
decide to test this hypothesis by doing a poll on 1, 000 randomly selected
Georgians with replacement (if the population you are testing is very large,
then you would not need to test with replacement). Suppose that 205 of
the responses are “smoker”, while 795 are “non-smoker”. Is the claim “20%
of Georgians smoke” unreasonable? (Obviously not, but let’s see what the
math tells us...)

__Step of Analysis:__

* Gather following data by statistics,combination/permutations or approximations, or proability theory

    - Group µ

        By using binomal case of CLT, the p we want to test is:
            p = 0.2 ( 20% of Georgians Smoke)
    - Group standard deviation σ
            σ = (0.2*0.8)^0.5
* Compute the sample group mean/sum mean and standard deviation from CLT

            If the hypothesis is true:

            The group mean = p =0.2
            standard deviation σ'= σ/(1000)^0.5 = 0.0126



* Use Normdist function of google spreadsheet to find out the probability, if needed.

    The polling result is 20.5%, which is wihin p+__σ', we would say it is quite probable.

___
[Example Testing a proportion](http://people.cas.uab.edu/~mpogwizd/ma180-fall-2014/HypothesisTesting.pdf)

> The XSORT method of gender selection is believed to increases the likelihood of birthing a girl.
14 couples used the XSORT method and resulted in the birth of 13 girls and 1 boy. Using a 0.05
significance level, test the claim that the XSORT method increases the birth rate of girls.

Step of analysis:

* Gather following data by statistics,combination/permutations or approximations, or proability theory

    - population µ
        * lets assume the probability of birthing a girl is 0.5
        
    - population standard deviation σ

        * by using binomial CLT, the 
        σ = 0.5
  * Compute the sample group mean/sum mean and standard deviation from CLT

        Sample group σ'= σ/14^0.5 =0.133689

and the sample result mean is 0.9286, which is more than 2σ' away from mean.

so the claim is accepted




* Use Normdist function of google spreadsheet to find out the probability, if needed.

___

[Example AP Scores](http://homepages.math.uic.edu/~bpower6/stat101/Sampling%20Distributions.pdf)

> A Teacher has a class of 68 students taking the AP Physics test. Assuming they are typical of the population, the result of whose scores are given, what is the probability the average score will be at least 3?

score | 1 | 2 | 3 | 4 |5
---|---|---|---|---
Probability|21.5%|18.8%|24.7%|21.7%|13.3%

The Base average value = 2.865
The Base group standard deviation = 1.337
So the Expected sample average standard deviation = 1.337 /(68)^0.5=0.1617

So the probability of the score higher than 3 is 20.2%
  
***

[Example: Is homefield advantage effect true in baseball ?](https://www.lakeheadu.ca/sites/default/files/uploads/77/docs/Anderson_Project.pdf)

>In the 2013 Major League Baseball season, there were 2431 games played, and of those games, 1308 of them were won at home. This indicates that approximately 53.81% of the games played were won at home. 

If there is no homefield advantage, the probability of winning at home will be 50:50, 0.5

We can use the same binomial CLT technique we used in the polling sample

the σ=((1-0.5)(0.5))^0.5 = 0.5

and sample average standard deviation = 0.5/(2431)^0.5=0.5/49.3=0.010141

using 1-normdist(0.5381,0.5,0.01014198,true)= 1-0.9999139= 0.008%

so the probability of hypothesis of homefield advantage not exist is 0.008%

**Bonus: Confidence Interval & CLT:**

Confidence Interval is a range, usualy is Sample Mean +- 1.96 standard deviation (95% Interval)

***


[Example Advertisement Campaign](https://www.youtube.com/watch?v=QRwPMzAL0iA&list=PLAKBwakacHbRRw278HMXpCsOOIIcLYGX5&index=4)

If you run two campagin banners fro 1000 impression, and first banner has a 1% conversion rate, and second banner has a 3% conversion rate, whats the probability of second banner better than the first banner?

Recall, conversion is basically 1 or 0, and we can use CLT for binomial distribution to estimate the standard deviation of two banners.

first banner:

mean= 0.01
standard devivation = sqrt(0.01*0.99/1000)=0.00314

second banner:

mean=0.03
standard deviation = sqrt(0.03*0.97/1000)= 0.00539

use 99% confidence interval

first banner:

1% +- 2.58*0.314%= 0.19% ~ 1.81%

second banner:

3% +- 2.58*0.539% = 3% +- 1.39% = 1.61

so the second banner has a probablilty of over 90% better converting than banner 1

[Example A keyword search program ](http://www.utdallas.edu/~mbaron/3341/Practice6.pdf)

> A keyword search program lists the files that contain a given keyword. If it runs
through 200 files, and each file contains the keyword with probability 0.36, independently of
other files, compute the probability that
(a) more than 70 files
(b) less than 70 files
(c) exactly 70 files will be listed.

p=0.36
sd= sqtr(0.36*0.64/200)
= 0.0339

Normdist(0.35,0.36,0.0339,true)=0.384

(a) 1-0.384 = 61.6%

***

[Example Roulette](https://www2.stat.duke.edu/courses/Spring05/sta101.2/lectures/STA101lecture13.pdf)

> You are playing Red and Black in roulette. (A roulette wheel
has 38 pockets; 18 are red, 18 are black, and 2 are green—the house takes
all the money on green). You pick either red or black; if the ball lands in
the color you pick, you win a dollar. Otherwise you lose a dollar.
Suppose you make 100 plays. What is the chance that you lose $10 or
more?

The win rate p: 18/38 = 47.37%

from Binomial CLT, the true mean = p = 0.4737

the 100 sample sum true mean = 0.4737*100 = 47.37
the 100 sample sum standard deviation = sqrt((1-0.4737)*0.4737*100)=4.99

The triky part is to find the target win rate for betting $100 and lose $10 more:


the win rate p for betting $100 and lose $10 more is:

90/100*0.5=0.45 

average:

betting 50
lost more than 45

so the final formular is:

normdist(45,47.37,4.99,true)= 31.74%

Using classic CLT to verify:

for betting $1

true mean = 2*0.4737 + (0)*(1-0.4737)=0.9474

true standard deviation = sqrt(0.4737*(2-(0.9474))^2+0.5263*(0-(0.9474))^2)=0.99861

for betting $1 100 times

the group mean = 0.9474* 100 = 94.74

the group standard deviation = sqrt(100)*0.99861 = 9.9861

for loss more than $10

=normdist(90,94.74,9.9861,true)=31.75%




***




[Example real life bell shape curve](http://math.stackexchange.com/questions/38825/cool-examples-of-the-central-limit-theorem-in-action)

>  by Matt E
Find an old stone step or lintel in front of a doorway (one that is old enough that it has been worn down by generations of people walking over it). If you look at how it is worn down, the wearing down won't be uniform over the surface of the step: rather, it will be in a bell-curve. (People tend to walk through the middle of the doorway.)

> If the door doesn't open all the way, the bell-curve won't be perfect; there will a bias towards the side away from the hinges.



**Bonus: How to Read the Normal Distribution Diagram**

I think I know Normal Distribution Digram, but until I use excel to plot one, I found out actually I don't really understand normal distribtuion digram ! So here is the findings of rediscovering normal distribution diagram.

![Normal Distribution Diagram][19]

what is the x-axis ?

the x-axis is the standard deviation from the mean, ( the 0 in the normal distribution digarm is equal to the mean of the histogram)

what is the y-axis ?

y-axis the the probability of getting this value, in real life terms, y-axis is the frequency in the histogram, noted the probability of getting mean value( the 0 point in x-axis is not 0.5! but about 0.4)

![Normal Distribution Diagram Explained][20]

* * *


***

Further study 

[z-test,Z-test is any statistical test for which the distribution of the test statistic under the null hypothesis can be approximated by a normal distribution.](https://en.wikipedia.org/wiki/Z-test)

[Beta distrubtion](https://en.wikipedia.org/wiki/Beta_distribution)
[Poisson distribution](https://en.wikipedia.org/wiki/Poisson_distribution)



More resource:

[Central limit Theorem demostration][21]

 [1]: http://www.rationalpov.com/wp-content/uploads/2016/03/E6A2D69A-C356-4900-AABE-46DFEDE096AD.gif
 [2]: https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/519d73uu.png
 [3]: https://docs.google.com/spreadsheets/d/10LqWsKJhCBxm_281Vt0d2yH8-WYg39OLwXkWY4eLTIg/edit#gid=0
 [4]: http://www.rationalpov.com/wp-content/uploads/2016/03/image-1.png
 [5]: https://docs.google.com/spreadsheets/d/10LqWsKJhCBxm_281Vt0d2yH8-WYg39OLwXkWY4eLTIg/edit#gid=626723546
 [6]: http://www.rationalpov.com/wp-content/uploads/2016/03/image-2.png
 [7]: http://www.rationalpov.com/wp-content/uploads/2016/03/Planche_de_Galton.jpg
 [8]: http://blog.vctr.me/posts/central-limit-theorem.html
 [9]: https://www.stat.auckland.ac.nz/~wild/ChanceEnc/Ch07.propCLT.pdf
 [10]: http://www.rationalpov.com/wp-content/uploads/2016/04/gn6xmnvy.png
 [11]: http://web.as.uky.edu/statistics/users/pbreheny/580-f10/notes/9.pdf
 [12]: https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/bryi_5g3.png
 [13]: https://www.ltcconline.net/greenl/courses/201/probdist/clt.htm
 [14]: https://upload.wikimedia.org/math/3/1/8/31830fa1f2f922edf6079209a51f8967.png
 [15]: http://www.rationalpov.com/wp-content/uploads/2016/03/render-2.png
 [16]: http://www.popularsocialscience.com/2013/08/26/can-we-trust-opinion-polls-the-central-limit-theorem-binomial-proportion-confidence-intervals-and-likely-voters/
 [17]: http://www.rationalpov.com/wp-content/uploads/2016/04/house-of-cards-season-4-key-art1.jpg
 [18]: http://www.rationalpov.com/wp-content/uploads/2016/04/rpov-polling-1.png
 [19]: http://www.rationalpov.com/wp-content/uploads/2016/04/Empirical_Rule.png
 [20]: http://www.rationalpov.com/wp-content/uploads/2016/04/ji8_ij43.png
 [21]: http://onlinestatbook.com/2/sampling_distributions/clt_demo.html