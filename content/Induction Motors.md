---
title: "Induction Motors"
---
## Induced torque
![[Magnetic Fields#A moving wire near a magnetic field has a voltage induced on it.]]

## Speed
![[AC Machine Fundamentals#^1db4d6]]

Note that the rotor will always be moving slightly slower than the stator field, since the induced torque is dependant on the relative speed between the stator field and the rotor.
The difference between the synchronous speed and the rotor speed:
$$n_{slip}=n_{sync}-n_{rotor}$$
and the **percentage slip**:
$$s=\frac{n_{sync}-n_{m}}{n_{m}}\times100\%$$
Then, $n_m=(1-s)n_{sync}$

### Rotor electrical frequency
If the rotor was stationary, its frequency would match the stator freq.
If the rotor was moving at sync speed, its frequency would be 0.
	$$f_{re}=sf_{se}=\frac{P}{120}(n_{sync}-n_{m})$$


## Equivalent circuit
$$E_R=sE_{R0}$$
$$X_R=X_{R0}$$
![[Pasted image 20230420133901.png]]
By reffering to the primary side:
$$E_1=aE_{R0}$$
$$I_2=\frac{I_R}{a}$$
$$R_2=a^2R_R$$
$$X_2=a^2X_{R0}$$
## Power in Induction Motors
![[Pasted image 20230420143312.png]]
- $P_{\mathrm{SCL}}=3 I_1^2 R_1$
- $P_{\text {core }}=3 E_1^2 G_C$
- $P_{\mathrm{AG}}=P_{\mathrm{in}}-P_{\mathrm{SCL}}-P_{\text {cose }}=3 I_2^2 \frac{R_2}{\mathrm{~s}}$
- $P_{\mathrm{RCL}}=3 I_2^2 R_2$
- $P_{\mathrm{conv}}=3 I_2^2 R_2\left(\frac{1-s}{s}\right)=(1-s) P_{\mathrm{AG}}$
- $\tau_{ind}=\frac{P_{AG}}{\omega_{sync}}=\frac{P_{conv}}{\omega_{m}}$

![[Pasted image 20230501195945.png]]
### Torque Angle
$$\delta=\sigma_R+90\degree$$

