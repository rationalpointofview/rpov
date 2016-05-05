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
**Lattice Rank :8**

**Related Lattice** Law of large numbers

# Introductions

The central limit theorom:

__The condition:__

* if you draw a fix number of random samples __many times__ ( assuming this fix number n is big enough, we will talk about whats big enough later ) from a pool of numbers with known standard deviation & mean.
 
    - The base pool distribution can be anything, step/normal, you name it, and it doesn't matter

    - How big of n is big enough ? 30 is a good number, while 15 is stretch minimum.
    
__The prediction:__

The sum( or average) of these sample values from each draw will form a bell curve


The mean of the bell curve be µ x n:
The standard deviation of these sum will be pool standard deviation * n^1/2.

If we use the group average instead, divided both average and the sample group standard deviation by n.

sample group mean average = µ

sample group average standard deviation = σ/n^0.5



**Why this is important?**

Have you wonder why normal distribution( The bell shape curve) is so widely seen and important ? 


Thats because a lot of things can be think of a black box, which consist of  many internal parts, and the output of the system could think of a sum of all the internal valuable, these values usually has range, so the output the system is a bell curve,

You see it every where, for example, ![human height](http://i.kinja-img.com/gawker-media/image/upload/s--z9tyvHx3--/c_scale,fl_progressive,q_80,w_800/17iprmfy286axjpg.jpg).


For example, Human height is influenced by genes, enviromental effects, nutritions etc. The final result(Height) can be think of as sumation of all the influencing factors of a complex system. so by the prediction of central limit theory, it is a bell curve .

**Why this is useful?**

Because if the shape of the distribution is known, we can reverse look up the probability of the data set

most natural things or complex could be simulated by this. you can use it to find out the probability of certain event.


**When it does'n apply ?**

One of the drawback of CLIT is , it is statistics, and statistics..

> There are three kinds of lies: lies, damned lies, and statistics
>   - Benjamin Disraeli

It is often the lesser reliable ones in science. 

 * The Central Limit Theorem only applies to the estimated means of a population parameter when sampled randomly and independently. 

 * The central limit theorem fails when there is an infinite variance

 * The internal factor of is of this blackbox not complete independent, and some times has strong correctlation with each other, and there could be possibly has positive/negative feedback into then, which will create extreme outcomes.

An Excellent illustration is explained by [Danielle Fong](http://daniellefong.com/2008/01/28/outliers-why-the-central-limit-theorem-is-typically-off/)


**How to use this mental Model**:

*   Gather following data by statistics,combination/permutations or approximations, or proability theory
    
    *   Group true mean
    *   Group standard deviation

    - Group µ
    - Group standard deviation σ

    There is a special case of [applying CLT when the base pool is Binomial distriubtion](https://www.stat.auckland.ac.nz/~wild/ChanceEnc/Ch07.propCLT.pdf).

    What is a Binomial Distribtuion ? If there is only two possible outcome, win or loss, head or tail, get elected or not, you got the idea, and the outcome of one trial will not affect the other

    ![formular for binomial distribution](https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/jnid2wrn.png)

    >The Binomial(n, p) distribution is the distribution of Y , the number of
    heads in n tosses of a biased coin, when the probability of getting a head on
    a single toss is p. We begin by setting up a separate random variable for each
    toss.

    if we assign value of head = 1, and value of tail = 0, and the probability of getting a head is p, then σ(x):

    p is also our group mean:

    ![CLT of binomial distribution](https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/l5xsvj_7.png)
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

It is a tricky one:

How can we know the standard deviation ?

There is only two possible outcome, winning $1, which has a probability of 45%, and losing $1, which has a probability of 55%

recall the formular for standard deviation is:

![standard deviation](https://upload.wikimedia.org/math/3/1/8/31830fa1f2f922edf6079209a51f8967.png)

we can compute the group standard deviation as the follows:

![standard deviation](http://www.rationalpov.com/wp-content/uploads/2016/04/render-2.png)

* The σ is a average measurement of each sample depart from mean, as we already know the proability(frequency) of each sample, we just need to mutiple the expected value (1, -1) with it's probability accordingly.
![Standard Deviation][14]


= 0.9947

Let's plug the numbers in to CLT

sample mean = group mean = -0.1

100 sample group standard deviation mean = 0.9947*10/100 = 0.09947

and the break even mark is 0.

not losing probability=1-normdist(0,-0.1,0.09947,true)= 1-0.84263= 15.7%

We can also try to use the CLT for binomial distrubtion to solve this:

P = 0.45
and mean = 0.45 σ= ((1-0.45)*0.45)^0.5=0.497

so the 100 sample group σ 
P = 0.45 and mean = 0.45 SD= ((1-0.45)*0.45)^0.5=0.497

and as we definite the losing payout is 0, winning payout is 1, the point of not losing should be 0.5

so the probablity of not losing = 1- normdist(0.5,0.45,0.0497,true) = 1-0.843 =15.7%

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

Can we deduct anything from this merely 1000 people poll data ? we are really interested in knowing what all US voter think.

lets assign value of voter vote for Obama = 1, and value of voter vote for Underwood = 0, and the probability of voter vote for Obama is p, recall:


while we dont know the value of µ, p, let's imaging that we conducted a lot of  opinion polls (say one million polls) and asking 1000 persons each time whether or not they would vote for Obama. 

By CLT, we know that the distrubtion of these average of 1000 persons polls will form a bell curve, around the µ, p.

But obviously, we don't have the luxury of doing 1 million 1000 people polls. We can just do one. And from the one data point, we got the sapme mean.

But we can use CLT to approximately guesstimate hwo these 1 million 1000 people polls will look like.


The σ'( The 1000 poll group average standard deviation)

We can make two assumptions:
while we dont know the value of true mean, p, let's imaging that we conducted a lot of opinion polls (say one million polls) and asking 1000 persons each time whether or not they would vote for Obama.

The σx = σ/N^0.5 = (p*(1-p)/n)^0.5

but the problem is , we dont know the µ P, how can we solve that?

__We can use the sample p' value as our approximation to µ P.__ 

__Heck. We could actually use the abitary number of 0.5 ( assume the chance is even, and hence the maximum σ)__
![SD(x)][10]

It is a relative Safe assumption, as long as the µ P is within 0.3 to 0.7 

Why ?

Using the same 1000 people Poll assumption:

Case: µ = 0.7 
 σ= 0.0145

Case: µ = 0.5
 σ = 0.0158

Case: µ = 0.3
 σ= 0.0145

If the µ is within range of 0.3-0.7, the maximum difference is only

0.0158-0.0145= 0.13 Percentage point standard deviation.





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

p'+ σ = 0.54+2*0.0157=0.5714
p'- σ = 0.054-2*0.0157 = 0.5086

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

[Example Noise Cancellation](http://people.math.gatech.edu/~ecroot/3215/central_limit_apps.pdf)

> Suppose that a man is driving through the desert, and runs out of gas. He
grabs his cellphone to make a call for help, dialing 911, but he is just at
the edge of the broadcast range for his cellphone, and so his call to the 911
dispatcher is somewhat noisy and garbled. Suppose that the 911 dispatcher
has the ability to use several cellphone towers to clean up the signal. Suppose
that there are about 100 towers near to the stranded driver, and suppose that
the signals they each receive at a particular instant in time is given by:

![example formular](https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/f3cjc3ug.png)

S is the true signal and Yi is the noise.

From basic signal & information theory, we can assume the Yi noise is independaent and normally distributed, and has a mean 0 and standard deviation of σ.

So the 911 dispatcher can do the noise cancellation by computing the average.  

![average](https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/x51fqq9-.png)

At any rate, if we assume that the Yi are all independent normal random variables, then we don’t even need the central limit theorem, because in that case we have that X − S is exactly N(0, σ2/100).

By just summing the signal average from 100 towers, we can perform a noisse cancellation and increate the Signal to noise ration by 100 fold !

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
  

* [Example: Is homefield advantage effect true in baseball ?](https://www.lakeheadu.ca/sites/default/files/uploads/77/docs/Anderson_Project.pdf)

>In the 2013 Major League Baseball season, there were 2431 games played, and of those games, 1308 of them were won at home. This indicates that approximately 53.81% of the games played were won at home. 

If there is no homefield advantage, the probability of winning at home will be 50:50, 0.5

We can use the same binomial CLT technique we used in the polling sample

the σ=((1-0.5)(0.5))^0.5 = 0.5

and sample average standard deviation = 0.5/(2431)^0.5=0.5/49.3=0.010141

using 1-normdist(0.5381,0.5,0.01014198,true)= 1-0.9999139= 0.008%

so the probability of hypothesis of homefield advantage not exist is 0.008%

**Bonus: Confidence Interval & CLT:

Confidence Interval is a range, usualy is Sample Mean +- 1.96 standard deviation (95% Interval)

> [Problem 1](http://stattrek.com/estimation/confidence-interval.aspx)

Suppose we want to estimate the average weight of an adult male in Dekalb County, Georgia. We draw a random sample of 1,000 men from a population of 1,000,000 men and weigh them. We find that the average man in our sample weighs 180 pounds, and the standard deviation of the sample is 30 pounds. What is the 95% confidence interval.

(A) 180 + 1.86 
(B) 180 + 3.0 
(C) 180 + 5.88 
(D) 180 + 30 
(E) None of the above

The correct answer ?

First we need to compute standard deviation of the sample.

Given the population SE= 30

by CLT, the Sample SE average = 30/sqrt(1000)= 0.95

so the confidence interval is:

1.96*0.95= 1.862

So A is the correct answer

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




**Bonus: How to Read the Normal Distribution Diagram**

I think I know Normal Distribution Digram, but until I use excel to plot one, I found out actually I don't really understand normal distribtuion digram ! So here is the findings of rediscovering normal distribution diagram.

![Normal Distribution Diagram][19]

what is the x-axis ?

the x-axis is the standard deviation from the mean, ( the 0 in the normal distribution digarm is equal to the mean of the histogram)

what is the y-axis ?

y-axis the the probability of getting this value, in real life terms, y-axis is the frequency in the histogram, noted the probability of getting mean value( the 0 point in x-axis is not 0.5! but about 0.4)

![Normal Distribution Diagram Explained][20]

* * *

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