---
title: "Synchronous Motors"
---
The Equivalent circuit of a Synchronous motor is the same as the [[Synchronous Generators]], however $I_A$ is reversed. Thus:
$$
V_\phi = E_A+jX_SI_A+R_AI_A
$$
And the speed, induced voltage, and induced torque is the same as with [[Synchronous Generators]]
- Torque speed characteristic curve:
	- ![[Pasted image 20230321101057.png]]

## Load Changes
- As load increases:
	- $|E_A|$ stays constant, but $\delta$ will increase.
	- $jX_SI_A$ and thus $I_A$ will increase
	- $\theta$ will decrease
![[Pasted image 20230321101934.png|350]]
## Field Current Changes
Way to control the reactive power of system.
 - Increasing field current
	 - $E_A$ increases, $\delta$ decreases.
	 - $I_A$ will decrease, then increase.
![[Pasted image 20230321102236.png|350]]

## Power factor
$E_A$ projection $< V_\phi$
![[Pasted image 20230321102422.png]]
- lagging
- small field current, underexcited

$E_A$ projection $> V_\phi$
![[Pasted image 20230321102445.png]]
- leading
- large field current, overexcited

> The lower the power factor, the greater the losses in the power lines.


---
![[Pasted image 20230321102733.png]]