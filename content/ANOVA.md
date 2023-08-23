---
title: "ANOVA"
---
ANOVA uses a single hypothesis test to check whether the means across many groups are equal.
## Sum of squares total
measures **total variability** in the response variable
$$S S T=\sum_{i=1}^n\left(y_i-\bar{y}\right)^2$$
$y_i$ :value of the response variable for each observation 
$\bar{y}:$ grand mean of the response variable

## Sum of squares group
Measures variability **between groups**:
$$S S G=\sum_{j=1}^k n_j\left(\bar{y}_j-\bar{y}\right)^2$$
$n_j$ : number of observations in group $j$
$\bar{y}_j$ : mean of the response variable for group $j$
$\bar{y}:$ grand mean of the response variable

## Sum of squares error
Measures variability **within groups**
$$SSE=SST-SSG$$

----
- Degrees of freedom associated with ANOVA:
	- total: $\quad d f_T=n-1$
	- group: $d f_G=k-1$
	- error: $d f_E=d f_T-d f_G$

- Mean squares: Average variability between and within groups, calculated as the total variability (sum of squares) scaled by the associated degrees of freedom.
	- group: $M S G=S S G / d f_G$
	- error: $M S E=S S E / d f_E$

- F statistic: Ratio of the average between group and within group variabilities:
$$
F=\frac{M S G}{M S E}
$$

the p-value in the case is the probability of at least as large a ratio between the "between" and "within" group variabilities if in fact the means of all groups are equal. (area under F curve.)
![[ANOVA 2023-03-08 13.25.44.excalidraw]]

## Conditions for ANOVA
1. **Independence**:
	1. within groups: sampled observations must be independent
		1. random sample / assignment
		2. each $n_j$ less than $10 \%$ of respective population
		3. always important, but sometimes difficult to check
	2. between groups: the groups must be independent of each other (non-paired)
2. Approximate **normality**: distributions should be nearly normal within each group
	1. check especially when sample size is small
3. **Equal variance**: groups should have roughly equal variability
	1. Variability should be constant across groups (homoscedastic groups)
	2. important when sample size differ between groups.

## Multiple comparisons
doing multiple tests inflates Type 1 error rate, which is undesirable. Then we use modified significance level.(Bonferroni correction)
- Bonferroni correction:
$$
\alpha^{\star}=\alpha / K \quad K \text { :number of comparisons, } K=\frac{k(k-1)}{2}
$$

- However, when we use paired data:
	- Standard error for multiple pairwise comparisons:$$
S E=\sqrt{\frac{M S E}{n_1}+\frac{M S E}{n_2}}
$$
