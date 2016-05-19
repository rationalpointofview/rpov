---
ID: 57
post_title: 'Mental Model, Mathematics,Bayes&#8217;s Theorem'
author: Rational POV
post_date: 2016-04-13 00:56:16
post_excerpt: ""
layout: post
permalink: >
  http://www.rationalpov.com/mental-model-mathematicsbayess-theorem-2/
published: true
---
**Mental Model Name:Bayes's Theorem** 
**Discipline:Mathematics** 
**Lattice Rank :6**

Introductions

> "When my information changes, I alter my conclusions. What do you do, sir?" - John Maynard Keynes

The essense of Bayes's Theorem is, the evidence could have many alternative explanations, and your plausible belief is just one of them.

When you think about it, it means all your belief can be never 100% confirmed, it is merely a plausibility, and this plausibility( probability to be true ) is depends on the evidence.

Through the lens of Baye's themrom, the world is an ever shifting array of probabilities;

[<img src="https://farm6.staticflickr.com/5532/11937781733_bd60ac6a3a_b.jpg" width="1024" height="640" alt="parallel-universe-visiongf-hd-wallpaper-84742" />][1]

Photo by: [Lee Davy][2]

One vivid example can be found in the [Black Swan][3]by Nassim Taleb

> Consider a turkey that is fed everyday. Every single feeding will firm up the bird’s belief that it is the general rule of life to be fed everyday by friendly members of the human race “looking out for its best interests,” as a politician would say. On the afternoon of the Wednesday before Thanksgiving, something unexpected will happen to the turkey. It will incur a revision of belief.



**Why is this important ?**

Even the best of us is subject to the hardwiring of our lizard brains [Confirmation bias][4] and [Avalilability bias][5], and Baye's theorem is a weapon we can use to fight our lizard brain.

Bayes' theorem gives the relationship between the probabilities of A and B, P(A) and P(B), and the conditional probabilities of A given B and B given A, P(A|B) and P(B|A). In its most common form, it is:

![Bayes Theorem][6]

p (A|B) read: probability of A happens given B is true note, P(B) is the overal probability of event B happens

Whats the relationship of A to B ?

A is the your hypothesis/believed fact for now, and you knwo how likely A happens.
B is an evidence approving or disapproving the fact,which you have a math model of A's response.

What do you mean by math model ?

Basically two things:

Positive: when Apply Test B to A, what's the % of B turn out true while A is true

False Positive: When Apply Test B to A, what's the % of B is true while A is not true


Note. Evidence/Test (B) is almost impossible to be 100 % by definition:


*   false positive: A is not true, but Test B say it is true.

Using the turkey example, the false positive is human is not turkey's friend, but they still feed the turkey's

*   false negative: A is true, but Test B say it is not true.

The false negative is human is turkey's friend, but they don't feed us.

If you want to access the strengh of the Belief/hypothesis (A), then you need to also access the strengh of the evidence(B) supporting your hypothese.

**The strengh of the evidence is depends on how many alternate explaination of evidence (B) could have. the fewer the alternate explaintion of evidence, the stronger the evidence.**

Lets use the turkey example again:

Turkey's Believe/Hypothesis (A):

> the human race is our friend and will look after our best interest.

Evidence (B)

> Huamn has fed us every day for 364 days !

From a Turkey prospertive:

From Turkey's propective, The Evidence of the believe( Human is a friend) is "humans feed us everyday".

But the evidence "humans feed us everyday" could have many alternative explanations, thus a weak evidence.

when we examine the Evidence (B)( "Human fed us every day" ), it could have the following alterative explaination

*   Alternate explaination A: Human feed us unconditionally because they are our friends.
*   Alternate explaination B: Human being is feeding us for their own purpose, 

The Evidence "Human fed us every day" can't distinguish between two Alternate Explaination.


**How to use this mental Model**:

*   Write down your current believe/Hypothesis A

*   Write down your evidence B.

*   Build The Math Model between A and B:

    *   Find out the base rate of A 
    *   Find out the possiblity of B is true given A is true
    *   Find out the overall possiblity of B is true
        *   Brain Storm/List out any reasons you can think of to cause event B to happen, and the probability associate with it.


*   Find out the following data:

False positive Rate of the test/evidence(B)

False Negative Rate of the test/evidence(B)

**Predictions:**

Give the probability of A when B is true;

___

**Example**

In an excellent [real life example by Allen Downey][7]

![House fire?](https://upload.wikimedia.org/wikipedia/commons/9/96/ShadowRidgeRoadFire.JPG)
> I had a chance to practice Bayesian inference in real life today: at 1pm my wife called to tell me that the carbon monoxide (CO) alarm at the house was going off. Immediately two hypotheses came to mind: (1) there is a dangerous amount of CO in my house, (2) it's a false alarm.
> 
> It's summer and all the windows are open in the house. The furnace is not running and we don't have a gas stove. And the detector is about 10 years old. This background information makes a false alarm more plausible, so I started with a low prior for (1). Since my wife was on her way out anyway, I suggested she disconnect the detector, turn on a fan, and leave.
> 
> After we hung up, I searched for information on CO detectors and false alarms. Apparently, the rate of false alarms is low, at least in once sense: CO detectors are very specific, that is, unlikely to go off because of anything other than CO. Of course the other possibility is that the detector is broken. On balance, this information made me less confident of a false alarm.

So write down your current believe/hypothesis you want to confirm/disconfirm:

> your house is on fire

The we estimate the chance of house on fire

> The FEMA U.S. Fire Administration keeps stats on fires
> 
> In 2010 there were 362,100 residential fires in the USA. In total the fires caused $6.65 billion in damages.
> 
> According to the Census there are 131 million housing units in the US and 114 million households.
> 
> As far as frequency you could figure that 0.317% of households experienced a fire in 2010. Or we could say that 0.276% of housing units had a fire in the year.

Lets be safe and just put the base rate of house catching fire on 2.7%, which is 10 times higher than national average.

We have our Evidence too, the C/O detctor goes off.

Then we Brain Storm/List out any reasons you can think of to cause the C/O detector to goes off

> *   A fire broken off
> *   The dectector malfunctioned and give false alarm
> *   A major street nearby is being paved. Does fresh pavement off-gas anything that would set off a CO detector? At a construction site down the street, they just poured a concrete foundation, and my neighbor is having some masonry done. Does fresh concrete off-gas CO? I vaguely remember that it sequesters oxygen, which turned out to be a problem for one of the Biosphere projects.
> *   What about a smoldering fire inside a wall? Could it produce enough CO to set off the detector, but not enough smoke to set off the smoke alarms?

A rough estimatation of fire alarm reliability is the following, by doing some google search:

[Reliability:][8]75% [False Positive Rate:][9] 15%

By a quick look at the possible causes:

The alarm trigged by street paving is quite unlikely, as it should trigger other house's fire alarm too( which is not happening). so just put a guesstimate probability of 0.5%.

And the fire alarm false positive and reliability rate for smoldering fire is similar to flaming fire, so probably we can combine these two plausible causes.

Then use Use Bayes Theorem to plugin in the equation and find out how possible it it.

P(fire|alarm) = P(alarm|fire) *P(fire)/P(alarm) = 0.75*0\.03/(0.75*0\.03 + 0.97*0\.15 + 0.005)

= 0.0225/(0.0225+0.1455+0.005)= 13 %

so the it doesn't seem so bad after all.

Given that said, this just an example for baysian analysis, if the fire alarm goes off, please follow the protocol and do what every baysian should do, leave the house and call the fire department !

___

**Examples**

Concrete example from [5 August 2011 New York Times article by John Allen Paulos][10]:

![3 gold coin](https://upload.wikimedia.org/wikipedia/commons/5/5a/NNC-US-1907-G$20-Saint_Gaudens_(Roman,_high_relief)_%E2%80%93_edge_detail.jpg)

Assume that you’re presented with three coins, two of them fair and the other a counterfeit that always lands heads. If you randomly pick one of the three coins, and flip it 3 times, you observed the chosen coin has landed head 3 times in a row.

Question: what is the probablity of you picked a counterfeit coin ?

Before you flip the coin, the probability of the coin is counterfeit is 1 in 3

P(counterfeit) = 0.33

After the flip the coin 3 time (3H, The test), and we want to know the probabilty of the coint is counterfei, P(P):

P(C|3H) = P(3H|C) * P(P) / P(3H)

P(3H|C) = 1 P(P) = 0.33 P(3H)= P(3H|NC) + P(3H|NC) + P(3H|C) = 0.5*0\.5*0\.5*0\.33 + 0.5*0\.5*0\.5*0\.33 + 1*0.33 = 0.4125

P(C| 3H )= 1* 0.33/0.4125 = 0.33/0.4125 = 80%

So after the test, we are 80% confident that the coin is a counter feit.

**Examples**

The chance that a woman will develop breast cancer in her forties is fortunately quite low — about 1.4 percent. But what is the probability if she has a positive mammogram?

Studies show that if a woman does not have cancer, a mammogram will incorrectly claim that she does only about 10 percent of the time. If she does have cancer, on the other hand, they will detect it about 75 percent of the time.

what is the probability of the woman has breast cancer giving positive manmogram ?

We want to know P(BC|MT)

P(MT)= mammogram is true; P(BC) = Breast Cancel is true;

P(BC|MT)= P(MT|BC)*P(BC)/P(MT)

= 0.75 * 0.014/(0.014 * 0\.75+ (1-0.014)*0\.1) = 0.0105 /( 0.0105+0.0986) = 9.6%

So even the memogram is true, the probability of the women got breast cancer is only 9.6 %

Why is that ? it is because the base rate of cancer happening is very low 1.4% , and for P(MT) it could either because of a positive result of a breast cancel or a false positive of a non breast cancer.

[According to this study][11]screening with mammography uss X-ray is not worth the cost;


**Example**

In the Nate Silver's Books [The Signal and the Noice][12]

There is a vivid example of applying Bayes Theorem

> Consider a somber example: the September 11 attacks. Most of us would have assigned almost no probability to terrorists crashing planes into buildings in Manhattan when we woke up that morning. But we recognized that a terror attack was an obvious possibility once the first plane hit the World Trade Center. And we had no doubt we were being attacked once the second tower was hit. Bayes's theorem can replicate this result.

How do we simulated the induction process using Bayes Theorem ?


P(T)= P(Terrorist Attack) 

P(P)= P(Planes crashing into Manhattan Building)

and We want to know:

P(T|P)

P(T|P) = P(C|T)* P(T)/P(P)


Lets gathering base rates:

In the previous 25000 days of aviation over Manhattan prior to 9-11, there had been only two such accidencts.

so P(P) = 2/25000 = 0.008%

and P(T) we can assign an arbitary intial rate: like 0.005%

__Before the first plane hits the twin tower, we have:__

P(T) = 0.005%
P(P|T) = 0.00 % , it is all good

__At the moment the first plane crahsed into the twin tower.__

P(T) = 0.005%

P(P|T) = 100 %

P(P) = 0.008% + 0.005%

P(T|P) = 1*0.00005/(0.00005+0.00008) = 38%

so with the new evidence, the probablility of P(T|C) revised to 38%

__at the moment of second plane hits the twin tower:__


P(T) = 38%
P(2P|T) = 100%
P(2P) = 0.008% * 0.008% + 1 * 38%= 0.3800000064

P(T|2P) = P(2P|T)*P(T)/P(2P)

P(2P|T) = 100% P(T) = 38% /P(2C)=38%/(0.008%*0.008% + 38%)= 99.99%

by the time the 2nd plane hits the twin tower, we can almost certain it is a Terro Attack.

___
**Example**

A reader from Quora poses a questioin:

> What does it mean when a girl smiles at you every time she sees you ?

Another reader using Bayes’s Theorem replies:

P(like|smile) = P(smile|like)*p(like)/p(smile)

so you need to gather the base rate data

P(smile|like) = Chance She Smiles at you given she likes you P(like) = Chances She likes you P(smile) = Chances she smile when seeing anyone

Lets assume two extreme:

P(smile) = 1, she smile at everyone

so

P(like|smile) = 1*P(Like)/1 = P(like)

Remember, the strengh of evidence is depends on how many alternative explanation it could have.

so the information of she is smiling at you doesn't mean anything.

But...

if She rarely smiles at someone, but smiles everytime she sees someone she likes, then

P(smile) = 0%. P(smile|like) = 100% P(smile)=P(like)

P(like|smile) = = 1*P(smile)/(0 + P(smile|like))= 100%

In general, to be a true Bayesian, you will gather the background data of how often she smiles at everyone, and how often she smiles at someone she likes etc.

The more often she smiles at everybody, the lower chance she likes you.

___

**Example**:

Marie is getting married tomorrow, at an outdoor ceremony in the desert. In recent years, it has rained only 5 days each year. Unfortunately, the weatherman has predicted rain for tomorrow. When it actually rains, the weatherman correctly forecasts rain 90% of the time. When it doesn't rain, he incorrectly forecasts rain 10% of the time. What is the probability that it will rain on the day of Marie's wedding?

So we want to know:

P(Raining |Forcasted Rain) = P(Forcasted Rain|Raining)*P(Raining)/P(Forcasted Rain)

= 0.9*(5/365)/(0.9*5/365+(360/365)*0.1)= 0.01232/(0.01232+0.08493)= 12.6%

Despite the weatherman's gloomy prediction, there is a good chance that Marie will not get rained on at her wedding.

___

[**Example:**][13]

Suppose that a barrel contains many small plastic eggs. Some eggs are painted red and some are painted blue. 40% of the eggs in the bin contain pearls, and 60% contain nothing. 30% of eggs containing pearls are painted blue, and 10% of eggs containing nothing are painted blue. What is the probability that a blue egg contains a pearl?

P( Contain Pearl | Blue ) = P (Blue | Contain Pearl) * P (Contain Pearl)/P(Blue)

P (Blue | Contain Pearl ) = 0.3 P (Contain Pearl) = 0.4

P(Blue) = P(Blue | Contain Pearl) + P(Blue | Not Contain Pearl) = 0.3*0.4 + (1-0.4) * 0.1 = 0.12 + 0.06

So the answer is = 0.12/0.18 = 66.7%

___

[**Example**][14]

Assume you have a room full of men and women. 70% of the people are women and 30% are men. Additionally, we know from polling every person that 40% of the women’s favorite color is green and 75% of the men’s favorite color is green.

Given that a randomly selected person likes green, what is the probability that the person is a female?”

P(Female | Like Green ) = P ( Like Green | Female ) * P(Female)/P( Like Green) = 0.4*0\.7/(0.4*0\.7+ 0.3*0.75)= 55 %

___

[**Example**][15]

The Monty Hall problem according to Wikipedia states:

> Suppose you're on a game show, and you're given the choice of three doors: Behind one door is a car; behind the others, goats. You pick a door, say No. 1, and the host, who knows what's behind the doors, opens another door, say No. 3, which has a goat. He then says to you, "Do you want to pick door No. 2?" Is it to your advantage to switch your choice?

For simplicity let: D1: The Event of Monty Hall opening door 1. D2: The Event of Monty Hall opening door 2. D3: The Event of Monty Hall opening door 3. C1: The Event of finding the car behind door 1. C2: The Event of finding the car behind door 2. C3: The Event of finding the car behind door 3.

The prior probability of Monty Hall finding a car behind any door is obviously p(C#)=1/3, where P(C1)=P(C2)=P(C3)

P(C1|D3) = P(D3|C1)* P(C1)/P(D3) = 0.5 * 1/3 /0.5 = 1/3

P(C2/D3) = P(D3/C2) * P(C2)/P(D3) = 1*1/3/0.5

[![Monty Hall Problem][16]][17]

___

[**Example**][18]

> Joe is a randomly chosen member of a large population in which 3% are heroin users. Joe tests positive for heroin in a drug test that correctly identifies users 95% of the time and correctly identifies nonusers 90% of the time. To determine the probability that Joe uses heroin (= H) given the positive test result (= E), we apply Bayes' Theorem using the values


P(H|E)= P(E|H)* P(H)/P(E) = 0.95 * 0.03/(0.95 * 0.03 + 0.97*0.1) = 22%

___

[**Example**][19]

> Say you wake up with spots all over your face. You rush to the doctor and he says that 90 percent of the people who have smallpox have the symptoms you have. Since smallpox is often fatal, your first inclination may be to panic.

But but applying the rules of Bayes Themrom, you have no fear:

*   Brain Storm/List out any reasons/causes you can think of to event B to happen
    
    so you ask your docter , what could cause spots all over your face. ?
    
    The doc replies.
    
    *   you have smallpox. 
    *   you have chicken pox.

*   Find out/Estimate the probability base rate of A is happening
    
    *   small pox, about 0.111 percent (or 0.0011) population has this
    *   chickenpox, which by estimation is about 10 times as likely, about 10% of the population has this
    
    Also your doc is kind enough to tell you
    
    *   90 percent of people with smallpox have these spots
    *   80 percent of people with chickenpox have these spots

so P(smallpox|Spots) = P(Spots|smallPox) * P(smallpox)/p(spots) = 0.9 * 0.001/(0.1*0\.8+0.001*0\.9)= 1.11 %

___

[**Example**][20]

In James V Stone excellent book of Bayes' Rule: A Tutorial Introduction to Bayesian Analysis, he mentions a interesting example:

If you walked into a hardware store and asked:

"Have you got fork handles ? "

You was surprised by the Bayesian Shop Owner whom present you with four candles.

The Phrase "Fork Handles" and "Four Candles " are acoustically almost identical.

Put you into the Bayeisan shop owner's shoes:

*   Brain Storm/List out any reasons you can think of to event B(you hear "fork handles") to happen
    
    *   The Customer wants four candles
    *   The Customer Wants fork handles

and since accoustic pattern of Four candles is almost identical of Fork Handles

We assign abitary probablity of

       P(Data | Four Candles ) = 0.6
       P(Data | Fork Handles ) = 0.7
    

And from the Bayesian Shop Owner pass experience,

    * he was asked about Fork Handles only 10 times 
    * he was asked about candles 90 times
    

so P(Four Candles| Data ) = P(Data | Four Candles ) * P(Four Candles) / P(Data)

= 0.6 * 0.9 /(0.6 *0.9 + 0.7 *0.1) = 88%

___

**Example**

[Games of Chance ][21]

Each of four urns is to be sampled once by the player. The first urn contains one red ball and two white balls, the second one red ball and three white balls, the third one red ball and four white balls, and the fourth one red bell and five white balls. The selection of urns is equally probable.

The player picked a red ball; what is the probability that the secon urn, U2, was selected ?

P(U2|Red) = P(Red|U2)P(U2)/( P(RED|U1)+P(RED|U3)+P(RED|U2)+P(RED|U4)) = 1/4*1/4/(1/4*1/3+1/4*1/4+1/4*1/5+1/4*1/6)= 26.3%

**Example**

[Defective Components][21]

Identical components are procured from three vendors for use in the next higher assembly of a production process. forty-five percent of the componente are procured from Vendor 1. 30 percent from Vendor 2, and 25 percent from Vendor 3. The respective percentages of defective: 6, 3, and 2.

What is the probability of a defective component is from vendor 1 ?

P(1|D)=P(D|1)*P(1)/P(D) = 0.06*0\.45/(0.06*0\.45+0.03*0\.3+0.25*0.02)= 65%

[Enviromental Protection][21]

Pollution detection devices of the enviromental protection agency of a certain state can detect excessive enounte of pollutente emitted by factories with a probability of 0.90. and probability of 0.20 that factories not exceeding limits will fail the test. The issue is whether to procure devices with a detection probability of 0.99.even though the increased sensitivity will increase the false alarI probability to 0.22, to apprehend more violators of state statutes. It is estimated around 30 percent of the factories in the state emit excessive pollutants.

Is that worth the investment ?

For the existing device:

P(P|F)= P(F|P)*P(P)/P(F)= 0.9*0\.3/(0.9*0\.3+0.7*0\.2)= 0.27/0.41=65.8%

If we buy the new device:

P('P|'F) = 0.99*0\.3/(0.99*0\.3+0.7*0.22) = 0.297/(0.297+0.154) = 65.8%

So, probably we should not invest in the new device:

[Example: Interview][22]

The Gallup organization randomly selects an adult American for a survey about credit card usage.

a. What is the probability that the selected subject is a male? b. After selecting a subject, it is later learned that this person was smoking a cigar during the interview. What is the probability that the selected subject is a male?

Our Hypothesis for now:

The interviewee is male:

So let try to find out the base rate of our hypothesis:

by some googling, we find out the [% for Male in US is about 49.2%][23]

So before the new evidence of the interviewee is smoking cigar, the base rate probability of the interviewee is male:

P(M)= 49.2

And the Test/Evidence is this interviewee smoke cigar during interview:

We got our much needed statistic data from [CDC][24]

> Current Cigar Use
> 
> Adults:
> 
> Percentage of U.S. adults who were current cigar smokers† in 2013:9
> 
> 5\.0% of all adults 8.2% of adult males 2.0% of adult females 7.5% of African American adults 6.7% of American Indian/Alaska Native adults 2.1% of Asian American adults 4.0% of Hispanic adults 5.0% of White adults

P(P) = 5% P(C|M) = 8.2% Lets plug all the data into Bayes themorem

P(M|C) = P(C|M)*P(M)/P(P) = 8.2% * 49.2% /5% = 80.6%

The probability of the interviewee is a male revised to 80.6%

[Example: Identical Twins][25]

> Elvis Presley had a twin brother who died at birth. What is the probability that Elvis was an identical twin?
> 
> To answer this one, you need some background information: According to the Wikipedia article on twins: ``Twins are estimated to be approximately 1.9% of the world population, with monozygotic twins making up 0.2% of the total---and 8% of all twins.''

So what is the hypothesis we are trying to find out the probability ?

Elvis was an identical twin

and the tricky part is, what the new evidence ?

> Elvis Presley had a twin brother

Presumably Elvis is a boy, and twin brother means same sex, and identical twins, by definition, is always has the same sex, but individual twins probably has 50% to 50% change of different sex( I could be wrong)

plug in the datas to Bayes Themrom, we got:

P(IT|Same Sex) = P(Same Sex| IT)* P(IT)/P(S) = 1* 8%/(92% * 50% + 1* 8%) = 14.8%

[Example: Lung Cancer and Smoking][25]

> According to the CDC, ``Compared to nonsmokers, men who smoke are about 23 times more likely to develop lung cancer and women who smoke are about 13 times more likely.'' If you learn that a woman has been diagnosed with lung cancer, and you know nothing else about her, what is the probability that she is a smoker?

The Hyothesis A:

This Woman is a smoker

A':

This Woman is not a smoker

And the Evidence/New Information:

THis Woman has been diagnosed with lung cancer

Lets find out the base rate first:

According to [CDC][26]:

in 2012

> 210,828 people in the United States were diagnosed with lung cancer, including 111,395 men and 99,433 women.

And 2012 the US population is about 314.1 million.

so the base rate for women diagnosed with lung cancer is:

99433/(314100000/2)= 0.06 %

Also from CDC, we can find the estimation of Adults whom is a smoker:

> By Gender
> 
> Men are more likely to be current cigarette smokers than women.
> 
> Nearly 19 of every 100 adult men (18.8%) Nearly 15 of every 100 adult women (14.8%)

Lets plugin in the equations:

P(S|L) = P(L|S)* P(S)/P(L)

Wait.. We dont know P(L|S) yet .ie. Probability of Smoker got lung cancer:

Fortunately, high school math come into rescue.

lets put P(L|NS) = x ie. the Probability of Women non-smoker got lung cancer:

0.852x + 13(0.148)x = 0.06 % 
2.776x = 0.06% 
x = 0.0216%

and P(L|S) = 13x = 0.28%

lets plug all the numbers into Bayes Equation

P(S|L) = P(L|S)* P(S)/P(L) = 0.28% * 14.8% /( 0.0216% * 85.2 % + 0.28% * 14.8%) = 0.04144%/(0.0184%+0.04144)=0.04144/0.0598 = 69.3%


[Example: Finding the Mole][27]

> So: you're the head of MI6. You're pretty sure there's a "mole" in your organization.
> 
> You've narrowed it down to five suspects: Alan,Bob, Chris,Dave, and Ed.
> 
> You know from previous experience with interrogations that there are five behaviours to be expected in any given session: normal behaviour, nervousness, anger at the accusation, making a mistake in one's story, and a desperate exhausted confession
> 
> you know from experience that moles and loyal operatives will exhibit the five behaviours at different rates.

Behavious of loyal Operatives:

Normal:70% Confess:5% Mistake:10% Angry:5% Nervous:10%

Behaviours of moles:

Normal:55% Confess:10% Mistake:10% Angry:10% Nervous:15%

The probability-of-being-the-mole is 0.2 for each person in this case. This is called a uniform prior.

We begin the interrogation sessions.

Session 1:

lets just use one Agent Alan as an example

P(M|N)= P(N|M) * P(M)/P(N) = 55 % * 20 % /(55 % * 20% + 70% * 80%) = 0.11/0.67 = 0.164

| Agent | Prior Probability | Reaction | Revised Probability of being a Mole |
| ----- | -----------------:| -------- | -----------------------------------:|
| Alan  |              0\.2 | Normal   |                              0\.164 |
| Bob   |              0\.2 | Normal   |                              0\.164 |
| Chris |              0\.2 | Confess  |                              0\.333 |
| Dave  |              0\.2 | Normal   |                              0\.164 |
| Ed    |              0\.2 | Normal   |                              0\.164 |

Session 2

Lets use Ed as example

P(M|C) = P(C|M) * P(M)/P(P) = 0.1*0\.164 /(0.1*0\.164 + 0.05* 0.836)= 0.0164/0.0582= 0.282

| Agent | Prior Probability | Reaction | Revised Probability of being a Mole |
| ----- | -----------------:| -------- | -----------------------------------:|
| Alan  |            0\.164 | Normal   |                              0\.134 |
| Bob   |            0\.164 | Mistake  |                              0\.164 |
| Chris |            0\.333 | Nervous  |                              0\.429 |
| Dave  |            0\.164 | Normal   |                              0\.134 |
| Ed    |            0\.164 | Confess  |                              0\.282 |

. . .

Session 150

| Agent | Prior Probability | Reaction | Revised Probability of being a Mole |
| ----- | -----------------:| -------- | -----------------------------------:|
| Alan  |              0\.0 | Normal   |                                   0 |
| Bob   |              0\.0 | Mistake  |                                   0 |
| Chris |            0\.999 | Nervous  |                                   1 |
| Dave  |            0\.001 | Normal   |                              0\.001 |
| Ed    |                 1 | Confess  |                                   1 |

* * *


[Example: A Bayesian view of Amazon Resellers](http://www.johndcook.com/blog/2011/09/27/bayesian-amazon/)

You want to buy a used book through Amazon, there are two sellers:

Seller A has 90 Positive reviews out of 100, thus a Rating of 90%

Seller B has 2 Positive reviews, thus a Rating of 100%

Which one will you pick ?

The 100% One Right ?

Because we deal with small numbers here, we need to use Beta-Distribution instead of Normal Distribution.

[best explaination of beta distrubtion & Bayesian therom](http://stats.stackexchange.com/questions/47771/what-is-the-intuition-behind-beta-distribution)

The Math behind is somewhat complicated, but you can use this calculator to quickly [judge the numbers](http://www.peakconversion.com/2012/02/ab-split-test-graphical-calculator/):


[Example: A Political Example, From Bayesian Statistics, Peter M. Lee](http://www.amazon.com/Bayesian-Statistics-Introduction-Peter-Lee/dp/1118332571/ref=sr_1_3?ie=UTF8&qid=1463538432&sr=8-3&keywords=Bayesian+Statistics+peter)


>The following example is a simplified version of the situation just before the time of the British national referendum as to whether the United Kingdom should remain part of the European Economic Community which was held in 1975. Suppose that at that date, which was shortly after an election which the Labour Party had won, the proportion of the electorate supporting Labour (L) stood at 52%, while the proportion supporting the Conservatives (C) stood at 48% (it being assumed for simplicity that support for all other parties was negligible, although this was far from being the case). There were many opinion polls taken at the time, so we can take it as known that 55% of Labour supporters and 85% of Conservative voters intended to vote ‘Yes’ (Y) and the remainder intended to vote ‘N o’ (N). Suppose that knowing all this you met someone at the time who said that she intended to vote ‘Yes’, and you were interested in knowing which political party she supported. If this information were all you had available, you could reason as follows: 

P(L|Y)=P(Y|L)* P(L)/P(Y)

= 55% * 52% /( 55% * 52% + 48%* 85%)

= 0.286/(0.286+0.408) = 0.286/0.694 = 41.2 %

She has a 41.2% Belongs to Labour Party

[Example: Forensic AnalysisFrom Bayesian Statistics, Peter M. Lee](http://www.amazon.com/Bayesian-Statistics-Introduction-Peter-Lee/dp/1118332571/ref=sr_1_3?ie=UTF8&qid=1463538432&sr=8-3&keywords=Bayesian+Statistics+peter)

![blood test](https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/eu85w0il.png)

>Suppose a crime has been committed. Blood is found at the scene for which there is no innocent explanation. It is of a type which is present in 1% of the population. The prosecutor may then state: 

>‘There is a 1% chance that the defendant would have the crime blood type if he were innocent. Thus, there is a 99% chance that he is guilty’ . 

>Alternatively, the defender may state: 

>‘This crime occurred in a city of 800,000 people. This blood type would be found in approximately 8000 people. The evidence has provided a probability of l in 8000 that the defendant is guilty and thus has no relevance.’ 

Which one is correct ? Armed with Baysian thinking, you find out both argument is not correct.

Lets Apply the Baysian Theorem here:

Believe:

The Suspect is Guity:

Evidence: 

The Suspect has the same blood type of the crime scene

Basic Data:

Priors: 

P(Guity) = 1/800000

P(Equal Blood Type| Guity) = 1

P(Equal Blood Type)= 8000/800000


P(Guilty|Equal Blood Type) = P (Equal Blood Type| Guilty)* P(Guity)/P(Equal Blood Type)
= 1 * 1/800000/(8000/800000)

With the new evidence of the suspect has the same blood type of the crime scene, the Postier Probability of P(Guity) change from 1/800000 to 1/8000


> Such a large change in the odds is, in Aitken’s words ‘surely of relevance’ . But, again In Aitken’s words, ‘Of course, it may not be enough to find the suspect guilty’. 


** Bonus 

[Bayesian Vesus Frequentist] (http://www.win-vector.com/blog/2013/05/bayesian-and-frequentist-approaches-ask-the-right-question/)

The difference between Bayesian vesus Fequentist is the question we are asking:

> Frequentist: Worry about correctness and repeatability, not p-values
> Bayesian: Focused on P value;

Example:

You went to see the doctor about your high blood pressure problem:

Freqentist Docotor:

>“If I prescribe drugX to all my hypertensive patients, will their blood pressure improve, on average?” 

Baesian Doctor:

>“If I prescribe drugX to this patient, the one sitting in my examination room, will the patient’s blood pressure improve?” "




More Resources:

[more examples][28]

[More examples ][29]

[A visual Explaination of Bay's Themrom][30]





[Think Bayes From Greenteapress][31]

 [1]: https://www.flickr.com/photos/chingster23/11937781733 "parallel-universe-visiongf-hd-wallpaper-84742"
 [2]: https://www.flickr.com/photos/chingster23/11937781733
 [3]: http://www.amazon.com/exec/obidos/ASIN/081297381X/
 [4]: https://en.wikipedia.org/wiki/Confirmation_bias
 [5]: https://en.wikipedia.org/wiki/Availability_heuristic
 [6]: https://upload.wikimedia.org/math/d/3/c/d3c7c452b3d01f5415dd9bf15d2ab822.png
 [7]: http://allendowney.blogspot.hk/2015/08/bayes-theorem-in-real-life.html
 [8]: http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.586.5246&rep=rep1&type=pdf
 [9]: http://fire.nist.gov/bfrlpubs/fire89/PDF/f89012.pdf
 [10]: http://www.nytimes.com/2011/08/07/books/review/the-theory-that-would-not-die-by-sharon-bertsch-mcgrayne-book-review.html?_r=0
 [11]: http://www.cochrane.org/CD001877/BREASTCA_screening-for-breast-cancer-with-mammography
 [12]: http://www.amazon.com/The-Signal-Noise-Predictions-Fail-but/dp/0143125087
 [13]: http://www.yudkowsky.net/rational/bayes
 [14]: http://blog.claymcleod.io/2016/02/02/Bayes-Theorem-for-Computer-Scientists/
 [15]: https://www.quora.com/How-do-I-solve-the-Monty-Hall-Problem-using-Bayes-Theorem
 [16]: https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/k9wgpe73.png
 [17]: https://youtu.be/4Lb-6rxZxx0
 [18]: http://plato.stanford.edu/entries/bayes-theorem/supplement.html
 [19]: https://lloydmelnick.com/2014/01/21/bayes-theorem-part-1-why-bayes-rule-is-the-key-to-good-decision-making-and-success/
 [20]: http://www.amazon.com/Bayes-Rule-Tutorial-Introduction-Bayesian/dp/0956372848/ref=sr_1_1?ie=UTF8&qid=1391446909&sr=8-1&keywords=Bayes+rule
 [21]: http://www.value-eng.org/knowledge_bank/attachments/Bayes%20Theorem%20in%20Decision%20Making.pdf
 [22]: http://faculty.washington.edu/tamre/BayesTheorem.pdf
 [23]: http://www.infoplease.com/ipa/A0884102.html
 [24]: http://www.cdc.gov/tobacco/data_statistics/fact_sheets/tobacco_industry/cigars/
 [25]: http://allendowney.blogspot.hk/2011/10/all-your-bayes-are-belong-to-us.html
 [26]: http://www.cdc.gov/cancer/lung/statistics/
 [27]: http://users.ecs.soton.ac.uk/jn2/teaching/bayes.pdf
 [28]: http://www.rigb.org/christmaslectures08/html/activities/learning-from-probabilities.pdf
 [29]: http://www.greenteapress.com/thinkbayes/html/thinkbayes006.html#toc41
 [30]: https://www.countbayesie.com/blog/2015/2/18/bayes-theorem-with-lego
 [31]: http://www.greenteapress.com/thinkbayes/thinkbayes.pdf