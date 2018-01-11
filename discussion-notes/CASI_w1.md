
# CASI Meetup - Week 1
_Jan 10th, 2018_

__DISCUSSING__:
  - Chapter 1 - Algorithms and Inference
  - Chapter 2 - Frequentist Inference
  - Chapter 3 - Bayesian Inference


## Logistics
Meeting every other week to discuss 2 chapters

Everytime someone (alex will define) will briefly present the material read


## Introducion - Are we Bayesian or Frequentist?
- We think in a Bayesian way, but simple questions ma make more sense to try a frequentist 
- We based our knowledge based on our experience -> Our biases have a lot of influence in our decision making
- People don't update as much... Find a time where you really changed your mind about something?


## Philosophical discussion
__FREQUENTIST__ 
Believe in a Truth, a parameter that is true and will always unkowable and unobservable... We are just trying to estimate it, using the data -- Plato's cave

Frequentist components of the world:
 - Truth of parameter (inobservable)
 - Estimates of the parameter
 - Algo or estimator of the parameter

--> The voltometer example, it is impossible to integrate the example problem of the voltometer into the frequentist model of the world

__BAYESIAN__
Truth as a construction (no objectivism - rather )
Bayes rule: Our understanding of the world is constructed based on our prior understanding, the data that we saw, and the probability of seeing what we saw

We are trying to obtain a function on the family of probability of the problem at hand


## Statistical discussion
__FREQUENTIST__
We obtain a series of moments to characterize such function -- we never have the "actual" distribution function.
The true value is unkown but __fixed__.
Concerned with $P(x|\theta)$ - the __probability of observing the sample data__ given the hypothesized parameter.

_Confidence Interval:_  
Cannot be interpreted as a probability, but rather about the repeated experiments.

$P(\theta \in I) = 0.95$

_It is a statement about the interval itself, and not about the paremeter (since it is fixed): if the experiment that generated the random sample x were repeated many times, 95% (or other) of such intervals constructed from those random samples would contain the true value of the parameter_

__BAYESIAN__
We get a series of functions that explain the data our understanding of the world at each moment (based on the data we have observed)
The Bayesian approach assumes that the "true" value is a __random variable__.
Concerned with $P(\theta|x)$ - the __probability of the parameter__ value given the observed sample data.

_Credibility Interval_(Bayesian confidence interval):  
Given our actual belief of the world (the random variable of the true value), we know the uncertainty we have, and we can construct a credibility interval such that:

$P(\l \leq \theta \leq \h]) = 0.95$

_It is a question about the location of the parameter: Our value is 95% likely to be less than the high bound and more than the lower bound_

