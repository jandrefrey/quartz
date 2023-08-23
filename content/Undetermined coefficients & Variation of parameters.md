---
title: "Undetermined coefficients & Variation of parameters"
---
# Undetermined coefficients & Variation of parameters
These are [[Differential equations]] of the form:
$a_ny^n + a_{n-1}y^{n-1}+....+a_0y=g(x)$

Notice how the left side looks like [[Homogeneous linear equations with constant coefficients]]
So the solution can be written as $y=y_{complementary} + y_{particular}$
> This method applies when $g(x)$ is a sum of products of the basic functions
> $e^{\alpha x}, sin(\beta x), cos(\beta x), polynomials$

1. Find the complementary function $y_c$ for the homogeneous part (LHS) with [[Homogeneous linear equations with constant coefficients]]
2. Suppose that $y_p$ is formed from a linear combination of derivatives of $g(x)$. So we can write y(p) in a form similar to g(x)
	1. then we can derive this "y" to the (n) times and write the LHS in terms of this "y" and its derivatives.
		![[Pasted image 20220525093608.png|300]]
	1. Simply to find y. This will be the solution to $y_p$
3. $y=y_c+y_p$

## Multiplication rule
Write $g(x)$ as $g(x) = g_1(x) +...+g_m(x)$
	where $g_1(x) +...+g_m(x)$ have no common derivatives and then check what would be a particular solution $y_i$ of the DE $a_ny^n + a_{n-1}y^{n-1}+....+a_0y=g_i(x)$ be.
	Then for each y_i, if y_c and y_i have terms in common, then we multiply y_i by x^k so that  x^ky_i has no terms in common with  y_c and k is as small as possible.

Not really sure what's going on here tbh


## variation of parameters
This solves the same problem as Undetermined coefficients, but here g is not limited to $e^{\alpha x}, sin(\beta x), cos(\beta x), polynomials$, but can be anything.
![[Pasted image 20220525102624.png]]
(we have to integrate $u_1'$ to find $u_1$)
