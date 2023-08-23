---
title: "AC Machine Fundamentals"
---
For a 3-coil machine:
$$
\begin{aligned}
i_{a a^{\prime}}(t) & =I_M \sin \omega t \\
i_{b b^{\prime}}(t) & =I_M \sin \left(\omega t-120^{\circ}\right) \\
i_{c c^{\prime}}(t) & =I_M \sin \left(\omega t-240^{\circ}\right)
\end{aligned}
$$
$$\begin{aligned}
&\ \mathbf{H}_{a a^{\prime}}(t)=H_M \sin \omega t \angle 0^{\circ} \\
& \mathbf{H}_{b b^{\prime}}(t)=H_M \sin \left(\omega t-120^{\circ}\right) \angle 120^{\circ} \\
& \mathbf{H}_{c c^{\prime}}(t)=H_M \sin \left(\omega t-240^{\circ}\right) \angle 240^{\circ}
\end{aligned}
$$
$$
\begin{aligned}
& \mathbf{B}_{a a^{\prime}}(t)=B_M \sin \omega t \angle 0^{\circ} \\
& \mathbf{B}_{b b^{\prime}}(t)=B_M \sin \left(\omega t-120^{\circ}\right) \angle 120^{\circ} \\
& \mathbf{B}_{c c^{\prime}}(t)=B_M \sin \left(\omega t-240^{\circ}\right) \angle 240^{\circ}
\end{aligned}
$$
$$
\mathbf{B}_{\mathrm{net}}(t)=\left(1.5 B_M \sin \omega t\right) \hat{\mathbf{x}}-\left(1.5 B_M \cos \omega t\right) \hat{\mathbf{y}}
$$
----
Electrical **frequency** of stator: $$f_{se}=\frac{n_{sm}P}{120}$$ 
	P is the number of poles
	n is the number of revolutions per minute. ^1db4d6

## Induced voltage
$$e_{ind} = N_C \Phi \omega cos(\omega t)$$
Then the RMS voltage (for 3 phase) can be given: $$\begin{align}
E_A&=\sqrt 2 \pi N_C \Phi f \\
&=K\phi \omega
\end{align}$$where $K$ is a constant representing the construction of the machine. If $\omega$ is expressed in electrical radians per second, then$$
K=\frac{N_c}{\sqrt{2}}
$$while if $\omega$ is expressed in mechanical radians per second, then$$
K=\frac{N_c P}{\sqrt{2}}$$ ^e2000d
> If the machine is Y-connected, then the terminal voltage $(V_T=V_L) = \sqrt 3 \times V_\phi$, and $I_A=I_L$
> if the machine is Δ-connected, then the terminal voltage $(V_T=V_L) = V_\phi$,  and $\sqrt 3 I_L=I_A$
> *The given voltage is usually $V_T$*

^beb3dc

Often we first need to convert $E_A$ to $V_\Phi$ to determine the voltage per phase. This highly depends on the question but can often present as $\frac{\#slots}{\#phases}$

## Induced Torque
$$\begin{align}
\tau_{ind} &= k\mathbf{B}_R+\mathbf{B}_S \\
&= k\mathbf{B}_R+\mathbf{B}_{net} \\
&=kB_RB_{net}sin\delta
\end{align}$$
where δ is the angle between $B_R$ and $B_{net}$

## Power in AC Machines
- [[Efficiency]] of an AC machine:
	- $\eta = \frac{P_{out}}{P_{in}} \times 100\%$

- Losses in AC machines
	- Electrical/copper/$I^2R$ losses
		- Stator Copper Losses: $P_{\mathrm{SCL}}=3 I_A^2 R_A$
		- Rotor Copper Losses $P_{\mathrm{RCL}}=I_F^2 R_F$
	- Core Losses
		- hysteresis losses and eddy current losses
	- Mechanical Losses
		- friction and windage
		- called the no-load rotational loss of the machine. At no load, all the input power must be used to overcome these losses. Therefore, measuring the input power to the stator of an ac machine acting as a motor at no load will give an approximate value for these losses.
	- Stray load losses
		- For most machines, stray losses are taken by convention to be 1 percent of full load.


![[Pasted image 20230302225955.png|500]]

## Voltage Regulation
$$
\mathrm{VR}=\frac{V_{\mathrm{nl}}-V_{\mathrm{fl}}}{V_{\mathrm{fl}}} \times 100 \%
$$
## Speed Regulation
$$
\begin{aligned}
\mathrm{SR} &=\frac{n_{\mathrm{nl}}-n_{\mathrm{fl}}}{n_{\mathrm{fl}}} \times 100 \% \\
&=\frac{\omega_{\mathrm{nl}}-\omega_{\mathrm{fl}}}{\omega_{\mathrm{fl}}} \times 100 \%
\end{aligned}
$$