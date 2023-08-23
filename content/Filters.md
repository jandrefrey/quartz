---
title: "Filters"
---
# Filters
![[Pasted image 20220418211331.png|200]]
## Transfer functions
- $H(f) = \frac{\bar{V}_{out}}{\bar{V}_{in}}$
	- $f_B = \frac{1}{2\pi RC}$ is the Half Power Function
	- in terms of [[Decibels]] $|H(f)|_{dB}=20log|H(f)|$
		- this is the voltage gain in dB

![[Pasted image 20220418212505.png|400]]
So we can use these graphs to find $\bar{H}$ at a specific frequency

## Lowpass filters
![[Pasted image 20220418220426.png|250]]
- $H(f) = \frac 1 {1+j\frac{f}{f_B}}$

![[Pasted image 20220418215429.png|350]]
![[Pasted image 20220418215907.png|300]]

## Highpass filter
![[Pasted image 20220418220139.png|250]]
$H(f) = \frac {j\frac{f}{f_B}} {1+j\frac{f}{f_B}}$
![[Pasted image 20220418221632.png|350|300]]


## Multiple frequency components
![[Pasted image 20220418212704.png|200]]
- We can break any functions (even square and trinagle waveforms) to sinusoidal frequency components. (with fourier transforms sometimes)
	- To calculate the **transfer function** of these functions, we have to split them into their components first, then apply the H, andthen we can add them back to find final funciton.

## Summary
![[Pasted image 20220419172327.png]]
![[Pasted image 20220425173017.png]]
using [[Decibels]]
![[Pasted image 20220425173505.png]]
## How to tell if it's low pass or high pass
1. Looking at the Circuit Diagram:
	1. for high freq, what is V_out?, and for low freq what is V_out? (Cap and high freq SC, and L in high freq OC)
2. We can look at f_b formula
3. can look ar frequency at 0 and $\infty$
	so if the f=0 and we have an open circuit, and Vout=Vin and it is a low pass filter.
	 ![[Pasted image 20220419222049.png]]
	![[Pasted image 20220419221755.png]]


![[Pasted image 20220502133608.png]]