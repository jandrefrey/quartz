---
title: "Modelling Electrical Systems"
---
1. Write fundamental FO ODE for each energy storage element.
	1. Capacitor: $C\dot e_C=I_C$
	2. Inductor: $L\dot I_L = e_L$
2. Use Kirchhoff's laws to express unknowns **in terms of dynamic variables ($e_c$ and $I_L$) and input variable.**
	1. Setup nodes around circuit and sum voltages to 0.
	2. Or current flow in and out of node and sum to 0.
3. Take a derivative of the equation if need be.

## Op-Amp
![[Pasted image 20230425152805.png|200]]
Output Voltage of Op-Amp: $$e_O=K(e_B-e_A)$$

### Ideal Op-Amp
- Input terminals draw negligible current.
- Voltage difference $e_B-e_A=0$
- Gain($K$) is infinite

## Electro-Mechanical Systems
If the Capacitance were to be a variable and not a fixed value, the above equation would not hold and instead we would have (By chain rule):
$$\frac{d}{dt}(Ce_C)=\dot C e_C + C\dot e_C = I_C$$
Then:
$$C_x \dot x e_C + C \dot e_C = I_C$$

where $C_x=\frac{dC}{dx}$, and $\dot x = \frac{dx}{dt}$

Then we can once again write $I_C$ in terms of input and variables. (Using Kirchhoff)
Finally we model the mechanical part of the system, and then we can replace the electrostatic force with the electric model, using work and energy:
$$F_{es}=0.5C_xe^2_C$$
