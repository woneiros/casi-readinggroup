# Chapter 6 - Empirical Bayes

## What is Empirical Bayes?

If we have data from observations, we can use it to getter a _better estimate_ of an average.

## How does it work?

Baseball example:

We have data on batting averages for hundreds or thousands of players (or more), by using the average and the variance of the entire 
population we can make a more _informed guess_ of how well a player will performed when we don't have much data for that player.  

Say we know that the overall batting average of all baseball players is 0.254, with a variance of 0.078. When we see a baseball player 
come along with a batting average of 0.500 from 50 hits out of 100 at bats, we know that person is unlikely to maintain that average over 
the long term because nobody does given enough at bats. Using Empirical Bayes, we would estimate that players batting average instead as 

```math
(50 + 78) / (100 + 78 + 254) = 128 / 432 = 0.296
```

This is still a much better batting average than most players (+0.042), yet much lower 
than the current statistic. 

## Pros

Without much effort or complex math, we get a _decent approximation_ of true expected value for outcomes where we don't have sufficient 
data by itself. 

## Cons

As [explained by DRob](http://varianceexplained.org/r/beta_binomial_baseball/)

> But there’s a complication with this approach. When players are better, they are given more chances to bat! 

Empirical Bayes may not perfom well when baseball players are new to the league or when they are much different than average. 
For example, a rookie future hall of famer probably won't have enough at bats to offset the shrinkage towards the average of the 
other players even though they really are exceptional. 
