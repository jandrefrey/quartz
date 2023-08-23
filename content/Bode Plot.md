---
title: "Bode Plot"
---
# Bode Plot
- A plot of 
	- magnitude of [[Filters#Transfer functions]] vs frequency
		- Transfer function is in [dB]
		- frequency in logarythmic scale ($0.01f_b, 0.1f_b, f_b, 10f_b...$)
	- phase angle of Transfer function vs frequency

## When is a filter 1st order?
- Only 1 inductor or capacitor
	- Even if there is 2 inductors/capacitors in parallel, we can combine them to form a equivalent imp, so it is still 1st order.

## Asymptotic approach
So we can go and plot every point for the f in terms of $f_b$, but it's easier to make an estemation. So for $f_b$ in standard form:
==(can we get it non-standard or will it always be like this?)==
### LPF
#### Magnitude plot
- For very low freq: $|H(f<<f_b)|_{dB}=0$
- For very large freq: $|H(f>>f_b)|_{dB}=-20log(\frac{f}{f_b})$
	- negative gradient of 20dB/decade

#### Phase plot
- $\angle H(f=0.1f_b)= -5.711 \degree \approx 0\degree$
- $\angle H(f=f_b)-45\degree$
- $\angle H(f=10f_b)= -84.19 \degree \approx -90\degree$

#### Plotting the bode plot
![[Pasted image 20220425182609.png]]

### HPF
#### Magnitude plot
- For very low freq: $|H(f<<f_b)|_{dB}=20log(\frac{f}{f_b})$
	- gradient of 20dB/decade
- For very large freq: $|H(f>>f_b)|_{dB}=0$

#### Phase plot
- $\angle H(f=0.1f_b)= 84.289 \degree \approx 90\degree$
- $\angle H(f=f_b)45\degree$
- $\angle H(f=10f_b)= 5.711 \degree \approx 0\degree$

#### Plotting the bode plot
![[Pasted image 20220425183526.png]]
![[Pasted image 20220425183457.png]]

### For [[Cascade connections]]
If we are given a more complex circuit with mulitple impediences, find H(f) as a product of a gain(most likely some constant) and H in standard form.

We can split the transfer function linearly if in decibel unit. So consider the "split transfer functions" and consider each one with the asymptotic approach. And then the final Transfer function is simply the sum of the split functions.
