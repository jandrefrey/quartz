---
title: "The Eigen Value Problem"
---
If A is an $(n\times n)$ matrix and $\bar x \in R^n$ and $\lambda \in R$ and such that $A\bar x = \lambda \bar x$ and ($\bar x \neq 0)$

Then
- $\lambda$ is an eigenvalue of A
- $\bar x$ is the eigenvector of A corresponding to $\lambda$

If $\bar x \neq 0$ and $\lambda \in R$ is an eigenvector and $\lambda$ the corresponding eigenvalue then
- $A \bar x = \lambda \bar x$
- $\rightarrow (A-\lambda I_n)\bar x = \bar 0$
- $\rightarrow det(A-\lambda I_n) = 0$
	- where $I_n$ is the identity matrix

**Basically**: The Eigenvector, with magnitude of eigenvalue is the vector along which the span of a transposed vector does not change.

## Solving Eigenvalue problems
$A\bar K = \lambda \bar K$
1. Find the eigenvalue $\lambda$ using:
	1. $(A-\lambda I)K=0$
	2. There exists a nonzero K making this equation hold if and only if $det(A − λI) = 0$
		1. So if we have 
	$$A=
	\begin{bmatrix}  
	a & b & c\\  
	d & e & f \\
	h & i & j \\
	\end{bmatrix}
	$$
	then $(A − λI)$ will be 
		$$
	A=
	\begin{bmatrix}  
	a-\lambda & b & c\\  
	d & e-\lambda & f \\
	g & h & i-\lambda 
	\end{bmatrix}
	$$
	2. Then using Gauss Jordan Elimination or row reduction (or just inspection for a 2x2 matrix), we can find the multiple values of $\lambda$
		
2. using $(A − λI)K = 0$ solve the Eigenvector for each eigenvalue.
	1. Where the eigenvector is:
		$$
	K=
	\begin{bmatrix}  
	k_1 \\  
	k_2 \\
	k_3 
	\end{bmatrix}
	$$
	2. So plug in each eigenvalue and find the corresponding eigenvector.
	$$
		\begin{bmatrix}  
		a-\lambda & b & c\\  
		d & e-\lambda & f \\
		g & h & i-\lambda 
		\end{bmatrix}
		
		\begin{bmatrix}  
		k_1 \\  
		k_2 \\
		k_3 
		\end{bmatrix}
		=0
		$$
![[Pasted image 20220519115144.png]]
![[Pasted image 20220519120029.png]]

Eigenvectors corresponding to distinct eigenvalues are linearly independent. As a consequence, **if all the eigenvalues of a matrix are distinct**, then their corresponding eigenvectors [span](https://www.statlect.com/matrix-algebra/linear-span) the space of [column vectors](https://www.statlect.com/matrix-algebra/vectors-and-matrices) to which the columns of the matrix belong. **However**, eigenvectors from different eigenvalues can still be linearly independent, so check.
