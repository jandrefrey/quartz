---
title: "Subspaces"
---
# Subspaces
Given a [[Vector Spaces]] V, then a subset $W\subset V$ is called a subspace if $W$ is **closed under vector addition** of $V$ and **scalar mulitplication** of $V$.
![[Pasted image 20220504210846.png]]
## Closure under vector addition.
Show that $x \in W$ and $y \in W$ $\rightarrow  x, y \in W$
- $x \in W, x = (x_1, y_1, 0)$
- $y \in W, y=(x_2, y_2, 0)$

Then $x+y = (x_1+ x_2, y_1+y_2, 0) \in W$

## Closure under multiplication
Show that $k \in R$ and $x \in W$ $\rightarrow k*x \in R$
* Let $k \in R$ and $x \in W$
	Then $x=(x_1, y_1, 0)$
- $k*x=(kx_1, ky_1, 0) \in W$

______________________________________________
Given a vector space V and a set $(x_2, x_3..., x_n) \subset V$
we say that  $(x_2, x_3..., x_n)$ is [[linearly independant]]  if
$k_1x_1 + k_2x_2+...+ k_nx_n = 0$
$k_1=k_2=k_n =0$
![[Pasted image 20220504222153.png]]
![[Pasted image 20220504222358.png]]
Think of this like: At least one of the vectors are redundant. So we can remove one, without changing the span of the vectors.

![[Pasted image 20220504222531.png]]
![[Pasted image 20220504222636.png]]



Given $B=[b_1, ..., b_n] \subset V$ linearly independent, we say $B$ is a [[Basis]] if for $x \in V$ there is $k_1, ..., k_n \in R$ such that $v=k_1\times b_1+...+k_n \times b_n$
If $B_1$ and $B_2$ are bases for $V$, then they have the same number of demands

From this we say that the dimension of $V$ is the number of Vectors in any Basis.

