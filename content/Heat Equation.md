---
title: "Heat Equation"
---
Given:
$$
\begin{aligned}
k \frac{\delta^2 u}{\delta x^2}=\frac{\delta u}{\delta t}, & & 0<x<L, \quad t>0 \\
u(0, t) &=0 \\
u(L, t) &=0 \\
u(x, 0) &=0
\end{aligned}
$$
where u is the temperature in a rod, 
x is the distance along the rond
and t is the time in seconds.


$$
u(x, t)=\sum_{n=1}^{\infty} A_n \cdot e^{-k\left(\frac{n^2 \pi^2}{L^2}\right) t} \cdot \sin \left(\frac{n \pi}{L} x\right)
$$
where 
$$\boldsymbol{A}_{\boldsymbol{n}}=\frac{2}{L} \int_0^L f(x) \cdot \sin \left(\frac{n \pi}{L} x\right) d x$$

k is the given constant
f(x) is u(x,0)
L is length of x


![[Pasted image 20221128122025.png]]
![[Pasted image 20221128122038.png]]

