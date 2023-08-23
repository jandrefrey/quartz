---
title: "Laplace Transforms"
---
# Laplace Transforms
> If a function $f(t)$ is said to be of exponential order if there exists $c>0$  st
$lim_{b \rightarrow \infty} f(t) e^{-cb}=0$

If f(t) is piecewise continuous over $[0, \infty]$ and $f(t)$ is of exp order, then L{f(t)} exists.
Given $f(t)$ defined $0 \leq t$

The Laplace-Transform of $f(t)$ is a function of $s$ defined by
$L[f(t)] = \int_0^\infty e^{-st} f(t) dt$

- Ex:
	- ![[Pasted image 20220404100447.png|250]]
	![[Pasted image 20220404100811.png|250]]
	![[Pasted image 20220404100841.png|100]]

## A few cases
- $L[e^{\alpha t}] = \frac 1 {s-\alpha}  \:\:\:\:\:\:\:\:\:\:\:(\alpha, \infty)$

- $L[1] = \frac 1 s$

- $L[t^n] = \frac{n!}{s^{n+1}}$

- $L[sin (kt)] = \frac{k}{s^2+k^2}$

- $L[cos(kt)] = \frac{s}{s^2+k^2}$

- $L[t] = \frac 1 {s^2}$

## Linearity of Laplace transform
$L[\alpha f(t) + \beta g(t)] = \alpha L[f] + \beta L[g]$


## Transforms of Products of functions
if $f(t)$ is a product of two other functions, use [[partial integration]] (possibly a few times).
(phone photo)

## Transforms of Piecewise defined functions
Given that $f(t)$ is a function defined piecwise over a set of intervals:
Then we can do the Lalpace transform over each interval seperately.
So for $f(t)\rightarrow 0 \leq t<1, \:\: g(t) \rightarrow 1\leq t<\infty$

$\int_0^\infty f(t) e^{-st} dt = \int_0^1 f(t) e^{-st} dt +\int_1^\infty g(t) e^{-st} dt$

## Transforms of derivatives

^116564

Let $f(t)$ be a differential function of exponential order.
$$
\begin{align}
L[f'] &= \int_0^\infty f'(t) e^{-st} dt 
\\ &= sL[f]-f(0)
\end{align}
$$


Given $f(t)$ such that $f, f', f'',..., f^{n-1}$ is of exp order

$L[f^{(n)}] = s^nL[f] - s^{n-1}f(0) - n^{n-2}f'(0)-....-f^{n-1}(0)$
