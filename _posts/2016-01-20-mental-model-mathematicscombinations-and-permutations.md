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

If each time you choose from different groups, thats the easiest, you just multple the avalible choices together

for scenario of Permutations choose from same group of choices:

There are two types of Permutations;

* One Allows Repetition, (Like the Combination Lock on your suitcase)

you got to pick 3 numbers from 0  - 9, and you can pick the same number.

When allows repetitions, we dont take aways the choices, so we just multiply the number of choice all toghether


**N^**

* One Doesn't Allow Repetitions.

When doesn't allows repetitions, after we choose one , next time there will be one less to choose from:

So First time you will got 0-9 to choose from, after choosen said number 9,  next time you can only choose 0-8.

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

**Combination and Groups**

In real life, often your choice will be partition in Groups.

Say you need to create a password consist only two digits.

Say first digit you need to pick one number from group 0-9

Second digit pick one Alphabet from A-Z

How many Combination will you have ?

The Solution, split this into two steps

* Calculate the avaliable combination choice from each group
    - In this exmample, first group you got 10 choice( Using the Combination allows repetition formular, 10!/(10-1)!/1! = 10, second you got 26 choice
    (26!/(26-1)!/1!)

    - Second step, you need to calculate how many **permutations** when combining these two groups.

    Why **Permutations** ? because these two group is different, so order do matter in step 2,  so by using Permuation formular, you got 10*26= 260 



**__How to use this mental Model__**:

* Use Basic Combinations & Permutations to Calculate the the avaiable choices/ probabilities.

* Then can combine with other probability model to estimate the chance of desired outcome

**Example**:

You forgot about passcode on your 3 digit combination lock of your suitcase,
you think probably you can try one code for 5 sec, then how many times does it take to unlock your suitecase ?

First of all, you will notice the Name of __combination__ lock is wrong, it should be __permutation__ lock actually. Because the Passcode order sequence does matter:

and the code allows repetition, so the use the formular N^r

and N = 10, r = 3

so you got 1000 permuation of code to try, and each try takes 5 secs, so approximately it will take 5000 secs, and thats about One and Half Hours, so actually it is not that bad.


**Examples:**

A New Pizza Shop can allow you to create pizzas of your own choice by choosing Crust, Topping and Cheese, How Many Difference type Pizza can you make ?

4 types of toppings - pepperoni, sausage, ham, bacon

3 types of crust -thin, regular,  thick

5 types of cheese - American, cheddar, Swiss, blue cheeze, Home Made.


Answer:

This is combination with group scenario:

So first we calculate the number of avaliable choice for each group:

Topping: 4C1 = 4
Crust: 3C1=3
Cheese:5C1=5

And calculate the permulation of 3 groups, thats 4x3x5= 60 different combinations

**Example:**

A 4 person task force is to be formed from 4 men and 3 women who work in Company G's HR dept. If there are to be 2 men and 2 women, how many different task forcers can be formed? 
A)14 
B)18 
C)35 
D)56 
E)144 

Answer:

This is combination with group scenario:

So first we calculate the number of avaliable choice for each group, as the order of the candidate within the group doesn't matter, we use combination without repetition.

Men: 4C2=6
Women: 3C2= 3

mutiple two number of choice together, you got 18, so you should chooice B


Another excellent choice for this is [Quora[(https://www.quora.com/What-is-the-practical-real-life-use-of-permutation-and-combination)]














