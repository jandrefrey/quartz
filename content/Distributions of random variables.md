---
title: "Distributions of random variables"
---
## Normal Distribution
Symmetric, unimodal, bell curve.

If a normal distribution has **mean $\mu$** and **standard deviation $\sigma$**, we may write the distribution
as N($\mu$; $\sigma$). The normal distribution model can be adjusted with mean(left/right) and standard deviation(stretch/constrain). the standard normal distribution is N(0; 1)
### Z-Score
Used to standardise scale. The Z-score of an observation is defined as the number of standard deviations it falls above or below the mean.
$$Z=\frac{x-\mu}{\sigma}$$
## Geometric Distribution
### Bernoulli distribution
If $X$ is a random variable that takes value 1 with probability of success $p$ and 0 with probability $1-p$, then $X$ is a Bernoulli random variable with mean 
$$
\mu=p
$$
and standard deviation
$$
\sigma=\sqrt{p(1-p)}
$$
### Geometric Distribution
The geometric distribution is used to describe how many trials it takes to observe a success.
If the probability of a success in one trial is $p$ and the probability of a failure is $1-p$, then the probability of finding the first success in the $n^{t h}$ trial is given by
$$
(1-p)^{n-1} p
$$
The mean (i.e. expected value),
$$
\mu=\frac{1}{p}
$$
variance,
$$
\sigma^2=\frac{1-p}{p^2}
$$
and standard deviation
$$
\sigma=\sqrt{\frac{1-p}{p^2}}
$$

## Binomial Distribution
Describe the number of successes in a fixed number of trials.

Suppose the probability of a single trial being a success is $p$. Then the probability of observing exactly $k$ successes in $n$ independent trials is given by
$$
\left(\begin{array}{l}
n \\
k
\end{array}\right) p^k(1-p)^{n-k}=\frac{n !}{k !(n-k) !} p^k(1-p)^{n-k}
$$
The mean,

$$
\mu=n p
$$
variance, 
$$
\sigma^2=n p(1-p)
$$
and standard deviation
$$
\sigma=\sqrt{n p(1-p)}
$$

> CHECK FOR BINOMIAL
> 1. Trials are Independent
> 2. Number of trials, n, is fixed
> 3. Each trial outcome can be classified as success or failure.
> 4. Probability of a success, p, is the same for each trial.

For large sample size (n), this is inefficient. 
We can use the **normal distribution** as an approximation:

The binomial distribution with probability of success $p$ is nearly normal when the sample size $n$ is sufficiently large that $n p$ and $n(1-p)$ are both at least 10 . The approximate normal distribution has parameters corresponding to the mean 
$$
\mu=n p
$$
and standard deviation of the binomial distribution:
$$
\sigma=\sqrt{n p(1-p)}
$$
The normal approximation to the binomial distribution tends to perform poorly when estimating the probability of a small range of counts, even when the conditions are met.
The normal approximation to the binomial distribution for intervals of values is usually improved if cut-off values are modified slightly. The cut-off values for the lower end of a shaded region should be reduced by 0.5, and the cut-off value for the upper end should be increased by 0.5.