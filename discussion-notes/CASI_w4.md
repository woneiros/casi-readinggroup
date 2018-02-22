
# CASI Meetup - Week 4
_Feb 21th, 2018_

__DISCUSSING__:
  - Chapter 8 - Generalized Linear Models and Regression Trees
  - Chapter 9 - Survival Analysis


## Chapter 8
 - Interpretation of coefficients in a logistic regression are dependent on where we are in the probability curve

- working through equation 8.9 

 - Divergence metrics: not symmetrical D(f1, f2) != D(f2, f1) typically:  This link may help? https://wiseodd.github.io/techblog/2016/12/21/forward-reverse-kl/ 

- can we also be explicit about the sufficient statistic for each model; 
    - a sufficient statistic fully parameterizes the a distribution (i.e. for a normal its the mean and the standard deviation)
     - The sufficient statistics of the GLM model can be calculated by a linear model: this ties together the GLM family



## Chapter 9

### Motivation

Insurance company - calculate total cost of estimated lifetime...
TO ADD..


### Survival function, CDF and hazard rate
TO ADD..

### Coin flip example
TO ADD..


### Kaplan-Meier: Estimation of the Survival function
TO ADD..

Kaplan-Meier: https://en.wikipedia.org/wiki/Kaplan%E2%80%93Meier_estimator


### Log-rank for comparing to samples
TO ADD..


### Proportional hazards

### Real-life example: Mortgage prepayment with proportional hazards + gompertz function
Gompertz: https://en.wikipedia.org/wiki/Gompertz_function
 - a generalized logistic function that allows you to model different portions of the probability  (level, slope and curvature)

R Implementations: 
https://cran.r-project.org/web/views/Survival.html

Python implementation:
Lifelines -- docs: http://lifelines.readthedocs.io/en/latest/
