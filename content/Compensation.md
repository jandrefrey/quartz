---
title: "Compensation"
---
Controller compensates for weakness (stability, response) in the system performance.
## Lead Compensation
### [[PID Control#Proportional + Derivative (PD) control|PD Control]]
We can write:
$$D_c(s) = T_Ds+1$$

We may reduce the high frequency noise amplification by adding a **pole**:
$$kD_c(s) = k\frac{T_D s +1}{\alpha T_D s +1}$$
#### break frequencies
At this frequency, the **zero** will have an effect on the frequency response:
$$\omega = \frac 1 {T_D}$$

At this frequency, the **pole** will have an effect on the frequency response:
$$\omega = \frac 1 {\alpha T_D}$$

> $\alpha$ is the ratio between zero and pole break frequencies.
> Thus $\alpha < 1$ for lead compensators

Frequency where max phase ($\phi_{max}$) is added to the system:
$$\omega_{max} = \frac{1}{T_D\sqrt{\alpha}}$$
> Note that we should not add more than $70\degree$ with a lead compensator to avoid high frequency noise.


![[Pasted image 20230815231138.png|350]]

$$\sin(\phi_{max})=\frac{1-\alpha}{1+\alpha}$$
$$\alpha=\frac{1-\sin\phi_{max}}{1+\sin\phi_{max}}$$

1. Find K that satisfies error or bandwidth requirement
2. Evaluate current PM for $\text{KG(s)}$
3. Calculate amount of phase to be added for PM requirement
4. Calculate $\alpha$ (using equation or graph)
5. Calculate T using equation with calculated $\alpha$ and $\omega_{max}=\omega_{c}$（from $\text{KG(s)}$)
6. Draw compensated Bode plot
7. Iterate design

## Lag Compensation
Considering a PI controller:
$$D_{c}(s)=\frac{K}{s}\biggl(s+\frac{1}{T_{I}}\biggr)$$
### Normal Form
$$D_{c}(s)=\alpha\frac{T_{l}s+1}{\alpha T_{l}s+1}$$
To avoid the oscillation and overshoot introduced by a PI control, we need to change where the pole is located.

> Thus $\alpha > 1$ for lag compensators

Select T such that effect is at much lower frequency than uncompensated $\omega_c$.
Design Steps:
1. Find K that satisfies PM requirement
2. Evaluate low frequency error for KG(s)
3. Determine c to satisfy low frequency error requirement4.
4. Select T so that the break frequency of the zero is one decade lower than $\omega_{c}$ (from KG(s)
$$
\omega={\frac{1}{T}}
$$
5. Break frequency of the pole will be at
$$
\omega=\frac{1}{\alpha T}
$$
6. Iterate design

### Unity DC Gain
$$D_c(s)=\frac{T_ls+1}{\alpha T_ls+1}$$
At lower frequency it has magnitude of 1
at high frequency magnitude<1

1. Find K that satisfies low frequency error requirement 
2. Evaluate current PM for KG(s)
3. Determine a to satisfy PM requirement4.
4. Select T so that the break frequency of the zero is one decade lower than oe(from KG(s)
$$
\omega=\frac{1}{T}
$$
5. Break frequency of the pole will be at
$$
\omega=\frac{1}{\alpha T}
$$
6. Iterate design

## Lead-Lag Compensator
$$KD_{c}(s)=K\bigg(\alpha\frac{T_{l}s+1}{\alpha T_{l}s+1}\bigg)\bigg(\frac{T_{D}s+1}{\alpha T_{D}s+1}\bigg)$$


![[Pasted image 20230817224533.png]]