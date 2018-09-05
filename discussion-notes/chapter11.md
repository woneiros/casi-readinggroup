# CASI Chapter 11 Notes
## 11.1 Neyman's Construction
### Pivotal construction
### Transformation invariance
## 11.2 Percentile Method
This uses the bootstrap samples' empirical CDF to define a quantile function. 
### Bootstrap sample count
To use the simple percentile method, we need to have confidence that there really is not bias to correct for. This is why I think the authors justify $B=2000$ by estimating the standard error of $p_0$.

$$z_0 = \Phi^{-1}(p_0)$$

Recall that

$$\frac{d}{dx}\,f^{-1}(x) = \frac{1}{f'\left(f^{-1}(x)\right)}$$

so

$$ \frac{dz}{dp}  = \frac{1}{\Phi'\left(\Phi^{-1}(p_0)\right)}
 = \frac{1}{\phi(z_0)}$$

 Given $\tau = g(\theta)$, the delta method approximation is 

 $$\mathbf{se}(\tau) =|g'(\theta)|\,\mathbf{se}(\theta)$$

Estimating everything,

 $$\mathbf{\widehat{se}}(\hat\tau) =|g'(\hat\theta)|\,\mathbf{\widehat{se}}
(\hat\theta)$$

Bringing this back to $z_0$, they seem to use the binomial standard error, yielding

 $$\mathbf{\widehat{se}}(z_0)  = \frac{1}{\phi(z_0)}\sqrt{\frac{p_0(1-p_0)}{B}}$$

Evaluating this for the unbiasedness assumption of $p_0=0.5$, the standard error is approximately

 $$\sqrt{\frac{\pi}{2B}} \approx 0.028$$

 as calculated in the chapter notes.
## 11.3 Bias-Corrected Confidence Intervals
### BC
### BCa
#### Estimating $a$
## 11.4 Second-order Accuracy
## 11.5 Bootstrap-t Intervals
## 11.6 Objective Bayes Intervals and the Confidence Distribution
### Objective Bayes intervals
### Confidence distribution
$$\hat\theta_\mathbf{x}[\alpha] : [0.1]\to \Theta$$
$$\alpha = \mathrm{Pr}\left\{\theta \leq \hat\theta_\mathbf{x}[\alpha]\right\}$$
$$\tilde{g} = \frac{d\alpha}{d\theta}$$
The confidence density is the posterior density of *every* matching prior.

We can approximate it by differentiating smoothed empirical CDF (percentile method) or a reweighting of this based on $p_0$ and $a$ for BC and BCa, respectively.
### What is a credible interval, and how does it differ from a confidence interval?

<!--stackedit_data:
eyJoaXN0b3J5IjpbNTE0MTE4ODA3LDg2MzI1NjI2NV19
-->