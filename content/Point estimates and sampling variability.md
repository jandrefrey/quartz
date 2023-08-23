---
title: "Point estimates and sampling variability"
---

- Parameter($p$): Response from entire population group
- Point Estimate($\hat p$):  Estimate of Parameter from smaller population sample size $n$.
	- Estimate varies between different population samples with **sampling error**

## Central Limit Theorem
When observations are ==independent== and the sample size is sufficiently large(called the success-failure condition: $n p \geq 10$ and $n(1-p) \geq 10$), the sample proportion $\hat{p}$ will tend to follow a normal distribution with the following mean and standard error:
$$
\mu_{\hat{p}}=p \quad S E_{\hat{p}}=\sqrt{\frac{p(1-p)}{n}}
$$
In real world problems we will use substitution approximation $\hat p$ instead of $p$ to calculate these.

- When the sample size increases we would expect the sampling variability to decrease.
- When either $np$ or $n(1 - p)$ is small, the distribution is more discrete, i.e. not continuous.
- When $np$ or $n(1 - p)$ is smaller than 10, the skew in the distribution is more noteworthy.
- The larger both $np$ and $n(1-p)$, the more normal the distribution. This may be a little harder to see for the larger sample size in these plots as the variability also becomes much smaller.
- When $np$ and $n(1 -p)$ are both very large, the distribution's discreteness is hardly evident, and the distribution looks much more like a normal distribution.