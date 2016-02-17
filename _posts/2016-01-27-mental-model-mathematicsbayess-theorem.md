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

**Why is this important ?**

Use it to understand the true implications of test results, and the realization of it is impossible to confirms a theory, merely test it and the result will be infintely close 100% but never reach it.

The key is to look at the world as an ever shifting array of probabilities and to remember the limitations. One such limitation can be explained by Nassim Taleb in the [Black Swan](http://www.amazon.com/exec/obidos/ASIN/081297381X/)

>Consider a turkey that is fed everyday. Every single feeding will firm up the bird’s belief that it is the general rule of life to be fed everyday by friendly members of the human race “looking out for its best interests,” as a politician would say. On the afternoon of the Wednesday before Thanksgiving, something unexpected will happen to the turkey. It will incur a revision of belief.

The essential thing to this theorem, is you need to consider all posibility the could be the causing the new evidence( Information, in Keynes words).

Conceptually, Bayes’ system was simple. We modify our opinions with objective information: Initial Beliefs + Recent Objective Data = A New and Improved Belief.

If you want to access the strengh of the hypothesis (A), then you need to also access the strengh of the evidence given your hypothese (B).

Mathematically, Bayes' theorem gives the relationship between the probabilities of A and B, P(A) and P(B), and the conditional probabilities of A given B and B given A, P(A|B) and P(B|A). In its most common form, it is:

![Bayes Theorem](https://upload.wikimedia.org/math/d/3/c/d3c7c452b3d01f5415dd9bf15d2ab822.png)

the key to really understanding Bayes’ theorem is recognizing that the denominator is actually just the law of total probability



whats the relationship of A to B ?

p (A|B) read: probability of A happens given B is true
note, P(B) is the overal probability of event B happens

A is the your hypothesis, ( usually an intrinsic fact), and  B is an evidene, or a test results, to support your hypothesis. 

The tricks is , Test (B) is almost impossible to be 100 % accuate, the errors can be:

* false positive: A is not true, but Test B say it is true.
* false negative: A is true, but Test B say it is not true.

This Theorem is better understand from an example.


In an excellent [real life example by Allen Downey](http://allendowney.blogspot.hk/2015/08/bayes-theorem-in-real-life.html)

> I had a chance to practice Bayesian inference in real life today: at 1pm my wife called to tell me that the carbon monoxide (CO) alarm at the house was going off.  Immediately two hypotheses came to mind: (1) there is a dangerous amount of CO in my house, (2) it's a false alarm.

> It's summer and all the windows are open in the house.  The furnace is not running and we don't have a gas stove.  And the detector is about 10 years old.  This background information makes a false alarm more plausible, so I started with a low prior for (1).  Since my wife was on her way out anyway, I suggested she disconnect the detector, turn on a fan, and leave.

> After we hung up, I searched for information on CO detectors and false alarms.  Apparently, the rate of false alarms is low, at least in once sense: CO detectors are very specific, that is, unlikely to go off because of anything other than CO.  Of course the other possibility is that the detector is broken.  On balance, this information made me less confident of a false alarm.

First Step to use Bayes Theorem is to Brain Storm/List out any reasons you can think of to cause the C/O detector to goes off

> * A fire broken off
> * The dectector malfunctioned
> * A major street nearby is being paved.  Does fresh pavement off-gas anything that would set off a CO detector?
At a construction site down the street, they just poured a concrete foundation, and my neighbor is having some masonry done.  Does fresh concrete off-gas CO?  I vaguely remember that it sequesters oxygen, which turned out to be a problem for one of the Biosphere projects.
>* What about a smoldering fire inside a wall?  Could it produce enough CO to set off the detector, but not enough smoke to set off the smoke alarms?
 

Then use Use Bayes Themrom to plugin in the equiation and find out how possible it it.

P(Detector Malfunctioned| Dectector goes Off) = P(Dectector goes off | Dectector Malfunctioned) * P(Dectector Malfunctioned)/(P(Dectector off))

Now Assume P(Dectector Goes off | Dector Malfunction) = 1

and you need to find out the base rate of P(Dectector Malfunctioned)

and all the probability of P(Dectector goes off)





**How to use this mental Model**:

* Brain Storm/List out any reasons you can think of to event B to happen
* Find out/Estimate the probability base rate of A is happening


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

Why is that ? it is because the base rate of cancer happening is very low 1.4% , and for P(MT) it could either because of a positive result of a breast cancel or a false positive of a non breast cancer.



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

**Example**

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

Marie is getting m`arried tomorrow, at an outdoor ceremony in the desert. In recent years, it has rained only 5 days each year. Unfortunately, the weatherman has predicted rain for tomorrow. When it actually rains, the weatherman correctly forecasts rain 90% of the time. When it doesn't rain, he incorrectly forecasts rain 10% of the time. What is the probability that it will rain on the day of Marie's wedding?

So we want to know:

P(Raining |Forcasted Rain) = P(Forcasted Rain|Raining)*P(Raining)/P(Forcasted Rain)

= 0.9*(5/365)/(0.9*5/365+(360/365)*0.1)= 0.01232/()= 11.1 %

Despite the weatherman's gloomy prediction, there is a good chance that Marie will not get rained on at her wedding.


[**Example:**](http://www.yudkowsky.net/rational/bayes)

Suppose that a barrel contains many small plastic eggs.  Some eggs are painted red and some are painted blue.  40% of the eggs in the bin contain pearls, and 60% contain nothing.   30% of eggs containing pearls are painted blue, and 10% of eggs containing nothing are painted blue.  What is the probability that a blue egg contains a pearl? 

P( Contain Pearl | Blue ) = P (Blue | Contain Pearl) * P (Contain Pearl)/P(Blue)

P (Blue | Contain Pearl ) = 0.3
P (Contain Pearl) = 0.4

P(Blue) = P(Blue | Contain Pearl) + P(Blue | Not Contain Pearl)
= 0.3*0.4 + (1-0.4) * 0.1
= 0.12 + 0.06

So the answer is = 0.12/0.18 = 66.7%


[**Example:**
](https://www.reddit.com/r/PNWS/comments/3wbm7r/the_black_tapes_i_did_the_math_bayes_theorem_in/)

Here is a fun example from Reddit:

In episode 102, Sebastian's mother says that every photo of Sebastian has the shadow man in it. When Alex tests this prediction against the evidence of the school photos, the school photos pass the test, but Dr. Strand remains unconvinced. Is he being closed-minded? Or is his continued skepticism justified?

Let's say there are 20 students in the class. Out of 21 photos, 2 had the shadow, exactly the two that had Sebastian in them. The photographer says that such artifacts can happen naturally in digital photos, so she doesn't think much of it. What's the probability of it just naturally happening in those two photos?


[**Example**](http://blog.claymcleod.io/2016/02/02/Bayes-Theorem-for-Computer-Scientists/)

Assume you have a room full of men and women. 70% of the people are women and 30% are men. Additionally, we know from polling every person that 40% of the women’s favorite color is green and 75% of the men’s favorite color is green.

Given that a randomly selected person likes green, what is the probability that the person is a female?”

P(Female | Like Green ) = P ( Like Green | Female ) * P(Female)/P( Like Green)
= 0.4*0.7/(0.4*0.7+ 0.3*0.75)= 55 %

[**Example**](https://www.quora.com/How-do-I-solve-the-Monty-Hall-Problem-using-Bayes-Theorem)

The Monty Hall problem according to Wikipedia states:

>Suppose you're on a game show, and you're given the choice of three doors: Behind one door is a car; behind the others, goats. You pick a door, say No. 1, and the host, who knows what's behind the doors, opens another door, say No. 3, which has a goat. He then says to you, "Do you want to pick door No. 2?" Is it to your advantage to switch your choice?

For simplicity let:
D1: The Event of Monty Hall opening door 1.
D2: The Event of Monty Hall opening door 2.
D3: The Event of Monty Hall opening door 3.
C1: The Event of finding the car behind door 1.
C2: The Event of finding the car behind door 2.
C3: The Event of finding the car behind door 3.

The prior probability of Monty Hall finding a car behind any door is obviously p(C#)=1/3, where P(C1)=P(C2)=P(C3)

P(C1|D3) = P(D3|C1)* P(C1)/P(D3) =  0.5 * 1/3 /0.5 = 1/3

P(C2/D3) = P(D3/C2) * P(C2)/P(D3) = 1*1/3/0.5

https://youtu.be/4Lb-6rxZxx0

[**Example**](http://plato.stanford.edu/entries/bayes-theorem/supplement.html )

>Joe is a randomly chosen member of a large population in which 3% are heroin users. Joe tests positive for heroin in a drug test that correctly identifies users 95% of the time and correctly identifies nonusers 90% of the time. To determine the probability that Joe uses heroin (= H) given the positive test result (= E), we apply Bayes' Theorem using the values

P(H|E)= P(E|H)* P(H)/P(E) = 0.95 * 0.03/(0.95 * 0.03 + 0.97*0.1) = 22%



[**Example**](https://lloydmelnick.com/2014/01/21/bayes-theorem-part-1-why-bayes-rule-is-the-key-to-good-decision-making-and-success/)

> Say you wake up with spots all over your face. You rush to the doctor and he says that 90 percent of the people who have smallpox have the symptoms you have. Since smallpox is often fatal, your first inclination may be to panic. 


But but applying the rules of Bayes Themrom, you have no fear:

* Brain Storm/List out any reasons/causes you can think of to event B to happen

    so you ask your docter , what could cause spots all over your face. ?

    The doc replies. 

    - you have smallpox. 
    - you have chicken pox.

* Find out/Estimate the probability base rate of A is happening

    - small pox, about 0.111 percent (or 0.0011) population has this
    - chickenpox, which by estimation is about 10 times as likely, about 10% of the population has this

    Also your doc is kind enough to tell you

    - 90 percent of people with smallpox have these spots
    - 80 percent of people with chickenpox have these spots

so P(smallpox|Spots) = P(Spots|smallPox) * P(smallpox)/p(spots)
= 0.9 * 0.001/(0.1*0.8+0.001*0.9)= 1.11 %

[**Example**](http://www.amazon.com/Bayes-Rule-Tutorial-Introduction-Bayesian/dp/0956372848/ref=sr_1_1?ie=UTF8&qid=1391446909&sr=8-1&keywords=Bayes+rule)

In James V Stone excellent book of Bayes' Rule: A Tutorial Introduction to Bayesian Analysis, he mentions a interesting example:

If you walked into a hardware store and asked:

"Have  you got fork handles ? "

You was surprised by the Bayesian Shop Owner whom present you with four candles.

The Phrase "Fork Handles" and "Four Candles " are acoustically almost identical.

* Brain Storm/List out any reasons you can think of to event B(you hear "fork handles") to happen

    * The Customer wants four candles
    * The Customer Wants fork handles
    

and since accoustic pattern of Four candles is almost identical of Fork Handles

We assign abitary probablity of 

       P(Data | Four Candles ) = 0.6
       P(Data | Fork Handles ) = 0.7

And from the Bayesian Shop Owner pass experience, 

    * he was asked about Fork Handles only 10 times 
    * he was asked about candles 90 times

so P(Four Candles| Data )  = P(Data | Four Candles ) * P(Four Candles) / P(Data)

= 0.6 * 0.9 /(0.6 *0.9 + 0.7 *0.1) = 88%


[more examples](http://www.value-eng.org/knowledge_bank/attachments/Bayes%20Theorem%20in%20Decision%20Making.pdf) 

[more examples](http://www.rigb.org/christmaslectures08/html/activities/learning-from-probabilities.pdf)
















