
# CASI Meetup - Week 1
_Jan 24th, 2018_

__DISCUSSING__:
  - Chapter 4 - 
  - Chapter 5 - 


## Chapter 4 

### MLE
Maximizing for the parameter - Most likely parameter

Where does this fit in the Frequentist (data fixed) vs Bayesian?
 - Although it has good frequentist properties.. but in the end we are actually estimating the parameters of a paremeter (Bayesian world-view)

 - Seems to assume a bayesian framework (with base distribution - _prior_- and then trying to find the best possible _posterior_)

 - Constraint: having to choose the function family


### Fisher Information

Fisher info and Kullback Leibler divergence (shannon)


### Conditional Inference
Follow up with @Alex


### Randomization Inference

@Jlandesman example: Correlations on certain types of days were different days (fake data release vs data release days)


## Chapter 5 - Parametric Models and Exponential Families

Historical motivation:
- reduce the dimension space by only having to search for a series of parameters
- also serves as classification -- similar problems will have similar functions -> same function family

However, now with computers it is not _that_ necessary ... a lot more compute power enables to search in higher dimensional spaces


### Univariate Familier

*Normal*

*Poisson* Number of (indep) events in a fixed interval of time 

*Binomial* 

*Gamma* Closed to chi-sq --> for feature selection

*Beta* Cont in [0,1] a lot of diff shapes
http://varianceexplained.org/statistics/beta_distribution_and_baseball/
--empirical Bayes


### Multivariate Normal Distributions
--> Multi-normal distribs...


### Fisher Information Bound
MLE -- harder and harder to estimate when we have "more" parameters (higher variance)

Could be used as a measure of model parsimony


### Multinomial distrib
For a finite (discrete) number of outcomes

The conditional of a single Poisson, given the sum of all Poissons follows a Multinomial !!

When N is larger, binomial approaches Poisson (N turns into a continuous time interval)... ties up with page 55

Negative binomial (different mean and variance) vs Poisson (mean and variance are the same)


### Exponential Families
The exponential family is a generalization ver the distribution families.

In fact, all the distributions above can be expressed as an instance of the exponential family.  

The exponential family have the following geenral form for a density function:  

p(mu, x) = h(x) exp( h(mu) T(x) - fi(mu) )  

Where T(x) is the sufficient statistic **TO DO**  

 - 


