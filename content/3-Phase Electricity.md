---
title: "3-Phase Electricity"
---
# 3-Phase
**Advantages:**
- Total power, less pulsating
- Less conductors, cheaper, less losses

## Balanced 3-phase circuits
![[Pasted image 20220411181547.png|250]]
### Sources
- ==magn== of $\bar V_{an} = \bar V_{bn} = \bar V_{cn}$
- phase angle differ by 120
- no current through neutral branch

### Loads
- All loads have the same value $Z_a = Z_b = Z_c$
- $Z_\Delta = Z_a +Z_b + Z_c$

### Positive sequence
- $V_{an} (t) = V_Y cos(\omega t)$
- $V_{bn} (t) = V_Y cos(\omega t -120 \degree)$
- $V_{cn} (t) = V_Y cos(\omega t +120 \degree)$
- So for a positive sequence, $v_{an}$ lead $v_{bn}$, leads $v_{cn}$.

### Negative sequence
- $V_{an} (t) = V_Y cos(\omega t)$
- $V_{bn} (t) = V_Y cos(\omega t +120 \degree)$
- $V_{cn} (t) = V_Y cos(\omega t -120 \degree)$


## Steps
1. Is it balanced?
	1. Amplitude voltages must be the same
	2. Phase shift must be 120
	3. The loads must all be the same
	4. loads in line(if any) are balanced
2. $I_{Nn} = 0A$ for any balanced 3-phase
2. Identify +/- sequence
3. Identify [[Star (Y) connected sources]] or [[Delta connected sources]]
	1. Star:
		1. Seperate phases and look at 1 phase
		2. do calculations on single phase circuits.
		3. $I_{line} = I_{phase}$
		4. ==positive seq:== $V_{line} = V_{phase} \sqrt 3 \angle 30$
		5. negative seq: $V_{line} = V_{phase} \sqrt 3 \angle -30$
	2. Delta
		1. Convert to a star source
		2. Follow star approach
		3. then we can convert back to delta to find line to line voltages and phase currents 
		4. $V_{line} = V_{phase}$
		5. ==positive seq:== $V_{line} = V_{phase} \sqrt 3 \angle -30$
		6. negative seq: $V_{line} = V_{phase} \sqrt 3 \angle 30$
4. Calculate, if necessary, current and voltages in other phases and current in delta connections.

![[Pasted image 20220527235125.png]]