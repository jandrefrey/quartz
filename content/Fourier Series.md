---
title: "Fourier Series"
---
$$
F(x)=\frac{a_0}{2}+\sum_{n=1}^{\infty}\left\{a_n \cdot \cos \left(\frac{n \pi}{p} x\right)+b_n \cdot \sin \left(\frac{n \pi}{p} x\right)\right\}
$$
Where: (usually [[partial integration||integrate by parts here]])
$$
\begin{gathered}
a_0=\frac{1}{p} \int_{-p}^p f(x) d x \\
a_n=\frac{1}{p} \int_{-p}^p f(x) \cdot \cos \left(\frac{n \pi}{p} x\right) d x \\
b_n=\frac{1}{p} \int_{-p}^p f(x) \cdot \sin \left(\frac{n \pi}{p} x\right) d x
\end{gathered}
$$
Most questions will give f(x) and also p in the form of a function boundary.
Note that the integral will only integrate over the p values of each function. (for step wise defined functions.)
$$
\begin{array}{|c|c|}
\hline \text { Function } & \text { Alternative representation } \\
\hline \cos (\boldsymbol{n} \pi) & (-1)^n \\
\hline \sin (n \pi) & 0 \\
\hline \cos \left(\boldsymbol{n} \pi+\frac{\pi}{2}\right) & 0 \\
\hline \sin \left(\boldsymbol{n} \pi+\frac{\boldsymbol{\pi}}{\mathbf{2}}\right) & (-1)^n \\
\hline \cos (\boldsymbol{\pi}(\boldsymbol{n} \pm \mathbf{1})) & -(-1)^n \\
\hline \sin (\boldsymbol{\pi}(\boldsymbol{n} \pm \mathbf{1})) & 0 \\
\hline
\end{array}
$$

## Fourier Sine and Cosine Series
> Recall:
> EVEN if $𝑓(−𝑥)=𝑓(𝑥)$ ==use COS==
> ODD if $𝑓(−𝑥)=−𝑓(𝑥)$  ==use SIN==

$$
\begin{aligned}
&F_C(x)=\frac{a_0}{2}+\sum_{n=1}^{\infty}\left\{a_n \cdot \cos \left(\frac{n \pi}{p} x\right)\right\} \\
&F_S(x)=\sum_{n=1}^{\infty}\left\{b_n \cdot \sin \left(\frac{n \pi}{p} x\right)\right\}
\end{aligned}
$$
Where:
$$
\begin{aligned}
&a_0=\frac{2}{p} \int_0^p f(x) d x \\
&a_n=\frac{2}{p} \int_0^p f(x) \cdot \cos \left(\frac{n \pi}{p} x\right) d x \\
&b_n=\frac{2}{p} \int_0^p f(x) \cdot \sin \left(\frac{n \pi}{p} x\right) d x
\end{aligned}
$$

## Complex Fourier Series
$$
K F(x)=c_0+\sum_{n=-\infty}^{\infty}\left\{c_n \cdot e^{\frac{i n \pi}{p} x}\right\}
$$
Where:
$$
\begin{gathered}
c_0=\frac{1}{2 p} \int_{-p}^p f(x) d x \\
c_n=\frac{1}{2 p} \int_{-p}^p f(x) \cdot e^{-\frac{i n \pi}{p} x} d x
\end{gathered}
$$
$$
\begin{array}{|c|c|}
\hline \text { Function } & \text { Alternative answer } \\
\hline e^{i x} & \cos (x)+i \cdot \sin (x) \\
\hline \boldsymbol{e}^{-i x} & \cos (x)-i \cdot \sin (x) \\
\hline \boldsymbol{e}^{\pm i n \pi} & (-1)^{\pm n} \\
\hline \boldsymbol{e}^{\pm 2 i n \pi} & 1 \\
\hline e^{\frac{i n \pi}{2}} & i^n \\
\hline e^{\frac{i n \pi}{2}} & i^n \\
\hline
\end{array}
$$

a complex fourier series converges to f(x) at a point of continuity and to the average at a point of discontinuity:
$$\frac{f(x+)+f(x-)}{2}$$