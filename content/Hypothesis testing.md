---
title: "Hypothesis testing"
---
The null hypothesis ($H_0$) often represents a sceptical/conservative perspective.
The alternative hypothesis ($H_A$) represents an alternative claim under consideration and is
often represented by a range of possible parameter values.

A Type 1 Error is rejecting the null hypothesis when H0 is actually true. A Type 2 Error
is failing to reject the null hypothesis when the alternative is actually true.

## Significance level
What percentage of times do we incorrectly reject $H_0$
- Generally $\alpha=0.05$
	- If making a Type 1 Error is dangerous or especially costly, we should choose a small significance level (e.g. 0.01).
	- If a Type 2 Error is relatively more dangerous or much more costly than a Type 1 Error, then we might choose a higher significance level (e.g. 0.10).

## P-value
The p-value is a way of quantifying the strength of the evidence against the null hypothesis
and in favour of the alternative hypothesis.

- Compare to significance level:
	- p-value is less than $\alpha$, reject $H_0$
	 - p-value is greater than $\alpha$, do not reject $H_0$, and report that we do not have sufficient evidence to reject the null hypothesis.

Calculate a p-value as the area under the normal curve beyond the observed sample proportion (either in one tail or both, depending on the alternative hypothesis). Note that in doing so you can use a $\mathrm{Z}$ score, where
$$
Z=\frac{\text { sample statistic }-\text { null value }}{S E}=\frac{\bar{x}-\mu_0}{S E}
$$
SE computed from nul value.

> Hypothesis testing should always be concerned with the population statistics and not the sample statistics, as we already know the sample statistics.