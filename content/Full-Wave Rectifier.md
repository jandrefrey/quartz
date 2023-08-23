---
title: "Full-Wave Rectifier"
---
Rectify the full wave – even the negative half cycle.
## Centre-Tapped Full-Wave Rectifier
![[Pasted image 20230810122942.png]]
![[Pasted image 20230810123743.png]]
![[Pasted image 20230810124530.png]]
### $v_I$ positive half cycle: 
- $v_s$ is in its positive half cycle.
- $D_1$ - forward bias & $D_2$ - reverse bias.
- $v_o = v_s - V_\gamma$
> $$PIV = 2(v_{s(max)} - v_\gamma$$ (maybe relocate)
![[Pasted image 20230810123251.png]]

![[Pasted image 20230810123236.png]]
### $v_I$ negative half cycle: 
- $v_s$ is in its negative half cycle.
- $D_1$ - reverse bias & $D_2$ - forward bias.
- $v_s + V_\gamma + v_o = 0$
- $v_o = -v_s - V_\gamma$
![[Pasted image 20230810123524.png]]

## Full-Wave Bridge Rectifier
![[Pasted image 20230810123942.png]]
![[Pasted image 20230810124519.png]]
### When $v_s$ is positive
![[Pasted image 20230810124127.png]]
- Diodes $D_1$ and $D_2$ are on – forward bias.
- Diodes $D_3$ and $D_4$ are off – reverse bias.
- $v_o = v_s - 2V_\gamma$
### When $v_s$ is negative
![[Pasted image 20230810124119.png]]
- Diodes $D_3$ and $D_4$ are on – forward bias.
- Diodes $D_1$ and $D_2$ are off – reverse bias.
- $v_o = -v_s - 2V_\gamma$

