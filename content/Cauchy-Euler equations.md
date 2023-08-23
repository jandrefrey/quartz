---
title: "Cauchy-Euler equations"
---
# Cauchy-Euler Equations
These are [[Differential equations]]
Any equation of the form 
$a_nx^ny^n+a_{n-1}x^{n-1}y^{n-1}+...+a_1xy^1 + n_0y=g(x)$
is a CE-equation. These can be homogeneous or non-homogeneous.

##  How to solve the homogenous part
$a_nx^ny^n+...+a_1xy^1 + n_0y=0$

1. ==Try sollution:== $y=x^m$
2. Write derivatives of y in terms of x and m.
3. Sub back into original equation.
4. factor out $x^m$
5. since $x^m$ is non-zero, we know that rest of the equation is = 0
	![[Pasted image 20220404091358.png|250]]
6. Solve for m.
7. The our sllution to the DE is $y=C_1x^{m_1}+C_2x^{m_2}$

## Second order CE equation
$ax^2y''+bxy'+cy=0$
To get the **aux eq.**, make sub $y=x^m$

### 2 distinct real root
If our aux eq has 2 real roots, $m_1, m_2$, then the sollution is 
$y =c_1x^{m_1} + c_2x^{m_2}$ 
since $y_1, y_2$ are linear independant

### Repeated real root
If the Aux eq has a repeated real root m then 
$y = c_1x^m+ c_2ln(x)x^m$ 
since $y_1, y_2$ are linear independant

### Complex root
The aux eq has a complex root $m=\alpha + \beta i$
Then the sollution is 
$y=c_1(x^\alpha(cos(\beta lnx)+isin(\beta lnx)))+c_2(x^\alpha(cos(\beta lnx)-isin(\beta lnx)))$ 
![[Pasted image 20220613204303.png]]
since $y_1, y_2$ are linear independant

## Non-homogeneous Part
Devide through with everything in front of y''.
Then use [[Undetermined coefficients & Variation of parameters|Variation of parameters]]
![[Pasted image 20220525105226.png]]
OR constant coefficients method.
