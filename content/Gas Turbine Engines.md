---
title: "Gas Turbine Engines"
---
# Gas Turbine Engines
- In reality, gas turbines operate on an open cycle
- Fresh air is continuously drawn into the compressor and exhaust gases are thrown out.
![[Pasted image 20220427164509.png]]

## Ideal Brayton Cycle
The open gas turbine cycle can be modeled as a closed cycle. The combustion process is replaces by a constant-pressure hear-addition prcoess and the exhaust process is replaced by a constant pressure heat-rejection process. 
![[Pasted image 20220427164709.png]]
Notice that this is now a [[Steady flow process]]
	
- 1-2: Isentropic Compression
	- $W_{in}$
- 2-3: Constant-pressure heat addition
	- Heat transfer from working fluid: $q_{in}=(h_3-h_2)=c_p\Delta T$
- 3-4: isentropic expansion
	- $W_{out}$
- 4-1: Constant-pressure heat rejection
	- $q_{out}=(h_4-h_1)=c_p\Delta T$

![[Pasted image 20220427164943.png]]
![[Pasted image 20220427170519.png]]

- Pressure ratio: $r_p = \frac{P_2}{P_1} = \frac{P_3}{P_4}$
- Back work ratio $r_{bw} = \frac{w_{c,in}}{w_{t,out}}$

![[Pasted image 20220427170734.png]]

### Important equations
- $q_H=c_p(T_3-T_2)$
- $W_{net}=W_{Turbine}-W_{compressor}$
- $W_T=mc_p(T_3-T_2)$
- $W_T=mc_p(T_2-T_1)$
	

## (Assumptions)
![[Pasted image 20220428165504.png]]

### Brayton Cycle with Regeneration
![[Pasted image 20220503093322.png]]
We're using the exhaust gasses to preheat the incoming air for better thermal efficiecy.
![[Pasted image 20220503093545.png]]
So for a perfect regen:
$T_4 = T_5$ and $T_2=T_6$

But for a real regen:
$T_4 > T_5$ and $T_2 <T_6$

So then
![[Pasted image 20220505145827.png]]
![[Pasted image 20220505150748.png]]

![[Pasted image 20220505150608.png|350]]
![[Pasted image 20220505150546.png]]
(bc cold air is constant specific heat)

### Brayton cycle with intercooling and reheat
![[Pasted image 20220505154849.png]]![[Pasted image 20220505160505.png]]

compression in stages, with cooling in between compression stages.
This process will minimise the compressor work, and also lowers the peak cycle temperature, and also increases m dot so more power.
1. compress in stages with equal pressure ratios per stage.
2. Cooling form 2 to 3 results in the same temp at 3 as at 1. Then also T_4 = T_2.
	 1. So $\frac{T_1}{T_2} = \frac{T_3}{T_4}$
3. ==intercooling is done at constant pressure.==
	1. $P_3 = P_2$

![[Pasted image 20220505155007.png]]
![[Pasted image 20220505154909.png]]

![[Pasted image 20220505155828.png]]
![[Pasted image 20220505160742.png]]

![[Pasted image 20220505161327.png]]

## Ideal Jet poropulsion Cycle.
Similar to brayton
![[Pasted image 20220505172938.png]]
![[Pasted image 20220505173422.png]]
![[Pasted image 20220505173544.png]]
![[Pasted image 20220505173735.png]]
so the net work out is 0

the only difference between the brayton cycle and the ideal jet - propulsion cycle is that the gases are expanded to a pressure such that the power Produced by the turbine is just sufficient to drive the compressor and auxiliary equipment - in other words the net work is zero (the aim is to create thrust not work)

### Jet propulsion
![[Pasted image 20220505174005.png]]

