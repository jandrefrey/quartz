---
title: "Eigenvalues"
---
# Eigenvalue
[[The Eigen Value Problem]]

> Recall $Av=\lambda v$

Non-Trivial Solutions ($v \neq 0$) is only possible if ($A-\lambda I$) is singular... ($det(A-\lambda I)=0$) but this calc is NOT performed in MATLAB.

To avoid ill-conditioned equations in eigen-computations, we use ==eig()== .
- eig() returns eigen ==values==
- [V, D] = eig(A) returns eigenvalues and eigenvectors.
	- Columns of V contain eigenvectors, diagonal of D contains eigenvalues This is so that $AV=VD$
- eigs() will return smallest or largest eigenvalues.