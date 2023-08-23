---
title: "Linear Regression"
---
- We can model a data set with a linear line $\hat y=\beta_0  + \beta_1 x$ if and only if:
	- The data shows a **linear** trend
	- Nearly Normal
	- The variability around the least squares line remains relatively constant.
	

- **Correlation** describes the slope of the data. (if it is linear)
	- Note that a relationship that is nonlinear is simply called an association.
	- correlation coefficient ($r$, also called Pearson’s $r$)
- **Residual**($e$): Leftover after model fit:
	- $Data=Fit+Residual$
	- $Variation(R^2) = r^2$
		- For a good model, we would like this number to be as close to 100% as possible.
	- Outliers can be influential or not influential
		- high leverage points fall horizontally far from data


$$b_1=\frac{s_y}{s_x} R$$
where $R$ is the correlations coefficient, $s_x$ the standard deviation of the explanatory variable, and $s_y$ the standard deviation of the response variable.
$$(\bar x, \bar y) \text{ lies on the line}$$
where $\bar x$ and $\bar y$ is the sample mean of the explanatory and response variables respectively.
And then:
$$y-\bar y = b_1(x-\bar x)$$

We can apply [[Hypothesis testing]] with positive/negative slope with $b_1$.
Here the [[t-distribution]] t-score becomes: 
$$T_{d f}=\frac{b_1-\text { null value }}{S E_{b_1}}$$
with $d_f=n-2$ since we lose one degree of freedom for each parameter we estimate, and in this case we estimate the intercept and the slope.

And the [[Confidence intervals]] becomes
$$b_1 \pm t_{d f}^{\star} S E_{b_1}$$