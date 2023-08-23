---
title: "The inverse Laplace Transform"
---
# The Inverse [[Laplace Transforms]]
Given $F(s)$, find $f(t)$ such that $L[f(t)] = F(s)$
If this is true, then $f(t)$ is unique and $f(t) = L^{-1}[F(s)]$

- If $L[f(t)] = L[g(t)] \rightarrow f(t) =g(t)$

==(insert graph)==
 - $L[y]=L \iff y=L^{-1}[L]$

The inverse Lapace transform is linear
- $L^{-1}[\alpha F(s) + \beta G(s)] = \alpha L^{-1}[F(s)] +\beta L^{-1}[G(s)]$

## A few cases:
- $L^{-1}[1] = \frac 1 s$
- $L^{-1}[t^n] = \frac{n!}{s^{n+1}}$
- $L^{-1}[e^{\alpha t}] = \frac{1}{s-\alpha}$
- $L^{-1}[t^n e^{\alpha t}] = \frac{n!}{(s-\alpha)^{n+1}}$
- $L^{-1}[sin(kt)] = \frac{k}{s^2+k^2}$
- $L^{-1}[cos(kt)] = \frac{s}{s^2+k^2}$

## Solving problems
Get the problem in the form of given cases.
Use linearity to take out constants and sums of functions.
If we have a product of functions, decompose using [[Partial fractions]], then use linearity.
