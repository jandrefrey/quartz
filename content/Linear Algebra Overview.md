---
title: "Linear Algebra Overview"
---
# Linear Algebra Overview
We can have different perspectives of vectors. We can view it as lines in space, sets of info. It can really be anything given by a set of axioms.

It's useful to think of vectors as arrows pointing from an origin. We can write them in matrix form vertically. We wanna focus on defining our vector space for vector addition and scalar(some constant) multiplication. 
![[Pasted image 20220609215949.png]]

We can also think of each element of the vector as a set of scalars, stretching a unit vector of that vector space (i, j, k). This is called the basis of the vector space.

Notice that using any two basis vectors we can scale them(this is called a linear combination of the vectors eg $\bar y=c_1\bar v_1 + c_2\bar v_2$) to effectively reach any point in the vector space. (as long as they aren't the same basis vector). 

This linear combination of the vectors (where we can use any scalars) is called the span of the vectors. It basically asks what is the set of all the vectors we can reach using scalar multiplication and vector addition.

Going back to the case where the basis vectors line up: These vectors are called **linearly dependent** (Det = 0). Or in other words the one vector is a linear combination of the other vector. If the vectors don't line up, and each new vector basically adds a new 'dimension', they are said to be **linearly independent**.

We can predict the movement of a vector through a linear transformation by looking at the transformation of the basis vector. This is called the transformation matrix and we can simply multiply it with any vector to find the transformation of that vector.

The determinate of a matrix determines how much the "area of a matrix" gets scaled when transformed. So looking back at our previous case, if the transformation matrix would squish the matrix to some lower dimension(line or dot) then we know the area is 0, thus Det = 0, this linearly dependent.
> If the det is 0, there is no inverse. You cannot unsquish a line to form a plane.

Orthonormal transformation "preserves dot product". there are no squishing or morphing occuring, so the vectors remain perpendicular and with unit lengths.

If we apply a transform to a matrix and the span of that tranformed matrix is the same as the original matrix(so the vectors only gets scaled), then the matrix is an eigenvector, stretched by the eigenvalue. Anytime we have a diagonal matrix, all the basis vectors are eigenvectors, and the diagonal entries are the eigenvalues. (Eigenbasis: Eigenvectors that are also the basisvecors.)

So for any diagonal matrix, it is almost like the eigenvectors are the (i, j) components. Then no matter how we transform the vector space, the span does not change.

We can change the basis to find the diagonal eq of any matrix.
![[Pasted image 20220610131419.png]]
We can do this to find the diagonal eq of any matrix.

> We can do the following with matrices(row operations):
> 	Scale any row
> 	Interchange any row
> 	Add or subtract a mutiple of one row to another.

