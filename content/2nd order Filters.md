---
title: "2nd order Filters"
---
# 2nd order [[Filters]]
Circuits with more than 1 reactive components.

1. Find H(f)
2. Equate to standard form
	1. ![[Pasted image 20220502130653.png|400]]
3. find f_o
4. find $\zeta$
5. is it < or > 1
6. as in pohots below...

![[Pasted image 20220501221734.png]]
![[Pasted image 20220502105802.png]]
## 2nd order LPF
![[Pasted image 20220501223258.png]]


## 2nd order HPF
![[Pasted image 20220501223558.png]]

## Series resonant circuit
![[Pasted image 20220502131048.png|250]]
We can measure V_out over different parts over the circuit to get a HPF, LPF. But if we take it over both R or L and C, we can get a band pass or band reject filter.

![[Pasted image 20220502131714.png]]
Comparing quality factors:
![[Pasted image 20220502134307.png|250]]
![[Pasted image 20220502134329.png|250]]


### Band Pass and Band Reject filter
![[Pasted image 20220502132508.png]]

![[Pasted image 20220502132604.png]]

We weill usually get these in the form of [[Cascade connections]] to plot. And if it comes out in the above form bode plots, we know its a BPF/BRF

## Parallel res circuits
Similar to series..