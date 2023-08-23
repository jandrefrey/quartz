---
title: "Convergence"
---
$\lim a_n \rightarrow$ exists, then $a_n$ cvgt
$\lim S_n \rightarrow$ exists, then $S_n$ cvgt
$S_n \operatorname{cvg} t \rightarrow \lim a_n=0$
$\lim a_n=0 \rightarrow S_n$ cvgt
$\lim a_n \neq 0$ or does not exist $\rightarrow S_n d v g t$
![[Pasted image 20221127205609.png]]

![[Pasted image 20221123174924.png]]

### Convergence Tests
- [[Integral Test]]
- [[Divergence Test]]
- [[Comparison Test]]
- [[Limit comparison test]]
- [[Alternating series test]]

## Absolute Convergence
$\sum a_n$ Absolutely convergent if $\sum |a_n|$ is convergent.
This test is divided into two subsections, namely:
- [[Ratio Test]]
- [[Root Test]]
When you have finished both these steps during the Ratio test and Root test, use the limit value L:
$$
\text { If } L\left\{\begin{array}{cc}
<1 & \begin{array}{c}
\text { ABSOLUTE CONVERGENT, } \\
\text { and therefore CONVERGENT }
\end{array} \\
\hline=1 & \rightarrow \text { NO RESULT }(n / a) \\
\hline>1 \text { or does not exist } & \rightarrow \text { DIVERGENT }
\end{array}\right.
$$

## Conditional Convergence
The series is seen as convergent, but not absolutely convergent.
[[Ratio Test]] or [[Root Test]] Limit yields 1.


## Radius of convergence of [[Power Series]]
- This is determined by the following equation:
$$
|x-a|
$$
If the series converges for $|x-a|<\Re$
then it diverges for $|x-a|>\Re$
- The interval of convergence is:
$$
[(a-\Re),(a+\Re)]
$$
- Furthermore it is important to note that the series will always converge for $x=a$

During questions: 
1.  Always converge at x=a
2. Use [[Ratio Test]] or [[Root Test]] to test for convergence.
3. If asked for ==interval of convergence==: Also test boundaries.