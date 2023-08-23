---
title: "Diagonalisation"
---
# Diagonalisation
Recall that a Diagonal matrix looks like:
$$
A=
	\begin{bmatrix}  
	x & 0 & 0\\  
	0 & y & 0 \\
	0 & 0 & z \\
	\end{bmatrix}
$$
and also that products of these are easy-we only multiply the diagonal

## When is a matrix Diagonalisable?
- Matrix A is diagonisable if it can be written as $A=PDP^{-1}$ where D is a diagonal matrix and P is nonsingular($det \neq 0$, P is nonsingular if its columns are linearly independent). We say that P diagonalises A.
	- $A=PDP^{-1}$ 
	$P^{-1}AP=D$
	- Diagonal matrices are diagonalisable by $P=I$

> By induction:
> $A^{100}=PD^{100}P^{-1}$

**A more Usable definition:**
- A is diagonalisable if and only if A has n linearly independent [[The Eigen Value Problem|eingenvectors]].
	- Note that this means that if A is diagonalisable, it has n linearly independent Eigenvectors.

## Diagonalising A
1. Find Eigenvalues
2. Find Eigenvectors.
3. If these eigenvectors are linearly independent, we know it is diagonalisable.
	1. Let $P=(\bar v_1,\bar v_2)$ . Linearly independent. if $det(P) \neq 0$ OR if $k_1v_1+k_2v_2$ = 0 and $v_1, v_2 = 0$
4. Let D=Diagonal matrix with **eigenvalues along diagonal**
5. let **P=(eigenvector1, eigenvector2)**
6. then $A=PDP^{-1}$

## If A is [[Orthogonal Matrix|symmetric]]
- There is an orthonormal set of eigenvectors for A.
	- Then the P we create from this set of vectors is orthogonal ($P^T=P^{-1}$)
	- So then A is Diagonalisable: 
		- $A=PDP^{-1}$
		- $A=PDP^{T}$
	- **A is orthogonally diagonalisable**. P(which diagonalises A) is orthogonal.)
- If A is orthogonally diagonalisable, A is symmetric.

(go through ipad notes for examples and some extra info)