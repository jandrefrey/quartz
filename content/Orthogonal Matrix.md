---
title: "Orthogonal Matrix"
---
# Orthogonal Matrix
A matrix (A) is **symmetric** if the [[Transposed matrix]]$(A^T)=A$
If a matrix is Real and symmetric, all [[The Eigen Value Problem|Eigenvalues]], and Eigenvectors are Real, and Eigenvectors corresponding to different Eigenvalues are orthogonal.

> Recall that $(AV)^T= V^TA^T$
> ![[Pasted image 20220508221843.png]]

So orthogonal basically means a higher dimensional generalisation of perpendicular.
![[Pasted image 20220508222818.png]]
![[Pasted image 20220508223111.png]]

## Orthonormal set of vectors
![[Pasted image 20220509090833.png]]
So it is orthogonal and unit vectors.

## Orthogonal Matrix
A matrix is orthogonal if its columns form an orthonormal set of vectors. So if we take the columns separately, they will form an orthonormal set.
Or in other words:
![[Pasted image 20220509091508.png]]
So we can find Orthogonal matrix by finding Eigenvectors for each eigenvallue. ( note that multiple eigenvectors for the same eigenvallue will not the orthogonal.) 
In this case where we have multiple eigenvectors for an eigenvalue, we process as follows:
![[Pasted image 20220509100924.png]]
Then, where K1 and K2 weren't orthogonal, V1 and V2 are.