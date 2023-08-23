---
title: "Transformers"
---
## Ideal Transformers
A transformer changes one AC voltage level to another voltage level at the same frequency without affecting the power transferred. So for an ideal transformer: $P_{in}=P_{out}$
![[Pasted image 20230413100454.png|450]]

From Faraday's law:
$$\frac{V_P}{V_S}=a$$
and
$$\frac{I_P}{I_S}=\frac 1 a$$
Where a is the **turns ratio($\frac{N_P}{N_S}$)**

### Dot Convention
- If the primary voltage is positive at the dotted end of the winding, then the secondary voltage will be positive at the dotted end too.
- If the primary current of the transformer flows into the dotted end of the primary winding, the secondary current will flow out of the dotted end of the secondary winding
### Impedance
On the Load:
$$Z_L = \frac{V_S}{I_S}$$
However, since the ratio of current and voltage is changed by the transformer, the **apparent impedance** of the primary circuit is:
$$Z_L'= a^2Z_L$$
By replacing the transformers with equivalent circuits as above, we can calculate the values of the other parts of the circuit.
Then we can use these equations again to find the transformer values.
	This is called **referring** 
## Real single-phase transformers
### Transformer Losses
- Copper Losses (modelled as series resistor $R_P$ and $R_S$)
- Core Losses (Eddy current and hysteresis) (modelled as shunt resistor $R_C$)
- Magnetizing current to establish the flux in the core (modelled as a shunt inductance $X_m$)
- Leakage flux (modelled as series inductances $X_p$ and $X_s$ respectively)
![[Pasted image 20230413111638.png]]
We can simplify this by reflecting either of the two sides:
Referred to LV side:
![[Pasted image 20230413113023.png|350]]
Referred to HV side:
![[Pasted image 20230413113030.png|350]]
### Parameters
Since the leakage flux and reluctance are relatively small:
$$\frac{V_P}{V_S}\approx a$$
and 
$$\frac{I_P}{I_S}\approx \frac 1 a$$

#### Transformer impedances
Open circuit test: (Find $R_c$ and $X_m$)
![[Pasted image 20230413114250.png|300]]
$$
\begin{aligned}
& Q_{o c}=\sqrt{\left(V_{o c} I_{o c}\right)^2-P_{o c}^2} \Rightarrow R_c^{\prime}=\frac{V_{o c}^2}{P_{o c}} ; X_m^{\prime}=\frac{V_{o c}^2}{Q_{o c}} \text {, or } \\
& I_c=\frac{V_{o c}}{R_c^{\prime}} \text { and } I_m=\sqrt{I_{o c}^2-I_c^2} \Rightarrow X_m^{\prime}=\frac{V_{o c}}{I_m}
\end{aligned}
$$

Short-circuit Test (Find $R_{eq}$ and $X_{eq}$)
![[Pasted image 20230413114444.png|300]]
$$
Z_{e q}=\frac{V_{s c}}{I_{s c}} \Rightarrow R_{e q}=\frac{P_{s c}}{I_{s c}^2}
$$
$$X_{e q}=\sqrt{Z_{e q}^2-R_{e q}^2}$$

## Voltage Regulation
Voltage Regulation (VR) compares the output voltage of the transformer at no load with the output voltage at full load while the input voltage is kept constant at a value corresponding to the full load condition
$$\begin{aligned}
V R & =\frac{V_{s(N L)}-V_{s(F L)}}{V_{s(F L)}} \times 100 \% \\
& =\frac{V_p^{\prime}-V_{s(F L)}}{V_{s(F L)}} \times 100 \% \\
& =\frac{V_{p, p u}-V_{s(F L), p u}}{V_{s(F L), p u}} \times 100 \%
\end{aligned}$$


## Efficiency
$$P_{\text {out }} =P_s=V_s I_s \cos \left(\theta_s\right)$$

$$P_{\text {in }} =P_s+P_{\text {losses }}=V_s I_s \cos (\theta)+P_{\text {core }}+P_{c u}$$
Then:
$$\eta =\frac{P_{\text {out }}}{P_{\text {in }}}=\frac{V_s \cos \left(\theta_s\right)}{V_s I_s \cos (\theta)+P_{\text {core }}+P_{\text {cu }}} \times 100 \%$$