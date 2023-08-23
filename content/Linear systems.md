---
title: "Linear systems"
---
# Linear systems
----

## Singular matrix

> Recall:
> If det(A)=0 then $A^{-1}$ DNE. A is thus Singular.

can have 0 or infinite sollutions if singular
If non-singular, 1 sollution.

In order to be non-singular (Invertible):
- rank() should match matrix size (since rows/columns are independent.)
- cond() should be small (well-conditioned)
- condest()
- det() should not = 0 (only for certain cases of small matrices bc of round-off error - not a good indicator.)


## Residual
We can calculate with error $\tilde x$ and plug back into eq. This is called ==Residual== ($r=b-A \tilde x$)
We can relate residual to error by multiplying with condition number. Residual can be small, but if cond(A) is large, then the relative error in the approximation can still be big.
