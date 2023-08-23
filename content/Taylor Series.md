---
title: "Taylor Series"
---
$$\begin{aligned}
&\text { Taylor series }=\sum_{n=0}^{\infty} \frac{f^n(a)}{n !}(x-a)^n\end{aligned}$$
The Maclaurin series replaces *a* with *0*
$$\begin{aligned}&\text { Maclaurin series }=\sum_{n=0}^{\infty} \frac{f^n(0)}{n !}(x)^n
\end{aligned}$$
### Finding the Taylor Series of a function:
1. Draw a table
	1.  n  | $f^n(x)$ |  $f^n(a)$
		------------ | ------------ | --------
		 0 | $f^0(x)$ | $f^0(a)$
		  1 | $f^1(x)$ | $f^2(a)$
		n-value  |n-th derivative| n-th derivative with a

2. From the 3rd column we can write the full formula.

### Some important Taylor functions
$$
\begin{array}{|ccc|}
\hline \text { Function } & \text { Taylor Series } \\
\hline e^{\boldsymbol{x}} & \sum_{n=0}^{\infty} \frac{x^n}{n !} \\
\hline \sin (x) & \sum_{n=0}^{\infty}(-1)^n \cdot \frac{x^{2 n+1}}{(2 n+1) !} \\
\hline \cos (x) & \sum_{n=0}^{\infty}(-1)^n \cdot \frac{x^{2 n}}{(2 n) !} \\
\hline(1-x)^k & \sum_{n=0}^{\infty}\left(\begin{array}{l}
k \\
n
\end{array}\right) \cdot x^n \\
\hline \ln (1+x) & \sum_{n=0}^{\infty}(-1)^{n-1} \cdot \frac{x^n}{n} \\
\hline
\end{array}
$$
$$
\begin{gathered}
\lim _{n \rightarrow \infty} \frac{x^n}{n !}=0 \\
\lim _{n \rightarrow \infty}\left(1+\frac{1}{n}\right)^n=e
\end{gathered}
$$