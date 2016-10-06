---
ID: 182
post_title: Mental Model, Engineering,Break Point
author: Rational POV
post_date: 2016-08-25 01:17:14
post_excerpt: ""
layout: post
permalink: >
  http://www.rationalpov.com/mental-model-engineeringbreak-point/
published: true
---
# Mental Model Name: Break Point

## Discipline: Engineering
## Related Lattice:

## Upstream: [Mathematics, basic arithmetic](http://www.rationalpov.com/mental-modeldiscipline-mathematics-2/)

## Downstream:

Engineering, Backup System
[Liebig's law of the minimum](https://en.wikipedia.org/wiki/Liebig%27s_law_of_the_minimum)

# Introductions

> A fuse interrupts an excessive current so that further damage by overheating or fire is prevented - wikipedia.

![fuse](https://upload.wikimedia.org/wikipedia/commons/2/25/Fuse.jpg)


> In software development, a breakpoint is an intentional stopping or pausing place in a program, put in place for debugging purposes. It is also sometimes simply referred to as a pause. - wiki


> “Somebody once said that in looking for people to hire, you look for three qualities: integrity, intelligence, and energy. And if you don’t have the first, the other two will kill you. You think about it; it’s true. If you hire somebody without [integrity], you really want them to be dumb and lazy.” - Warrent Buffet

[Farnam Street](https://www.farnamstreetblog.com/2016/08/mental-model-multiplicative-systems/) give a very good explaination of the nature of break point -- Multiplicative System.

> What’s 1,506,789 x 9,809 x 5.56 x 0?

> Hopefully you didn’t have to whip out the old TI-84 to solve that one. It’s a zero.

and that zero, is our concept of break points.

Break Point can be understand as Weakest Link in the multicaptive system, it could be place in the system intentionally, such as fuse in electrial circuits, or shar pins in boat propellers.

Example: [Liebig's law of the minimum](https://en.wikipedia.org/wiki/Liebig%27s_law_of_the_minimum)

> This concept was originally applied to plant or crop growth, where it was found that increasing the amount of plentiful nutrients did not increase plant growth. Only by increasing the amount of the limiting nutrient (the one most scarce in relation to "need") was the growth of a plant or crop improved. This principle can be summed up in the aphorism, "The availability of the most abundant nutrient in the soil is only as good as the availability of the least abundant nutrient in the soil." Or, to put it more plainly, "A chain is only as strong as its weakest link."

> Dobenecks[1] used the image of a barrel—often called Liebig's barrel—to explain Liebig's law. Just as the capacity of a barrel with staves of unequal length is limited by the shortest stave, so a plant's growth is limited by the nutrient in shortest supply.

![bucket law](https://upload.wikimedia.org/wikipedia/commons/1/1c/Minimum-Tonne.svg)



the Upstream of this lattice is Basic Arithmetics:

[Farnma Street](https://www.farnamstreetblog.com/2016/08/mental-model-multiplicative-systems/) argues there are two type of system:

* Multiplicative System. the system is a multiple system, and each stage of the system process is a multiplication and thus the system output is govern by the weakest link, or the break points.

System Ouput = Stage1 x Stage 2 x Stage 3 ...

Computuer software, series electrical circuit, human being, is examples of multiplicative system.

Another name for multiplicative system is the Fragile System of Nassim Taleb descripted in his book [Anti Fragile](https://www.amazon.com/Antifragile-Things-That-Disorder-Incerto/dp/0812979680)

Some Example he has given:

> Salaried employment: while it looks safe on the surface (predictable salary every month) it is subject to the catastrophic risk of losing one's job. ie. the breakpoint is the boss, the boss changed his mind, your "job security is gone"

> Debt-fueled economies: debt has no flexibility, so these economies can't stand even a slowdown without risking implosion (cf current situation)

* Additive System.

System Output = Stage 1 + Stage 2 + Stage 3 ...

The Nassim Taleb's term for Additive System is robust or even better, **Anti Fragile**

Nassim Tableb gives all sorts of example in this book. A clerk in a large company is fragile as he has only one source of income. A taxi driver is antifragile. A banker is fragile. A prostitute is antifragile. General Petraeus is fragile: a single indiscretion was enough to destroy his career. Boris Johnson is antifragile: a whole string of scandals has actually enhanced his reputation.


Most Real Life System is a hybrid of two systems;


# How to use this mental Model:

## Conditions:

Analyze the Systems critical path, is it multiplicative system or additive system by nature ?

if the system is a multiplicative one, enlarge the input by 10x or 100x and try to find out where it will break. thats the break point.


## Predictions:

The System output is govern by its breakpoint, thus simplies the system


## Examples:

___
* [ExampleL Pilot light](https://www.reddit.com/r/engineering/comments/4c2te0/what_is_a_breakpoint/)
> I took a course on materials and a speaker came to talk about his line of work consisting of analyzing failures. He spoke of a manufacturing plant of a certain flammable gas and they have pilot lights all around the plant, so if a gas leak gets large enough one of the pilot lights will ignite the gas cloud and explode. The pilot lights aren't there for IF a gas leak happens,it's there for WHEN it does. The fail safe is a pilot light, without it the gas cloud would get so dense and large that it would be catastrophic otherwise.
