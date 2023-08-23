---
title: "Rectifier Filters"
---
Adding a parallel capacitor:
- Capacitor charges initially
- Diode switches off at peak
- Capacitor discharges
	- At rate $e^{-\frac{t}{\tau}}$

![[Pasted image 20230816123259.png]]

## Using [[Half-Wave Rectifier]]:
$$V_r=\frac{V_M}{fRC}$$
where: $f= \frac 1 {T_p}$
> Note the ripple decreases with $R$ or $C$.

$$i_{D,avg} = \frac1{2\pi}\sqrt{\frac{2V_r}{V_M}}\cdot\frac{V_M}R\left(1+\pi\sqrt{\frac{2V_M}{V_r}}\right)$$
$$_{D, peak} = \frac{V_M}R\left(1+2{\pi}\sqrt{\frac{2V_M}{V_r}}\right)$$


## For a [[Full-Wave Rectifier]]:
$$V_r=\frac{V_M}{2fRC}$$
Where: $f=\frac{1}{2T_p}$
$$i_{D,avg} = \frac1\pi\sqrt{\frac{2V_r}{V_M}}\cdot\frac{V_M}R\left(1+\frac\pi2\sqrt{\frac{2V_M}{V_r}}\right)$$
$$_{D, peak} = \frac{V_M}R\left(1+{\pi}\sqrt{\frac{2V_M}{V_r}}\right)$$



