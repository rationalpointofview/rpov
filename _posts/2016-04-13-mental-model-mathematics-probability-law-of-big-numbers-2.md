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
**Mental Model Name:** 

**Law of big numbers** 

**Discipline: Mathematics** 

Introductions

Law of large numbers, it has many synonyms, but probably you dont know it.

* revert to the mean
* widsom of crowds

![law of large numbers](https://upload.wikimedia.org/wikipedia/commons/0/02/Law_of_large_numbers_%28blow_up%29.gif)

**How to use this mental Model**:

Useful to Predict how the mean will behave when you do a large number of trials of same thing/same experiment.

**Two Conditions:**

*   The result must be come out of same thing/same process
*   The number of trial should be large. How large a number we should call it large ? A Common Pracitice in statistic is the magic number 30. Anything over 30 (times) is considered as large.
*   The trial must be independent

**Predictions:**

The average of the large number should close to the true mean of the group.

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

[Example Noise Cancellation](http://people.math.gatech.edu/~ecroot/3215/central_limit_apps.pdf)

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

![average](https://dl.dropboxusercontent.com/spa/8a95omz6xkznrmw/x51fqq9-.png)

At any rate, if we assume that the Yi are all independent normal random variables, then we don’t even need the central limit theorem, because in that case we have that X − S is exactly N(0, σ2/100).

By just summing the signal average from 100 towers, we can perform a noisse cancellation and increate the Signal to noise ration by 100 fold !


 [1]: http://archive.fortune.com/magazines/fortune/fortune_archive/2001/12/10/314691/index.htm
 [2]: http://static4.businessinsider.com/image/56336b28bd86ef18008c5f4f-907-659/screen%20shot%202015-10-30%20at%209.05.08%20am.png