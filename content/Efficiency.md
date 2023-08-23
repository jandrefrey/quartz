---
title: "Efficiency"
---
# Efficiency
> $Efficiency = \frac{Desired\: output}{Required\: input}$
## Thermal efficiency of [[Heat Engine]]
- $\eta_{th} = 1-\frac{Q_{out}}{Q_{in}} = \frac{W_{net}}{Q_{out}}$

### Thermal Effeciency of [[Carnot Cycle]] Heat engine
- $\eta_{th, rev} = 1-\frac{T_{L}}{T_{H}}$
	- $T_L$ is low reservoir temp, and $T_H$ is high reservoir temp in $K$
	- ![[Pasted image 20220412092156.png|250]]

### Thermal Efficiency of [[Reciprocating  Engines#Otto Cycle]]
$\eta_{th} = \frac{W_{n}}{q_{in}}=1-\frac{q_{out}}{q_{in}}= 1-\frac{T_4-T_1}{T_3-T_2} = 1-\frac 1 {r^{k-1}}$ where $r=\frac {v_1} {v_2}$

### Thermal Efficiency of [[Reciprocating  Engines#Diesel Cycle]]
$\eta_{th} = \frac{W_{n}}{q_{in}}=1-\frac{q_{out}}{q_{in}}= 1-\frac{c_v(T_4-T_1)}{c_p(T_3-T_2)} = 1-\frac {T_4-T_1}{k(T_3-T_2)} = 1-\frac 1 {r^{k-1}}(\frac{r_c^{k-1}}{k(r_c-1)})$

$\eta_{th, Otto} > \eta_{th,Diesel}$
as $r_c \rightarrow 1$ then $\eta_{th, Otto} \rightarrow \eta_{th,Diesel}$

### Thermal Efficiency of [[Gas Turbine Engines#Ideal Brayton Cycle]]

$\eta_{th} = 1-\frac{Q_{out}}{Q_{in}} = \frac{W_{net}}{Q_{out}} = 1- \frac{T_4-T_1}{T_3-T_2}=1-\frac{1}{r_p^{\frac{k-1}{k}}}$
using isentropic efficiency we can relate the ideal breyton cycle efiency to actual efficiencies.
![[Pasted image 20220428175126.png|300]]
	![[Pasted image 20220428175140.png]]

For brayton cycles with regen:
![[Pasted image 20220505145839.png]]
And then if we have constant entropy:
![[Pasted image 20220505150819.png]]

![[Pasted image 20220505150655.png]]
only when we have perfect regenerator and ideal gas with constant specific heats

Brayton cycle with Intercooling
![[Pasted image 20220505155732.png]]

Breyton with everything
![[Pasted image 20220505161638.png]]


### Thermal efficiency of [[Vapor Cycle#Rankine Cycle]]
![[Pasted image 20220505211913.png]]
![[Pasted image 20220505212821.png]]
note that we can't use VP at the turbine bc we have vapor and not liquid.

If the cycle regen:
![[Pasted image 20220512142400.png]]

If reheat:
![[Pasted image 20220512152455.png]]

## Propulsive efficiency
![[Pasted image 20220505174207.png]]

## [[Energy]] Efficiencies
### Specific scenarios
- $\eta_{pump} = \frac{\Delta\dot{E}_{mech,fluid}}{\dot{W}_{shaft, in}}$

- $\eta_{turbine} = \frac{\dot{W}_{shaft, out}}{|\Delta\dot{E}_{mech,fluid}|}$

- $\eta_{motor} = \frac{\dot{W}_{shaft, out}}{\dot{W}_{elect, in}}$

- $\eta_{generator} = \frac{\dot{W}_{elect, out}}{\dot{W}_{shaft, in}}$

- $\eta_{pump-motor} = \frac{\Delta\dot{E}_{mech,fluid}}{\dot{W}_{elect, in}}$

- $\eta_{turbine-generator} = \frac{\dot{W}_{elect, out}}{|\Delta\dot{E}_{mech,fluid}|}$

## Coefficient of performance
The way we measure the [[Efficiency]] of refrigerators and heat pumps.
### [[Refrigerators and heat pumps#^707e99|Refrigerator]]
- $COP_R = \frac{1}{\frac{Q_H}{Q_L}-1} = \frac{Q_L}{W_{net}}$ 
- The COP of a refrigerator decreases with decreasing refrigeration temperature.

### [[Refrigerators and heat pumps#Heat Pumps|Heat pumps]]
- $COP_{HP} = \frac{1}{1-\frac{Q_L}{Q_H}} = COP_R +1 = \frac{Q_H}{W_{net}}$ 

### COP of [[Carnot Cycle#Carnot Refrigerators and heat pumps|Carnot refrigerators and heat pumps]]
- $COP_{R, rev} = \frac{1}{\frac{T_H}{T_L}-1}$
- $COP_{HP, rev} = \frac{1}{1-\frac{T_L}{T_H}}$

![[Pasted image 20220412093006.png|350]]
We can still use Q and W for carnot cycles though!
So if we have T's we can use COP to find the Q and W

## [[Processes#Isentropic processes]] Efficiencies of [[Steady flow process]]
- Since Isentropic devices are also Reversible, they can be considered as "deal" devices.
- So Isentropic Effieciency compares actual to isentropic.
- When solving problems, only the Pressure of the actual and isentropic systems are the same.
- If you get stuck on these problems, remember you can always use Cons of Energy actual and isentropic
### [[turbines and compressors]]
![[Pasted image 20220423123548.png]]
![[Pasted image 20220423123956.png]]
### [[nozzles and diffusers]]
![[Pasted image 20220423124110.png]]

