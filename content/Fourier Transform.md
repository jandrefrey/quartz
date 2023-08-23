---
title: "Fourier Transform"
---
Fourier Transform is the proses or function that is is used to convert signals from the time domain to the frequency domain.

$$
F\{f(x)\}=\int_{-\infty}^{\infty} f(x) \cdot e^{i \alpha x} d x=F(\alpha)
$$

> Recall
> $e^{i \alpha x}=\cos (\alpha x)+i \cdot \sin (\alpha x)$


The Inverse Fourier Transform
$$
\mathrm{F}^{-1}\{\boldsymbol{F}(\boldsymbol{\alpha})\}
$$
$$
=\frac{1}{2 \pi} \int_{-\infty}^{\infty} F(\alpha) \cdot e^{-i \alpha x} d \alpha=f(x)
$$
The Fourier Cos Transform
$$
\mathrm{F}_c\{F(\alpha)\}
$$
$$
=\int_0^{\infty} f(x) \cdot \cos (\alpha x) d x=F(\alpha)
$$
The Fourier Sin Transform
$$
\mathrm{F}_s\{F(\alpha)\}
$$
$$
=\int_0^{\infty} f(x) \cdot \sin (\alpha x) d x=F(\alpha)
$$
The Inverse Fourier Sin Transform
$$
\mathcal{F}_s^{-1}\{F(\alpha)\}
$$
$$
=\frac{2}{\pi} \int_0^{\infty} F(\alpha) \cdot \cos (\alpha x) d \alpha=f(x)
$$
The Inverse Fourier Cos Transform
$$
\mathcal{F}_c^{-1}\{F(\alpha)\}
$$
$$
=\frac{2}{\pi} \int_0^{\infty} F(\alpha) \cdot \sin (\alpha x) d \alpha=f(x)
$$
Which Transform to use when:
![[Pasted image 20221128174303.png]]
![[Pasted image 20221201232742.png]]
![[Pasted image 20221201232751.png]]
![[Pasted image 20221201232759.png]]
### Solving PDE with Fourier transform
![[Pasted image 20221128125930.png]]
![[Pasted image 20221128125950.png|700]]
![[Pasted image 20221128130026.png]]




![[1478128033.pdf]]