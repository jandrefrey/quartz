---
title: "Differential equations"
---
# Differential equations
### Linear DE
$a_0(x)y^n + a_0(x)y^{n-1} + a_0(x)y =g(x)$

#### First Order Linear DE
$a_0(x)y' + a_0(x)y =g(x)$

So the standard form is:
$y' + P(x)y = f(x)$

- Integration factor:
$I = e^{\int P(x)dx}$
- So then:
$y=\frac{1}{I} \int{If(x)} dx$


##### Newton's law of cooling
$\frac{dT}{dt} = k(T_a - T)$

...So:
$T=T_a + e^{-kt}C$
there $T_a = T_0$

### Initial Value Problems

^639f12

Sub values for $x$ and $y$ in to find $C$

#### Using [[Laplace Transforms]] to solve IVP.
(for linear DE with constant coefficients)

1. Take $L$ of LH side:
	1. Seperate L linearly
	2. write $L[y, y', y'']$, etc in terms of $L$ using [[Laplace Transforms#^116564|Laplace transforms of derivatives]]
2. Take L of RH side
3. By original eq, $L[LH] = L[RH]$
4. Solve for $L$
6. Solve IVP by computing the [[The inverse Laplace Transform]] of $L(s)$ solved in 4.
	1. So $y=L^{-1}[L(s)]$

__________________________________________________________

## Types of DE:
[[seperable equations]]
[[Exact equations]]
[[Solutions by Substitution]]
[[Theory of linear equations]]
[[Reduction of order]]
[[Homogeneous linear equations with constant coefficients]]
[[Undetermined coefficients & Variation of parameters]]
[[Cauchy-Euler equations]]