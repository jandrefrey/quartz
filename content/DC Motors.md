---
title: "DC Motors"
---
Different types of DC Motors include:
- [[Separately excited DC Machine]]
- [[Shunt DC Machine]]
- [[Permanent-Magnet DC Machine]]
- [[Series DC Motor]]
- [[Compound DC Motor]]

## Speed Regulation
$$
SR = \frac{n_{m,nl}-n_{m,fl}}{n_{m,fl}} \times 100 \% 
$$
- nl = no-load
- fl = full-load

$$
\omega_m=\frac{V_T}{K \phi}-\frac{R_A}{(K \phi)^2} \tau_{\text {ind }}
$$
Speed control of [[Separately excited DC Machine]] and [[Shunt DC Machine]] can be accomplished by:
1. Inserting an external resistor in series with the armature circuit (Use below rated speed)
	![[Pasted image 20230228010402.png|300]]
1. Adjusting the terminal voltage applied to the armature circuit (Use below rated speed)
	![[Pasted image 20230302104727.png|300]]
2. Inserting an external resistor in series with the field circuit in order to change the field current and hence the field flux (use when above rated speed)
	![[Pasted image 20230302104900.png|300]]

> Dot Is the operating voltage, current, torque, power and speed of machine.


## Mechanical Equation
$$\begin{split}
\tau_{ind} & = \tau_b + \tau_J + \tau_{load} \\
		&= b\omega_m +J\frac{d\omega_m}{dt}+\tau_{laod}
\end{split}
$$
- $\frac{d\omega_m}{dt}=0$ for steady condition
- $\tau_{ind}=b\omega_m$ for no-load

## Electrical Equation
$$
V_T=E_A+V_{\text {brush }}+i_A R_A+L_A \frac{d i_A}{d t}
$$
- $\frac{d i_A}{d t}$ =0 for steady state
----

- MMF : $F=N_F I_F$
- Flux : $\Phi = \frac F R =\frac{N_FV_F}{R R_F}$
	- R = Reluctance
	- R_F resistance in field circuit
	- V_F voltage applied to field circuit
## Magnetisation Curve
$$
E_A=K \phi \omega_m
$$
Flux increasing with MMF:
![[Pasted image 20230227113919.png|350]] 
Internal Voltage increasing with field Current:
![[Pasted image 20230227113953.png|350]]

## DC Motor Starters
At Start:
- $\omega = 0$, therefore $E_A = 0$
- $R_A$ very small
- Therefore, $I_A$ and $\tau_{ind}$ very high
- Hence a starting resistor in series with armature circuit or a lower starting armature terminal voltage is required

## DC Motor [[Efficiency]]
- The efficiency of a DC motor at a certain operating point, is given by
$$
\begin{aligned}
\eta & =\frac{P_{\text {out }}}{P_{\text {in }}} \times 100 \% \\
& =\frac{P_{\text {conv }}-P_{\text {no-load }}}{P_{\text {armature }}+P_{\text {field }}} \times 100 \% \\
& =\frac{\left(\tau_{\text {ind }}-b \omega_m\right) \omega_m}{V_T I_A+V_F I_F} \times 100 \%
\end{aligned}
$$





