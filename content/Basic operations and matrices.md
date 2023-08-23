---
title: "Basic operations and matrices"
---
[[NM 262 MOC]]
# Basic operations and matrices
---

## Basic operations
- We can easily perform all basic operations like addition, subtraction, exponents, multiplication, etc.
```matlab
>> 2+3
ans = 5
```

- We can Assign variables:
```matlab
>> radius = 10;
```

- We have built in constants:
	- `pi`
	- `i` (complex)
	- `e`
- And also basic functions
	- `sqrt`
	- `exp` ($e^x$)
	- `log` (ln)
	- `cos`

- We can write numbers in exponential form:
	- $3 \times 10^8$ = `3e8`

- Notice that Matlab works to 16 dec places, so very small numbers can be seen as 0. (but not in tests)

- We can produce `inf` and `NaN` (NotaNumber) results.

- Matlab uses standard arithmetic order.

- We can get more or less demicals by using
	- `format long` and `format short`

---
## Matrices
- Row vector: 
```matlab
>> rv = [3, 1, 4]
rv = 3  1  4
```

- Column vector:
```matlab
>> cv = [3; 1; 4]
cv = 3
     1
     4
```

- Matrix
```matlab
>> m = [3, 1; 4, 5]
m =  3  1
	 4  5
```

**notice that rows are separated with semicolons.**

- Entries can be extracted:
	- `cv(2)` = 1
	- `cv(2:4)`= 1; 4; -1
	- `m(2:3,4)`= 1; 4
	- `m(:,3)`= -1; -9; 6

- Functions:
	- `size(cv)` yields matrix size
	- `ones(2, 3)` yields 2x3 ones matric
	- `eye(3)` yields 3x3 identity matrix

- scalar multiply with `s*cv`
- matrix multiply with `m*cv`
	- (dimensions!)
- Transpose `m'`
- Dot product `dot(m1, m2)` or `m1'*m2`
- ==New rules:== These will all be performed component-wise
	- Dot-multiply `v1.*v2` (notice that `2*x` needs no dot product as it is scalar multiplication - well defined.)
	- dot-divide `v1./v2`
	- dot-exponentiation `v2.ˆ2`
	- Add scalar to vector `4+2x` where `2x` is a vector
	- functions `pi`, `cos`

- Vectors with uniformly spaced entries:
	- `[1:4]` = 1 2 3 4
	- `[3:2:9]` = 3 5 7 9
	- can also use `linespace(0, 2, 5)` to create 5 evenly space points in `[0, 2]`
- plot graphs `plot(x, y)`

- `help elmat` lists the elementary functions for the assembly and manipulation of matrices
- `help elfun` lists the elementary math functions, including trig, exponential, complex, and rounding functions

- `;` can suppress a command, or be used to separate commands