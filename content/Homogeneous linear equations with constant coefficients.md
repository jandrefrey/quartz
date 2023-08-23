---
title: "Homogeneous linear equations with constant coefficients"
---
# Homogeneous linear equations with constant coefficients
These are [[Differential equations]]
$a_ny^n + a_{n-1}y^{n-1}+....+a_0y=0$
where $a_0, a_1... a_n$ are constants

## 2nd order linear homogeneous DE
$ay'' + by' +cy = 0$

### Auxiliary equation
The auxiliary equation is given by:
$am^2 + bm + c= 0$

Then by [[quadratic formula]], we can have 
- 2 real roots
	- $y=c_1e^{m_1x} + c_2e^{m_2x}$
		bc $y_1, y_2$ are [[linear independent]]
- 1 real root
	- $y_1 = e^{mx}$ is a solution, find other solution with [[Reduction of order]]
	- $y=c_1e^{mx} + xc_2e^{mx}$
- 2 complex roots
	- $m = \alpha + \beta i$
	- $y = c_1e^{\alpha x} cos \beta x + c_2e^{\alpha x} sin \beta x$

## Higher order equations
$a_nm^n + a_{n-1}m^{n-1}+....+a_0=0$
- if $m_1$ is a root of multiplicity $k$ then we will have $k$ linearly independant sollutions
	- $y = e^{m_1x}, xe^{m_1x}, x^2e^{m_1x}..., x^{k-1}e^{m_1x}$

## Finding rational roots
![[Pasted image 20220406093757.png]]
![[Pasted image 20220406093822.png]]