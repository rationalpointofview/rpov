---
ID: 73
post_title: >
  Mental Model, Mathematics,Combinations
  and Permutations
author: Rational POV
post_date: 2016-01-20 00:43:43
post_excerpt: ""
layout: post
permalink: >
  http://www.rationalpov.com/blog/mental-model-mathematicscombinations-and-permutations/
published: true
---


**Mental Model Name:elementary math of permutations and combinations**
**Discipline:Mathematics  ** 
**Lattice Rank:4 **

>Elementary math of permutations and combinations, It's very simple algebra. It was all worked out in the course of about one year between Pascal and Fermat. They worked it out casually in a series of letters.

>It's not that hard to learn. What is hard is to get so you use it routinely almost everyday of your life. The Fermat/Pascal system is dramatically consonant with the way that the world works. And it's fundamental truth. So you simply have to have the technique.

Why Pascal and Fermat work this out ? They work this work for ... Gambling.



**What is Combinations and Permutations**:


When the order doesn't matter, it is combinations;

When the order does matter, it is permutations


**Permutatations is the easier one to Explain:**

There are two types of Permutations;

* One Allows Repetition, (Like the Combination Lock Example)

Imaging you walk into a Hall, and In front of you there are 10 Doors and each labeled 1-10.

When allows repetitions, we dont take aways the choices, so each time there will be the same numbers of choices, say 10 doors to choose from , if we choice r number of times, it will be 10^r, Thats the Total Number of Permutations when Repetitions is allowed.

So the Formular for Combinations with Repetions is:

**N^r**

* One Doesn't Allow Repetitions.

When doesn't allows repetitions, after we choose one doors, the Door will vanish from the hall and not avaliable to be choosen next time.

So First time you will got 10 Doors to choose from, after choosen one doors, next time it will be only 9 Doors, each Iteration you will has one doors less to choose from.

then the computations will be  (N)(N-1)(N-2)...

So the Formular for Combinations without Repetions is:

**N!**

**Combinations**

There are also two types of Combinations:

* One Doesn't Allows Repetition

Example: Lottery, you pick 7 numbers, the order of this 7 numbers doesn't matter, but you can't pick the same number twice.

we can simplify it as Permutations, then reduce it to combinations

say we want to know the possibilities of picking R balls out of a Pool of N, then

The Permutations = N!/(N-R)!, and remember, how many permutations does R balls has ? R!

the R balls could have a permutations of R! iteself, which we dont quite care and all the same to us now, so reduced the choice by R! number of times,

so Combinations without repetion = Permutations without repetitions / R!


* One Allows Repetion

Combinations allows repetition, actually it is the hardest to explain
but we can flatten the problem and change it to linear

Say we can pick 2 scoops out of a 4 ice cream favors,

GreenTea, Charcolate, Vanilla, Mango

Question, why the answer is not 4*4 = 16 ?
because order doesn't matter, if order does matter, you are right
but [Green Tea, Charcolate] and [Charcolate green tea] is exact the same when we dont consider order

we can transform the question and think how to program a robot to do it

1 means pass
0 get the soop

Green Tea, Vanilar, chocolate, Coffee

and the robot arm is poniting at the green tea now, you need to programm it to walk to the coffee.

so there will be always 3 pass moves, and 2 get the scoop moves

so it looks like this

00111
10101
01101
*
*
*
lets do another transformation, label each position from 1 to 5, imaging it is 5 balls

12345
and 0 means take 1 ball out of this 5 balls, how many permutations can i have ? take 2 balls out of these 5 balls, no repetition allowed, and orders doesn't matter.

so it will be (5)!/(5-2)!/2!

we have a formula for that

5!/3!*2! = 10 Combinations.


**Example**:

The Name of __combination__ lock is wrong, it should be permutation lock actually. Because the Passcode order sequence does matter:


**__How to use this mental Model__**:

* Use Basic Combinations & Permutations to Calculate the the avaiable choices/ probabilities.

* Then can combine with other probability model to estimate the chance of desired outcome

















