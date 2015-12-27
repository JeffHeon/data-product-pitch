Central Limit Theorem App Pitch
========================================================
author: Jean-François Héon
date: December 26th, 2015

Central Limit Theorem?
========================================================

The [central limit theorem](https://en.wikipedia.org/wiki/Central_limit_theorem)  according to wikipedia:
> In probability theory, the central limit theorem (CLT) states that, given certain conditions, the arithmetic mean of a sufficiently large number of iterates of independent random variables, each with a well-defined expected value and well-defined variance, will be approximately normally distributed, regardless of the underlying distribution

Wait, what?
========================================================
The central limit theorem tells us that under the right conditions, the distribution of sampling of a distribution is normal, even though the original distribution might not be.

That's a bit abstract, so you can use our Shiny App to experiment with an exponential distribution, which does not have a normal distribution. Additionnaly, you can experiment with samplings of exponential distributions. The next two slides will show you how you could use code to explore the concept, but it's really easier to just use the app!

An exploration example - Code
========================================================

Let's have a look at what you would normally have to write in order to explore the central limit theorem via exponential distributions.

Let's get the distribution of 1000 averages of exponentials of 40 observations with rate .2.

```r
averages = NULL
for (i in 1 : 1000) averages = c(averages, mean(rexp(40,.2)))
```


An exploration example - Plot
========================================================
Here, we will display an histogram of the means distribution. Additionnaly, we will calculate the mean of the means and mark it with a vertical line on the plot. Well, isn't that tedious? use the app!

![plot of chunk unnamed-chunk-2](ctl-pitch-figure/unnamed-chunk-2-1.png) 
