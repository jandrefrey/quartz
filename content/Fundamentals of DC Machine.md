---
title: "Fundamentals of DC Machine"
---
## Linear DC Machine
![[Pasted image 20230328094617.png|400]]
![[Magnetic Fields#A current-carrying wire near a magnetic field has a force induced on it.]]
![[Magnetic Fields#A moving wire near a magnetic field has a voltage induced on it.]]

Considering Kirchhoff's voltage law: $$V_B=iR+e_{ind}$$
and thus $i=\frac{V_B-e_{ind}}{R}$
### Starting Linear Machine
- Initially bar at rest
	- $e_{ind} = 0$
	- $i=\frac{V_B}{R}$
- Then current flow through bar (in presence of magnetic field) induces magnetic field
	- $F_{ind} = ilB$
- Bar accelerates, voltage appears across bar.
	- $e_{ind} = vBl$
- Then $i$ reduces as $e_{ind}$ increases until we reach steady state where $e_{ind}=V_B$ and the force on the bar is 0. Then the speed of the bar is:
	- $v_{ss}=\frac{V_B}{Bl}$

### Motor Operation
Starting initially at no load (steady state) condition. $F_{load}$ is applied opposite direction.
$v$ decreases, $e_{ind}$ decreases, $i$ increases. $F_{net}$ increases until
- $F_{ind} = F_{app}$
- $i=\frac{F_{ind}}{lB}$
- $e_{ind} = V_B - iR$
- $velocity=\frac{e_{ind}}{Bl}$
- $P_{conv} = F_{ind} v$

### Generator Operation
Starting initially at no load (steady state) condition. $F_{load}$ is applied in same direction.
$v$ increases, $e_{ind}$ increases, $i$ decreases. $F$ decreases until:
- $F_{ind} = F_{app}$
- $e_{ind} = V_B + iR$

## Real DC Machines
![[Pasted image 20230220220220.png]]
$e_{ind} = e_{ba}+e_{dc} = 2vBl = 2r\omega B l$
![[Pasted image 20230220220337.png|250]]

- If there are P poles on the machine, then the portion of the area associated with each pole:
	$A_P=\frac{2k\pi rl}{P}$

- The armeture voltage:
	$K=\frac{ZP}{k2\pi a}$
	$E_A = K(\Phi _P)\omega_m$ 
- induced torque:
	$\tau_{ind} = K\Phi _P I_A$

