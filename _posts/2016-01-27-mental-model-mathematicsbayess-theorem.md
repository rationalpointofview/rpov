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

Use it to understand the true implications of test results:


**Conditions:**

The Event A is statistical event.

The Event B is an imperfect ;


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
















