---
ID: 94
post_title: 'Mental Model, Mathematics,Bayes&#8217;s Theorem'
author: Rational POV
post_date: 2016-01-27 01:49:05
post_excerpt: ""
layout: post
permalink: >
  http://www.rationalpov.com/blog/mental-model-mathematicsbayess-theorem/
published: true
---
**Mental Model Name:Bayes's Theorem** 
**Discipline:Mathematics** 
**Lattice Rank :6**

Introductions

> "When my information changes, I alter my conclusions. What do you do, sir?" - John Maynard Keynes
 
If you want to access the strengh of the hypothesis (A), then you need to also access the strengh of the evidence given your hypothese (B).

Mathematically, Bayes' theorem gives the relationship between the probabilities of A and B, P(A) and P(B), and the conditional probabilities of A given B and B given A, P(A|B) and P(B|A). In its most common form, it is:

![Bayes Theorem](https://upload.wikimedia.org/math/d/3/c/d3c7c452b3d01f5415dd9bf15d2ab822.png)

whats the relationship of A to B ?

p (A|B) read: probability of A happens given B is true
note, P(B) is the overal probability of event B happens

A is the your hypothesis, ( usually an intrinsic fact), and  B is an evidene, or a test results, to support your hypothesis. 

The tricks is , Test B is almost impossible to be 100 % accuate, the errors can be:

* false positive: A is not true, but Test B say it is true.
* false negative: A is true, but Test B say it is not true.

you can imaging A is a elephant, and B is an blind observer and try to determine what is he touching.

note, the event A is not going to interference B, mainly an observer event, use decision tree to understand this.

This Theorem is better understand from an example.



**How to use this mental Model**:

Use it to understand the true implications of test results, and the realization of it is impossible to confirms a theory, merely test it and the result will be infintely close 100% but never reach it.

The key is to look at the world as an ever shifting array of probabilities and to remember the limitations. One such limitation can be explained by Nassim Taleb in the [Black Swan](http://www.amazon.com/exec/obidos/ASIN/081297381X/)

>Consider a turkey that is fed everyday. Every single feeding will firm up the bird’s belief that it is the general rule of life to be fed everyday by friendly members of the human race “looking out for its best interests,” as a politician would say. On the afternoon of the Wednesday before Thanksgiving, something unexpected will happen to the turkey. It will incur a revision of belief.


**Conditions:**

The Event A is statistical event, with fairly low probability of A happening.

The Event B is test or evidence related to A, and you know 2 data points:

False positive Rate of the test/evidence

False Negative Rate of the test/evidence



**Predictions:**

Give the outcome of P(A) is true give B is true:


**Examples**

Concrete example from [5 August 2011 New York Times article by John Allen Paulos](http://www.nytimes.com/2011/08/07/books/review/the-theory-that-would-not-die-by-sharon-bertsch-mcgrayne-book-review.html?_r=0):

Assume that you’re presented with three coins, two of them fair and the other a counterfeit that always lands heads. If you randomly pick one of the three coins, and flip it 3 times, you observed the chosen coin has landed head 3 times in a row.

Question: what is the probablity of you picked a counterfeit coin ?

Before you flip the coin, the probability of the coin is counterfeit is 1 in 3

P(counterfeit) = 0.33

After the flip the coin 3 time (3H, The test), and we want to know the probabilty of the coint is counterfei, P(C):

P(C|3H)  =  P(3H|C) * P(C) / P(3H)

P(3H|C) = 1
P(C) = 0.33
P(3H)= P(3H|NC) + P(3H|NC) + P(3H|C) = 0.5*0.5*0.5*0.33 + 0.5*0.5*0.5*0.33 + 1*0.33 = 0.4125

P(C| 3H )= 1* 0.33/0.4125 = 0.33/0.4125 = 80%

So after the test, we are 80% confident that the coin is a counter feit.


**Examples**

 The chance that a woman will develop breast cancer in her forties is fortunately quite low — about 1.4 percent. But what is the probability if she has a positive mammogram?

Studies show that if a woman does not have cancer, a mammogram will incorrectly claim that she does only about 10 percent of the time. If she does have cancer, on the other hand, they will detect it about 75 percent of the time.

what is the probability of the woman has Breas Cancel giving positive manmogram ?

We want to know P(BC|MT)

P(MT)= mammogram is true;
P(BC) = Breast Cancel is true;

P(BC|MT)= P(MT|BC)*P(BC)/P(MT)

= 0.75 * 0.014/(0.014*0.75+ (1-0.014)*0.1)
= 0.0105 /( 0.0105+0.0986)
= 9.6%

So even the memogram is true, the probability of the women got breast cancer is only 9.6 %

[According to this study](http://www.cochrane.org/CD001877/BREASTCA_screening-for-breast-cancer-with-mammography)screening with mammography uss X-ray is not worth the cost

**Example**

In the Nate Silver's Books [The Signal and the Noice](http://www.amazon.com/The-Signal-Noise-Predictions-Fail-but/dp/0143125087)

There is a vivid example of applying Bayes Theorem

> Consider a somber example: the September 11 attacks. Most of us would have assigned almost no probability to terrorists crashing planes into buildings in Manhattan when we woke up that morning. But we recognized that a terror attack was an obvious possibility once the first plane hit the World Trade Center. And we had no doubt we were being attacked once the second tower was hit. Bayes's theorem can replicate this result.

So we want to know the following facts

P(T)= P(Terrorist Crashing Planes into Building)
P(C)= P( Planes crashing into Building)

and We want to know:

P(T|C) 

P(T|C) = P(C|T)* P(T)/P(C)

we gathering base rates:

In the previous 25000 days of aviation over Manhattan prior to 9-11, there had been only two such accidencts.

so P(C) = 2/25000 = 0.008%

and P(T) we can assign an arbitary intial rate: like 0.005%

so before the plane hits the twin tower, P(C|T) is not true, so the probablilty is just 0.005%

but at the moment the first planes hits the twin tower, P(C|T) = 100 %

P(T|C) = 1*0.00005/(0.00005+0.00008) = 38%

so with the new evidence, the probablility of P(T|C) revised to 38%

at the moment of second plane hits the twin tower:

P(T|2C) = P(2C|T)*P(T)/P(2C)

P(2C|T) = 100%
P(T) = 38%
P(2C)=(0.008%*0.008% + 38%)= 99.99%

** Example **

A reader from Quora poses a questioin: 

> What does it mean when a girl smiles at you every time she sees you ?
> 

Another reader using Bayes’s Theorem replies:

P(like|smile) = P(smile|like)*p(like)/p(smile)

so you need to gather the base rate data

P(smile|like) = Chance She Smiles at you given she likes you
P(like) = Chances She likes you
P(smile) = Chances she smile when seeing anyone

Lets assume two extreme:

P(smile) = 1, she smile at everyone

so 

P(like|smile) = 1*P(Like)/1 = P(like)

so the information of she is smiling at you doesn't mean anything.

But...

if She rarely smiles at someone, but smiles everytime she sees someone she likes, then

P(smile) = 0%.
P(smile|like) = 100%
P(smile)=P(like)

P(like|smile) = = 1*P(smile)/(0 + P(smile|like))= 100%

In general, to be a true Bayesian, you will gather the background data of how often she smiles at everyone, and how often she smiles at someone she likes etc.

The more often she smiles at everybody, the lower chance she likes you.


**Example**:

Marie is getting married tomorrow, at an outdoor ceremony in the desert. In recent years, it has rained only 5 days each year. Unfortunately, the weatherman has predicted rain for tomorrow. When it actually rains, the weatherman correctly forecasts rain 90% of the time. When it doesn't rain, he incorrectly forecasts rain 10% of the time. What is the probability that it will rain on the day of Marie's wedding?

So we want to know:

P(Raining |Forcasted Rain) = P(Forcasted Rain|Raining)*P(Raining)/P(Forcasted Rain)

= 0.9*(5/365)/(0.9*5/365+(360/365)*0.1)= 0.01232/()= 11.1 %

Despite the weatherman's gloomy prediction, there is a good chance that Marie will not get rained on at her wedding.





















