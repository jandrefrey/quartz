---
title: "System Type"
---
Inputs can be approximated by polynomials: $\frac{1}{s^{k+1}}$
- Step (Position) Input: $\frac 1 s$
- Ramp (Velocity) Input: $\frac 1 {s^2}$
- Parabola (Acceleration) Input: $\frac 1 {s^3}$

**Type** = Order of polynomial input that a system can reasonably track (constant steady state error)

## Determining system type
### Reference tracking
- Receives a reference input.

$$Y=\frac{GD}{1+GD}R+\cancel{\frac{G}{1+GD}W}\:-\cancel{\frac{GD}{1+GD}V}$$
And then:
$$E=R-Y$$
Finally, from the final value theorem:
$$\begin{aligned}e_{ss}&=\lim_{s\to0}sE(s)\\\\e_{ss}&=\lim_{s\to0}s\big(R(s)-Y(s)\big);\quad R(s)=\frac{1}{s^{k+1}}\end{aligned}$$
### Disturbance Rejection
- System following a disturbance input.

$$Y=\cancel{\frac{GD}{1+GD}R}+\frac{G}{1+GD}W\:-\cancel{\frac{GD}{1+GD}V}$$
And then:
$$E=\cancel R-Y = -Y$$
Finally, from the final value theorem:
$$\begin{aligned}e_{ss}&=\lim_{s\to0}sE(s)\\\\e_{ss}&=\lim_{s\to0}s\big(-Y(s)\big);\quad W(s)=\frac{1}{s^{k+1}}\end{aligned}$$
Set $k = 0$, $k=1$, $k=2$ and compare with the **Error Constants** step, tamp and parabola.
## Error Constants
![[Pasted images/Pasted image 20230801215210.png]]
