---
title: "Exact equations"
---
## Exact equation
This is a [[Differential equations]]
- Given $f(x,y)$
The differential of $f$ is:
- $df=\frac{\partial f}{\partial x} dx + \frac{\partial f}{\partial y}dy$
	- See [[Partial derivatives]]

### Steps to solve:
1. Test exactness by

> So in form $Mdx + Ndy = 0$
> This is exact if $\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}$ 

2. If exact, then there exists $f$ so that $df = Mdx + Ndy$
3. So then $\frac{\partial f}{\partial x} = M$ and $\frac{\partial f}{\partial y} = N$
4. Choose 1 from (3) and integrate to find $f$. ==Remember $+g()$==
5. Differentiate wrt x or y (different than chose at (3)). (now $g'()$)
6. Set equal to N or M (different than chose at (3)) and find $g'()$)
7. Integrate to find $g()$
8. Write final $f$

### Using Integration Factor
- $\mu .Mdx + \mu .Ndy = 0$
	- Assume $\mu$ is a function of $x$ or $y$ but not both
- Then for DE to be exact
	- $\frac{\partial}{\partial y}(\mu .M) = \frac{\partial}{\partial x}(\mu .N)$
- FInd $\mu$
- ==THEN== $\mu .Mdx + \mu .Ndy = 0$ is exact...
- follow normal exact equations

> Add demi formula