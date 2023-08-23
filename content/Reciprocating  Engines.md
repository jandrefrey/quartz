---
title: "Reciprocating  Engines"
---
# Reciprocating  Engines
These are types of [[Power Cycles]]

![[Pasted image 20220426220456.png]]
![[Pasted image 20220426221259.png]]

- Compression ratio = $\frac{V_{BDC}}{V_{TDC}}$
- Mean effective pressure (MEP) = $\frac{W_{net}}{V_{max}-V_{min}}$ [kPa]
- $W_{net} = MEP \times Displacement \: Volume$
- $m_{in} = N_{cylinders} \frac{\Delta V}{v} = N_{cylinders} \frac{\pi B^2 S / 4}{v}$
- $\dot W_{net} = \frac{W_{net} \times rpm}{rev/cycle}$
	- rev/cycle is 2 for 4-stroke.

## Otto Cycle
The Ideal Cycle for **spark-ignition(petrol) engines**
![[Pasted image 20220426224705.png]]
- So for an Ideal Otto Cycle:
	- $W_{out,0-1} = P_0(v_1-v_0)$
	- $W_{in,1-0} = P_0(v_1-v_0)$

So we can use the Air stantdard assumptions from [[Power Cycles]] for an **ideal otto cycle**:
- 1-2: Isentropic Compression [[Processes]]
- 2-3: Constant-volume heat addition (**NO WORK**)
	- $q_{in} = u_3-u_2 = c_v(\Delta T)$ since cold air assumptions assume constant specific heats
- 3-4: Isentropic expansion
- 4-1: constant-volume heat rejection. (**NO WORK**)
	- $q_{out} = u_4-u_1 = c_v(\Delta T$)

![[Pasted image 20220426230306.png]]
![[Pasted image 20220426230636.png]]


## Diesel Cycle
The Ideal Cycle for **compression ignition Engines**
- 1-2: Isentropic Compression [[Processes]]
- 2-3: Constant-**PRESSURE** heat addition
	- $q_{in} = \Delta u + P\Delta v = \Delta h = c_p(T_3-T_2)$
- 3-4: Isentropic expansion (ideaL gas, variable sp heats))
- 4-1: constant-volume heat rejection. (**NO WORK**)
	- $q_{out} = u_4-u_1 = c_v(\Delta T)$

![[Pasted image 20220531095747.png]]
notice that we use cp for the constant pressure process, because h and we use cv for the constant volume process because u.


- Cutoff ratio: $r_c=\frac{v_3}{v_2}$
- Cobining that with .. we can find **compression ratio**: $r=\frac{v_1}{v_2}$
![[Pasted image 20220427160257.png]]

