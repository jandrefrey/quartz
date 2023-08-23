---
title: "Solving Differential Equations"
---
## First order DE
### Standard form 
for all first order systems:
$$\tau \dot y + y = bu$$
$y$ is the output variable of interest
$u$ is the input variable
$b$ is the RHS coefficient.
$\tau$ is unit [time] for mechanical systems.
> For step response: $u(t)=A U(t) \text {, that is, } y_{\mathrm{ss}}=b A$
### Settling time
We can estimate the settling time as:
$$t_s=4\tau$$
## Second Order DE
$$a_2\ddot y +a_1\dot y +a_0 y = b_0 u(t)$$
The **characteristic roots** are:
$$r=\frac{-a_1 \pm \sqrt{a_1^2-4a_0}}{2a_2}$$
- Complex roots: underdamped system
- Real distinct Roots: overdamped
- Real equal roots: Critically damped
> if $r_1>0$, $x \rightarrow \infty$, the system is unstable
> if $r_1<0$ and $r_2<0$, $x \rightarrow c$, the system is stable.

**Damping Ratio**:
$$\zeta = \frac{a_1}{2\sqrt{a_0a_2}}$$
$\zeta>1$ : Overdamped
$\zeta=1$ : Critically damped
$0<\zeta<1$ : Underdamped system
$\zeta=0$: Undamped (free response)

**damped natural frequency**
$$\omega_d = \omega_n \sqrt{1-\zeta^2}$$

**natural frequency**
$$\omega_n = \sqrt \frac{a_0}{a_2}$$
The closer to the origin, the smaller the natural frequency.

**Standard form** of LTI Second order I/O equation:
$$\ddot y + 2\zeta \omega_n \dot y + w_n^2 y = b_0 u(t)$$
For underdamped: $b_0=w_n^2$ ??


Solutions to y (cases):
Real roots:
$$x(t) = c_1e^{p_1t} + c_2e^{p_2t}+\text{particular solution}$$
and for complex roots: 
$p= \alpha \pm j\beta$
$$x(t)=Ke^{\alpha t}cos(\beta t + \phi)+\text{particular solution}$$
## Characteristics
Step Response of an Underdamped system:
| Performance Criteria | Equation |
| :--- | :--- |
| Peak time, $t_p$ | $t_p=\frac{\pi}{\omega _n\sqrt{1-\zeta^2}}$ |
| Maximum overshoot, $M_{os}$ | $M_{os}=e^{\frac{-\zeta \pi}{\sqrt{1-\zeta^2}}}$ |
| Settling time to steady state, $t_{S}$ | $t_S=\frac{4}{\zeta \omega_n}$ |
| Period of oscillation, $T_{period}$ | $T_{period}=\frac{2pi}{\omega_n \sqrt{1-\zeta^2}}$ |
| Number of cycles to steady state, $N_{cycles}$ | $N_{cycles}=\frac{2\sqrt{1-\zeta^2}}{\pi \zeta}$ |

### Settling time
The system takes as infite time to settle, but we can define a "band" to be a settled position. Using a 5% settling time:
$$
|y(t)-y_{ss}|\leq 0.05(y_{ss}-y(0))
$$
$|y(t)-y_{ss}|$ is the displacement at time t
$0.05(y_{ss}-y(0))$ is 0.05 of the initial displacement

![[Step Response 2023-04-11 18.50.49.excalidraw]]

> Oscillation period:
> $T_d=\frac{2\pi}{\omega_d}$

### % overshoot
$$
M^\%_P=\frac{y_{max}-y_{ss}}{y_{ss}-y_0}
$$
We can use the graph (fig 4.15) to find the damping ratio from % overshoot.

### Max overshoot
$$M_{OS}=\frac{|y_{max}-y_{SS}|}{y_{ss}}$$

## Steps
1. find the I/O equation with [[Deriving differential equations of mechanical systems]]
2. Determine if it is a underdamped system.
3. Compare with **Standard Form**
4. Compute damping ratio ($\zeta$) and undamped natural frequency ($\omega_n$).
5. From here we can compute all the underdamped performance metrics required.

These only hold if the system is underdamped ($\zeta < 0$)
Not if it is overdamped ($\zeta > 1$), critically damped ($\zeta = 1$) or undamped ($\zeta = 0$)

![[Pasted image 20230509224840.png]]