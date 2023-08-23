---
title: "Synchronous Generators"
---
This is a machine that operates on a rotating speed synced to the electrical speed.
![[AC Machine Fundamentals#^1db4d6]]

- A Synchronous Machine has **DC current** at the rotor windings and **AC current** at the stator windings.
- Rotors can be salient(sticking out - ideal for low speed and >4 poles) or non-salient(cylindrical - ideal for high speed and 2 or 4 poles)
	- ![[Pasted image 20230306112858.png|300]]
- Small Machines may use brushes+slip rings to supplt rotor current where larger machines use brishless excitation
	- ![[Pasted image 20230306113219.png|350]]

----
## Induced voltage
Refer to [[AC Machine Fundamentals]]
- Usually $V_{\phi}$ **is not equal to** $E_A$ (unless when armature current is 0) due to: 
	- Distortion of the air-gap magnetic field caused by armature reaction
	- The self inductance of the armature coils
	- The resistance of the armature coils

> $$V_{\phi}=E_A-jX_sI_A-R_AI_A$$
> and $X_S=X+X_A$ (self-induced+armeture)

**Recall:**
![[AC Machine Fundamentals#^beb3dc]]

We will only consider 1 phase and multiply the power or torque by 3:
![[Pasted image 20230306115632.png|400]]

## Phasor Diagram
- $I_A$ is current flowing **out of system**
- Recall $I_A$ lags $jX_SI_A$ by $90 \degree$ (CIVIL)

$$P_{\text {conv }}=\frac{3 V_\phi E_A}{X_S} \sin \delta$$
where $\delta$ is the torque angle or power angle of the machine (angle between $V_\phi$ and $E_A$)
Then:
$$\tau_{\text {ind }}=\frac{3 V_\phi E_A}{\omega_m X_S} \sin \delta$$
And the reactive power given by:
$$
Q=\frac{3 V_\phi E_A}{X_S} \cos \delta-\frac{3 V_\phi^2}{X_S}
$$
(INSERT TEXTBOOK IMAGES)
## Measuring parameters
- $R_A$ measured by DC voltage test
- $V_{Terminal}$ measured by disconnecting loads and running at rated speed (**Open-circuit test**)
	- Saturation occurs if $I_F$ becomes too high
	- $E_A=V_\phi$ since open-circuit ($I_A=0$)
	- ![[Pasted image 20230309090453.png|300]]
- $I_A$ measured by shorting armature terminals and running at rated speed.
	- Since $X_S \gg R_A$, the armature current $I_A$ significantly lags the induced voltage $E_A$. The stator flux density phasor $B_S$ lags $I_A$ by $90^{\circ}$ and consequently will lag the $B_R$ by almost $180^{\circ}$.
	- $B_{net}$ is too low to cause saturation.
	- ![[Pasted image 20230309090524.png|300]]
- Unsaturated synchronous reactance:
	$$X_{S \mid \text { unsat }} \approx \frac{E_A}{I_A}=\left.\frac{\left.V_\phi\right|_{\text {OCC, air-gap line }}}{\left.I_A\right|_{S C C}}\right|_{I_F=x \mathrm{~A}}$$
	- If it was saturated, simply replace $\left.V_\phi\right|_{\text {OCC, air-gap line }}$ with $\left.V_\phi\right|_{\text {OCC, actual curve }}$

![[Pasted image 20230309091303.png]]

