---
title: "t-distribution"
---
Used to describe the distribution of the **sample mean** when the population standard deviation is unknown. Notice that t-distribution focuses on the mean of a data set.

> Recall:
> $\mu$ population mean
> $\bar x$ sample mean
> $\sigma$ population standard deviation
> $s$ sample standard deviation

Standard error for $\bar x$: $$SE=\frac{\sigma}{\sqrt n}\approx \frac{s}{\sqrt n}$$
When we have more observations, the degrees of freedom will be larger and the t-distribution will look more like the standard normal distribution
![[Pasted image 20230307195533.png]]
- Always centered at 0
- single parameter: degrees of freedom($df$)
	- $df=n-1$, where $n=$ sample size

## [[Confidence intervals]] for t-distribution
$$\text { point estimate } \pm t_{d f}^{\star} \times S E \quad \rightarrow \quad \bar{x} \pm t_{d f}^{\star} \times \frac{s}{\sqrt{n}}$$

1. Determine SE
2. Find $df$
3. Determine critical t-score ($t_{d f}^{\star}$) using t-table

### Hypothesis Test:
1. Test Statistic: $T_{d f}=\frac{\bar{x}-\mu}{S E}$
	1. ![[t-distribution 2023-03-08 11.38.10.excalidraw]]
2. 
3. 2 or 1 sided? (double area or not)
4. $p<0.05$ Reject $H_0$
---
## Paired Data
Two sets of observations are paired if each observation in one set has a special correspondence or connection with exactly one observation in the other data set. (not independent)
We Subtract the data sets and then use the t-distribution method.

The [[Hypothesis testing]] $H_0$ will assume no difference ($\mu_{diff}=0$).

To visualize the p-value (green area), the sampling distribution of $\bar x$ is drawn as though $H_0$ is true, and the p-value is represented by the shaded tails
	![[t-distribution 2023-03-08 12.11.23.excalidraw]]

---