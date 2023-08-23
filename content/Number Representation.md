---
title: "Number Representation"
---
- Decimal/base-10 numbering system: Each digit represents a multiple of a power of 10.
	- $9742_{10} = 9\times 10^3 + 7\times 10^2 + 4\times 10^1 + 2\times 10^0$
- Binary/base-2 numbers: Each bit represent a multiple of a power of 2.
	- An N-bit binary number represents one of 2N possibilities.
- Hexadecimal/base-16: Each digit represents a multiple of a power of 16.
	- Each hexadecimal digit represents a group of four bits (4 binary digits).
-----

- Unsigned numbers range from $0$ to $2^n-1$
- Signed numbers range from $-2^{n-1}$ to +$2^{n-1}-1$
- 2s complement are identical to unsigned binary numbers, but the most significant bit has a weight of $-2^{N-1}$ instead of $2^{N-1}$.

Sizes are declared in C with`stdint.h`:
![[Pasted image 20230727101802.png]]

## Floating point numbers
$$Value = (-1)^s \times (1.M) \times 2^{E-b}$$
- $S$ = Sign bit
- $M$ = Mantissa
- $E$ = Exponent
- $b$ = bias

Single precision provides typically 6–9 digits of numerical precision, while double precision gives 15–17.
![[Pasted image 20230727102219.png]]

## ASCII

Used to interpret numbers as characters:
![[Pasted image 20230727102359.png]]
![[Pasted image 20230727102411.png|400]]



