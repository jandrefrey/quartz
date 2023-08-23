---
title: "Entropy"
---
# Entropy
check photos from tut session
- Measure of disorder.
- Thermal energy that is unavailable to be converted to work
- From [[Second law of thermodynamics]], entropy of an isolated system is always increasing.
-  It is not dependant of path, only dependant on the state.

> $\Delta S = \int_1^2(\frac{dQ}{T})_{int.rev}$
> Where s is entropy in [kJ/K] for internally reversable process.
> Specific entropy is [kJ/kgK].

## Special cases
### Internally reversible, isothermal [[Processes]] heat transfer
> $\Delta S = \frac Q T$

If we have a large source or sink that doesn't change temp during the process, then it will be isothermal, and we can use this formula.

## Clausius Inequality
![[Pasted image 20220414081557.png]]
(Differential heat transfer per temp integrated over a cycle)

If something totally reversible or internally reversable
![[Pasted image 20220414081936.png]]

Irreversible
![[Pasted image 20220414081949.png]]


## Increase in Entropy principle
> - $\Delta S = \int_1^2(\frac{dQ}{T}) + S_{gen}$
> 	Change in entropy = entropy change due to heat transfer + entropy change due to irreversibilities
> 	- $\Delta S = 0$ if isentropic [[Processes]]
>	- $\int = 0$ if adiobatic [[Processes]]
> 	- $S_{gen}  = 0$ if reversible [[Processes]]

- So we can use s_gen to determine how reversible a process is.
	- $S_{gen} = +$ irreversible, 
	- $S_{gen} = 0$ reversible

- **if a process is reversible and adiobatic, then it must be isentropic so then we can use constant entropy throughout system. $S_{in} =S_{out}$**

### Isolated (adiabatic)
$S_{gen} = \Delta S$
(integral falls away and $S_{gen} = +$)

We can consider a system and its surroundings as an isolated system.
So $S_{gen, total} = \Delta S_{source}+ \Delta S_{sink}$
So when solving problems where we asked TOTAL entropy change, we have to find the entropy change in the system AND the surroundings.


## Entropy of pure Substances
From our tables: 
![[Pasted image 20220414090942.png|300]]

![[Pasted image 20220414091022.png|100]]
The entropy change of a substance can be negative(if there's losses), but the total entropy can never be <0.

## T-s Diagram
![[Pasted image 20220414094709.png]]

![[Pasted image 20220414094801.png]]

![[Pasted image 20220414094851.png]]

## Tds equations
From [[First law of thermodynmics]]:
![[Pasted image 20220414095340.png]]
Correction:
![[Pasted image 20220422100524.png]]
But we know du, dh and [[Specific Heats]]
Soooo, for [[Incompressible substances]]
![[Pasted image 20220414095621.png]]
and then if isentropic, it will also be isothermal

## H-s diagram
![[Pasted image 20220414095010.png]]

## Entropy of [[ideal gas]]
Do not use these equations when working with steam or R-134a
### Finding entropy change
#### with Average specific heats
![[Pasted image 20220422100343.png]]
and for constant [[Specific Heats]]
![[Pasted image 20220422100418.png]]
And this is when R is per unit mass.

#### With property tables
Using tables A-17 we can get $s\degree$ (more exact than $c_{avg}$)
![[Pasted image 20220422100916.png]]
When is Rln a +?

### Constant entropy of ideal gasses
#### For constant specific heats (less acurate)
Table A2:
if you don't know what T you are ending with, use the k of the initial T.
![[Pasted image 20220422101255.png]]
#### With variable specific heats
For air A17: 
![[Pasted image 20220422101304.png]]
![[Pasted image 20220422101434.png]]