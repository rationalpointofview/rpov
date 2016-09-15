---
ID: 55
post_title: >
  Mental Model, Mathematics, Probability,
  Law of big numbers
author: Rational POV
post_date: 2016-04-13 00:56:16
post_excerpt: ""
layout: post
permalink: >
  http://www.rationalpov.com/mental-model-mathematics-probability-law-of-big-numbers-2/
published: true
---
#Mental Model: Law of big numbers

## Discipline: Mathematics 

### Introductions

Law of large numbers, it has many synonyms, but probably you dont know it.

* revert to the mean
* widsom of crowds

![law of large numbers](https://upload.wikimedia.org/wikipedia/commons/0/02/Law_of_large_numbers_%28blow_up%29.gif)

#### How to use this mental Model**:

Useful to Predict how the mean will behave when you do a large number of trials of same thing/same experiment.

**Conditions:**

*   The result must be come out of same thing/same process
*   The number of trial should be large. How large a number we should call it large ? A Common Pracitice in statistic is the magic number 30. Anything over 30 (times) is considered as large.
*   The trial must be independent


**Predictions:**

The average of the large number should close to the true mean of the group.




### Up Stream Lattice
None

### Down Stream Lattice

#### Wisdom of the Crowd

In his [book wisdom of the crowds](https://www.amazon.com/Wisdom-Crowds-James-Surowiecki/dp/0385721706), james highlighted four elements required to form a wise crowd:

Criteria  |  Description
---|---
Diversity of opinion  |  Each person should have private information even if it's just an eccentric interpretation of the known facts.
Independence  |  People's opinions aren't determined by the opinions of those around them.
Decentralization |   People are able to specialize and draw on local knowledge.
Aggregation | Some mechanism exists for turning private judgments into a collective decision.


the four elements requred to form a wise crowds is also the conditions for law of large numbers to work.

By using the following example we can better illustrates how widsom of the crowds is a special form of the law of large numbers.

___
[Example Noise Cancellation](http://people.math.gatech.edu/~ecroot/3215/central_limit_apps.pdf)

![noise cancellation](https://upload.wikimedia.org/wikipedia/commons/thumb/7/7d/Active_Noise_Reduction.svg/2000px-Active_Noise_Reduction.svg.png)

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

___

The first condition from critiera for wise crowd to work:
> Each person should have private information even if it's just an eccentric interpretation of the known facts.

We could think of each person is the signal received by different cell towers, and his/her opinion can be split into two parts:

sign and noise.

By the law of large numbers, the signal will add up and noice will cancel each other, thus the crowd opinion is actually the sum of the crowds intelligence.



![average](https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/x51fqq9-.png)

At any rate, if we assume that the Yi are all independent normal random variables, then we don’t even need the central limit theorem, because in that case we have that X − S is exactly N(0, σ2/100).

By just summing the signal average from 100 towers, we can perform a noisse cancellation and increate the Signal to noise ration by 100 fold !


#### Revert to the mean

### Peer Lattice:




___
Examples:

The whole term life insurance industry is based on law of large number, so the larger the subscriber to a policy, the mean life expectacy of the subscripber will be approaching to the group mean, and better the predictability.

Examples:

Warrent Buffet talks about how he come up with the the [single best measures to value the stock market][1] as a whole.

Single stock and short term market is not predictable, but by using law of large numbers, stock market trends can be predicted to some extend.

> On a macro basis, quantification doesn't have to be complicated at all. Below is a chart, starting almost 80 years ago and really quite fundamental in what it says. The chart shows the market value of all publicly traded securities as a percentage of the country's business--that is, as a percentage of GNP. The ratio has certain limitations in telling you what you need to know. Still, it is probably the best single measure of where valuations stand at any given moment. And as you can see, nearly two years ago the ratio rose to an unprecedented level. That should have been a very strong warning signal.
> 
> For investors to gain wealth at a rate that exceeds the growth of U.S. business, the percentage relationship line on the chart must keep going up and up. If GNP is going to grow 5% a year and you want market values to go up 10%, then you need to have the line go straight off the top of the chart. That won't happen.

Later is becomes Buffett indicator:

![Buffet Indicator][2]

source and attribtion:http://www.businessinsider.com/buffett-indicator-better-but-not-great-2015-10


___



 [1]: http://archive.fortune.com/magazines/fortune/fortune_archive/2001/12/10/314691/index.htm
 [2]: http://static4.businessinsider.com/image/56336b28bd86ef18008c5f4f-907-659/screen%20shot%202015-10-30%20at%209.05.08%20am.png