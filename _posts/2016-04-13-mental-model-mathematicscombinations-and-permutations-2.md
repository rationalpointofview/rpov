---
ID: 53
post_title: >
  Mental Model, Mathematics,Combinations
  and Permutations
author: Rational POV
post_date: 2016-04-13 00:56:16
post_excerpt: ""
layout: post
permalink: >
  http://www.rationalpov.com/mental-model-mathematicscombinations-and-permutations-2/
published: true
---
**Mental Model Name:elementary math of permutations and combinations** **Discipline:Mathematics** **Lattice Rank:4**

> Elementary math of permutations and combinations, It's very simple algebra. It was all worked out in the course of about one year between Pascal and Fermat. They worked it out casually in a series of letters.
> 
> It's not that hard to learn. What is hard is to get so you use it routinely almost everyday of your life. The Fermat/Pascal system is dramatically consonant with the way that the world works. And it's fundamental truth. So you simply have to have the technique. --Charlie Munger

Why Pascal and Fermat work this out ? They work this out for winning money (Gambling), Of Course!

**Conditions:**

discrete number

**Predictions:**

avaliable choice from combination/permutations of factors

**How to use this mental Model:**

can use this to calcualor the avaliable choices in your head

*  Identify if repetition allowed

    * If repetition allowed, use N^r to calculate base permutation
    * If repetition is not allowed, used N! to calculate base permutation

* Revise the number up or down, if needed. 

couple scenarios:

* If results is combination, scale the number down by divide the base permutation by r!

    
* If there is multiple group combination, multiple the base permuations.


**What is Combinations and Permutations**:

When the order doesn't matter, it is combinations;

When the order does matter, it is permutations

**Permutatations is the easier one to Explain:**

**The Basic methodology to calculate Permutation is you just mutiple the avaliable choice together**.

If each time you choose from different groups, thats the easiest, you just multple the avalible choices together

for scenario of Permutations choose from same group of choices:

There are two types of Permutations;

*   One Allows Repetition, (Like the Combination Lock on your suitcase)

![Combination Lock](https://c2.staticflickr.com/4/3800/12351110484_1718e441ac_b.jpg)

you got to pick 3 numbers from 0 - 9, and you can pick the same number.

When allows repetitions, we dont take aways the choices, so we just multiply the number of choice all toghether

<img src="http://www.sciweavers.org/tex2img.php?eq=%20N%5E%7Br%7D%20&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0" align="center" border="0" alt=" N^{r} " width="22" height="17" />

*   One Doesn't Allow Repetitions.

When doesn't allows repetitions, after we choose one , next time there will be one less to choose from:

So First time you will got 0-9 to choose from, after choosen said number 9, next time you can only choose 0-8.

then the computations will be (N)(N-1)(N-2)...

So the Formular for Combinations without Repetions is:

**N!**

**Combinations**

**The Basic methodology to calculate Permutation first, then calculate how many ways it can arrange the order, then reduce it to combination**

There are also two types of Combinations:

*   One Doesn't Allows Repetition

Example: Lottery, you pick 7 numbers, the order of this 7 numbers doesn't matter, but you can't pick the same number twice.

we can simplify it as Permutations, then reduce it to combinations

say we want to know the possibilities of picking R balls out of a Pool of N, then

The Permutations = N!/(N-R)!, and remember, how many permutations does R balls has ? R!

the R balls could have a permutations of R! iteself, which we dont quite care and all the same to us now, so reduced the choice by R! number of times,

so Combinations without repetion = Permutations without repetitions / R!

*   One Allows repetition

Combinations allows repetition, actually it is the hardest to explain but we can flatten the problem and change it to linear

Say we can pick 2 scoops out of a 4 ice cream favors,

GreenTea, Charcolate, Vanilla, Mango

Question, why the answer is not 4*4 = 16 ? because order doesn't matter, if order does matter, you are right but [Green Tea, Charcolate] and [Charcolate green tea] is exact the same when we dont consider order

we can transform the question and think how to program a robot to do it

1 means pass 0 get the soop

Green Tea, Vanilar, chocolate, Coffee

and the robot arm is poniting at the green tea now, you need to programm it to walk to the coffee.

so there will be always 3 pass moves, and 2 get the scoop moves

so it looks like this

00111 10101 01101 * * * lets do another transformation, label each position from 1 to 5, imaging it is 5 balls

12345 and 0 means take 1 ball out of this 5 balls, how many permutations can i have ? take 2 balls out of these 5 balls, no repetition allowed, and orders doesn't matter.

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

*   Calculate the avaliable combination choice from each group
    
    *   In this exmample, first group you got 10 choice( Using the Combination allows repetition formular, 10!/(10-1)!/1! = 10, second you got 26 choice (26!/(26-1)!/1!)
    
    *   Second step, you need to calculate how many **permutations** when combining these two groups.
    
    Why **Permutations** ? because these two group is different, so order do matter in step 2, so by using Permuation formular, you got 10*26= 260

**How to use this mental Model**:





**Example**:

You forgot about passcode on your 3 digit combination lock of your suitcase, you think probably you can try one code for 5 sec, then how many times does it take to unlock your suitecase ?

First of all, you will notice the Name of **combination** lock is wrong, it should be **permutation** lock actually. Because the Passcode order sequence does matter:

and the code allows repetition, so the use the formular N^r

and N = 10, r = 3

so you got 1000 permuation of code to try, and each try takes 5 secs, so approximately it will take 5000 secs, and thats about One and Half Hours, so actually it is not that bad.

**Examples:**

A New Pizza Shop can allow you to create pizzas of your own choice by choosing Crust, Topping and Cheese, How Many Difference type Pizza can you make ?

4 types of toppings - pepperoni, sausage, ham, bacon

3 types of crust -thin, regular, thick

5 types of cheese - American, cheddar, Swiss, blue cheeze, Home Made.

Answer:

This is combination with group scenario:

So first we calculate the number of avaliable choice for each group:

Topping: 4C1 = 4 Crust: 3C1=3 Cheese:5C1=5

And calculate the permulation of 3 groups, thats 4x3x5= 60 different combinations

**Example:**

A 4 person task force is to be formed from 4 men and 3 women who work in Company G's HR dept. If there are to be 2 men and 2 women, how many different task forcers can be formed? A)14 B)18 C)35 D)56 E)144

Answer:

This is combination with group scenario:

So first we calculate the number of avaliable choice for each group, as the order of the candidate within the group doesn't matter, we use combination without repetition.

Men: 4C2=6 Women: 3C2= 3

mutiple two number of choice together, you got 18, so you should chooice B

Another excellent choice for this is [Quora][1]]

**Example:**

Case 1 : You have a date with your girlfriend. And, you want a perfect combination of shirt and pant. Suppose, you have 2 shirts (White and Blue) and 2 pants (Black and Brown). So, how many combinations do you have?

This is a Grouped Combinations and you calculate how many possible combinations from each groups

shirts = 2C1 = 2!/1!= 2 pants = 2C1 = 2

so the possible combinations = 2 x 2 = 4

**Example:**

![How many ways you can personalize wendy's hamburger][2]

[Walkinginmathland][3] give an interesting application for combinations and how Wendy's marketing department got it wrong.:

> The bag my food was in (picture above) had the following phrase: "We figured out that there are 256 ways to personalize a Wendy's hamburger. Luckily someone was paying attention in math class."

is that correct ? Hint: Wendys hamburger has 9 different topping to choose from at the time.

so it is a combinations doesn't allow repetion problem. The trick is, you can pick 0-9 topping from all the avaliable toppings.

9C0 = 1 9C1 = 9 9C2 = 36 9C3 = 84 9C4 = 126 9C5 = 126 9C6 = 84 9C7 = 36 9C8 = 9 9C9 = 1

Total: 512 ways to personalize a Wendy's hamburger

**Example**

[StackOverflow][4] has a permutation & combinations interview problem:

> Imagine an urn filled with balls, two-thirds of which are of one color and one-third of which are of another. One individual has drawn 5 balls from the urn and found that 4 are red and 1 is white. Another individual has drawn 20 balls and found that 12 are red and 8 are white. Which of the two individuals should feel more confident that the urn contains two-thirds red balls and one-third white balls, rather than vice-versa? What odds should each individual give?
> 

**[Example](http://www.mathwarehouse.com/probability/combination.php)**

> Over the weekend, your family is going on vacation, and your mom is letting you bring your favorite video game console as well as five of your games. How many ways can you choose the five games if you have 12 games in all?


>12C5 = (12)!/(5!×(12-5)!)=(12)!/(5!×(7)!) 
(12×11×10×9×8×7!) /(5!×7!) = 792

**[Example](https://www.cs.sfu.ca/~ggbaker/zju/math/perm-comb-more.html)**

> Example: How many ways are there to permute the letters of the word HAPPY?

* Note there are two Ps, so it is sort of permutation/combination hybrid

let follow the steps:

1. Is repetition allowed ?

No, so use N! formula, 5!=120

2. reduce to combination.
Since PP and PP is the same thing, so reduce to 

120/2! = 60

**[Example single deck or double deck](https://www.cs.sfu.ca/~ggbaker/zju/math/perm-comb-more.html)**

> in a card game with a single deck (no jokers), how many way to order the deck ? and how many for two decks shuffled together ?

single deck

> 1. Is repetition allowed ?

No, so use N! formula, 52!=8.06582E+67

2. combination? no. so 8.06582E+67 is the final anwser

double deck

1. is repetion allowed ?

No. so use N1 formular, 104! =1.0299E+166

2. Combination, reduce to combination

there are two decks and there are 52 pair cards is identical.

so questions is, how many permutations can 52 different pairs of card have ?

permutation of a pairs of card:

=2! = 2

52 independent groups of cards permutation, it is a daisy chain, need to multiple the possible permutations together; 

= 2^52

so total = 2.28684E+150



**[Example](https://www.cs.sfu.ca/~ggbaker/zju/math/perm-comb-more.html)**

> How many ways to order the letters of MISSISSIPPI?
> 

1. is repetition allowed ? No

11! = 39916800

2. reduce to combination

there are 4S, 2P and 4 I

the permutation of each will be 4!, 2!, 4!

= 11!/(4!*2!*4!)

**[Example. Too many gifts](https://www.cs.sfu.ca/~ggbaker/zju/math/perm-comb-more.html)

>Your mother-in-law buys 1000 small gifts to give to relatives for Christmas, for reasons you don't understand. Each of the 1000 things is different, because she spends too much time shopping. There are 25 relatives to give gifts to. How many ways are there to distribute the gifts?
Note: the question allows the possibility of one person getting 1000 things, and everyone else getting nothing. There's no fairness in this family

for 1 gift:

you can give the gift to any of the 25 relatives, so choices:

= 25

for 2 gift:

you can give the gift to any of the 25 relatives, so choices:

= 25

so you can transform the question into this form:

you got to pick 25 relative to give gift too, and pick 1000 times. repetition allowed( since there is no fairness in the family)

25^1000 = 8.7×101397

> In the above scenario, how many ways can the gifts be distributed so each person gets 40 items?


 [1]: https://www.quora.com/What-is-the-practical-real-life-use-of-permutation-and-combination
 [2]: https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/jf-2if5l.png
 [3]: http://walkinginmathland.weebly.com/teaching-math-blog/wendy
 [4]: http://stackoverflow.com/questions/447384/permutation-combinations-interview