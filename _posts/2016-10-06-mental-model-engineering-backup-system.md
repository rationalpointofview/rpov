---
ID: 262
post_title: Mental Model, Engineering, Backup System
author: Rational POV
post_date: 2016-10-06 00:59:25
post_excerpt: ""
layout: post
permalink: >
  http://www.rationalpov.com/mental-model-engineering-backup-system/
published: true
---
# Mental Model: Backup System


### Discipline: Engineering

### Up Stream Lattice

*   [Break Points][1]

### Down Stream Lattice

### Peer Lattice:

*   [Margin of Safety][2]

## Introductions

What is a Backup System ?

From [Reliability Engineering for Electronic Design](https://www.amazon.com/gp/product/0824775716),

> Websters defines redundancy as needless repetition. In reliability engineering, however, redundancy is defined as the existence of **more than one means for accomplishing a given task**. Thus **all** of these means must fail before there is a system failure.

A Backup System is turning a Multiplicative System with a single break point into an additive system with two or more break points.

When the primary system break point fails, the input can flow through the backup system to the output.

If the primary system is a simple one, backup system is less useful, and can backfire, because added a needless path from input to output increases system complexity.

But if the primary system is a very complex one, and very hard to understand/predict/control it, backup system will provide great values there.

You can see Backup system it in Biological system more than any other discipline.

Samuel Arbesman explains in his book [Overcomplicated: Technology at the Limits of Comprehension](https://www.amazon.com/dp/1591847761/)

He argues Physics system is a simple one, but biology is much more complex system.

>[B]iological systems are generally more complicated than those in physics. In physics, the components are often identical—think of a system of nothing but gas particles, for example, or a single monolithic material, like a diamond. Beyond that, the types of interactions can often be uniform throughout an entire system, such as satellites orbiting a planet.


> In biology, there are a huge number of types of components, such as the diversity of proteins in a cell or the distinct types of tissues within a single creature; when studying, say, the mating behavior of blue whales, marine biologists may have to consider everything from their DNA to the temperature of the oceans. Not only is each component in a biological system distinctive, but it is also a lot harder to disentangle from the whole. For example, you can look at the nucleus of an amoeba and try to understand it on its own, but you generally need the rest of the organism to have a sense of how the nucleus fits into the operation of the amoeba, how it provides the core genetic information involved in the many functions of the entire cell.

Your body is one of the best example of redundancy.

The author of Black Swan and antifragile , NASSIM TALEB  argues;

> she(Mother nature) likes redundancies. Look at the human body. We have two eyes, two lungs, two kidneys, even two brains (with the possible exception of company executives) - and each has more capacity than is needed ordinarily. So redundan­cy equals insurance, and the apparent inefficiencies are associated with the costs of maintain­ing these spare parts and the energy needed to keep them around in spite of their idleness.


## How to use this mental Model:

* Analyze the primary system:

  * Is the primary system a multiplicative one or additive one ?
      If the system if additive, by definition it doesn't need a backup system.

  * if the primary system is a simple or complex one ?
      If the system is a simple one, other means of increasing reliability could be more effective( margin of safety )

* Designing Backup System.  

  if the primary system is a complex and multiplicative one, adding backup system could greatly improve reliability:

      * the backup system path need to be independent of the primary


### Conditions:

### Predictions:

### Examples:




 [1]: http://www.rationalpov.com/mental-model-engineeringbreak-point/
 [2]: https://www.farnamstreetblog.com/2013/12/margin-of-safety/
