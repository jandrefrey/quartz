---
title: "Power in AC circuits"
---
[[Power]]
### At a specific time
- $p_R(t) = \frac{V_mI_m}{2}(1+cos(2\omega t))$
	- $p_{R,avg} = \frac{V_mI_m}{2}$
	- Always positive (abosorbing)
- $p_L(t) = \frac{V_mI_m}{2}(sin(2\omega t))$
	- $p_{L,avg} = 0$
	- $p_{L,peak} = \frac{V_mI_m}{2}$
- $p_C(t) = -\frac{V_mI_m}{2}(sin(2\omega t))$
	- $p_{C,avg} = 0$
	- $p_{C,peak} = \frac{V_mI_m}{2}$

So more generally:
for $\theta = \theta_v - \theta_i$:
- $p(t) = \frac{V_mI_m}{2}cos(\theta)[1+cos(2\omega t)] + \frac{V_mI_m}{2}sin\theta sin(2\omega t)$
	- $= P_{pulsating} + P_{oscillatory}$
	- = active power $P$ + reactive power $Q$
- $P_{avg} = \frac{V_mI_m}{2}cos(\theta)$
	- $= V_{rms}I_{rms}cos(\theta)$
- $P_{oscil} = \frac{V_mI_m}{2}sin(\theta)$
	- $= V_{rms}I_{rms}sin(\theta)$

Average power = active power

### Apparent power
> $S \rightarrow [VA]$
> $P \rightarrow [W]$
> $Q \rightarrow [VAR]$
- $S=V_{rms}I_{rms}$
- $S^2 = P^2 + Q^2$
	- $Scos(\theta) = P$
	- $Ssin(\theta) = Q$

- ![[Pasted image 20220314214518.png|400]]

### Power factor
$PF = cos(\theta)$
- leading: $\theta \rightarrow -$
- lagging $\theta \rightarrow +$

#### Power factor correction
Power factor correction is the process of compensating for the lagging current (low PF) by creating a leading current by connecting capacitors to the supply. A sufficient capacitance is connected so that the power factor is adjusted to be as close to unity as possible.

1. draw the circuit (add capacitor)
2. Find $P_{L,old}$ and $PF_{old}$
3. $P_{new}$ usually equal to $P_{old}$ (same work being done)
4. $PF_{new}$
5. $\theta_{old}$ and $\theta_{new}$
6. Find $Q_{new}$ and $Q_{old}$ (use $P_L$ and $tan\theta$)
7. $\bar{S}_{old}$ and $\bar{S}_{new}$
8. $Q_{comp} = Q_{new} - Q_{old}$ 
	- this will be negative as we are adding a capacitor
9. $\bar{S}_{comp} = jQ_{comp}$ (as $P_{comp} = 0$)
10. $\bar{S}_{comp} = \frac{{|\bar{V}_{rms}|}^2}{Z^*_{comp}}$ to find $Z$
11. $Z_{comp} = \frac 1 {j\omega C}$ to find $C$

### Complex Power
> $\bar{S} = \bar{V}_{rms}\bar{I}^*_{rms}$
	> $= V_{rms}I_{rms}\angle \theta$
	> = $P+jQ$

- $\bar{S} = |\bar{I}_{rms}|^2Z$
- $\bar{S} = \frac{|\bar{V}_{rms}|^2}{Z^*}$

- $\sum P_n = 0$
- $\sum Q_n = 0$

- If $I$ lags $\rightarrow$ inductive $\rightarrow$ $Q+$ $\rightarrow$ absorbs $Q$
- If $I$ leads $\rightarrow$ capacitive $\rightarrow$ $Q-$ $\rightarrow$ delivers $Q$