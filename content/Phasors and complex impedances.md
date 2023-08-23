---
title: "Phasors and complex impedances"
---
# Phasors and complex impedances
## Phasors
- A Phasor has a complex and a real part ($x+yj$).
We can use $\bar{V}_a=V_a \angle \theta_a$ notation

- we can represent phasors graphically as vectors.
	- ![[Pasted image 20220314191629.png|200]]
	- One phasor leads another one if it has 

## Complex Impedances
- complex impedence $Z$ is made of a real part, $R$ and an imaginary part, called reactance $X$.
### Inductance
> $Z_L\: [\ohm]=j\omega L$
- $i_L(t) = I_m sin(\omega t + \theta)$
	- $\bar{I_L} = I_m \angle \theta -90\degree$
- $v_L(t) = \omega LI_mcos(\omega t + \theta)$
	- $\bar{V_L} = \omega LI_m \angle \theta = V_m \angle \theta$
- $X_L = 2\pi f L$
	- Always positive

### Capacitance
> $Z_C\:[\ohm] = -j\frac 1 {\omega C}$
- $v_C(t) = V_m sin(\omega t + \theta)$
	- $\bar{V}_C = V_m \angle \theta -90\degree$
- $i_C(t)=\omega C V_m cos(\omega t + \theta)$
	- $\bar{I}_C = \omega CV_m \angle \theta= I_m \angle \theta$
- $X_C = -\frac{1}{2\pi f C}$
	- This will always be negative for a capacitor

>**CIVIL**
>Capactiance: current(I) leads Voltage...
>Inductance (L): Voltage leads current(I)

### Resistance
The $I$ through resistor is always in phase with $V$.

## Complex Circuit Analysis
### KVL
$\sum V =0$

### KCL 
$\sum I = 0$

1. Write down all voltages and current sources as cosinus functions
2. Transform all the voltages and current sources to phasors.
3. Now write all **Impedances** in their complex form.
4. Solve as with DC.
