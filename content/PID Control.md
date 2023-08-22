---
title: "PID Control"
---
## Proportional Control
Control signal is linearly **proportional to error signal**.
$$D(s)=\frac{U(s)}{E(s)}=k_P$$

- Increasing Proportional Gain ($k_p$)
	- Decrease steady state error (but never achieve zero error)
	- Allows faster system response
	- Decrease damping (increase overshoot and oscillation)
## Integral Control
Control signal is linearly proportional to **integral** of error signal.
$$\begin{aligned}u(t)&=\left.k_I\int_{t_0}^te(\tau)d\tau\right.\\D(s)&=\frac{U(s)}{E(s)}=\frac{k_I}s\end{aligned}$$

- Eliminate steady state error (no matter the value of $k_I$ )
- Introduce overshoot and oscillation

## Proportional + Integral (PI) Control
Faster response than pure integral control, but still achieving zero steady state error.
$$D(s)=k_P+\frac{k_I}s=\frac{k_Ps+k_I}s$$
## Derivative Control
Control signal is linearly proportional to **rate of change** of error signal.
$$\begin{aligned}u(t)&=k_D\frac{de(t)}{dt}\\D(s)&=\frac{U(s)}{E(s)}=k_Ds\end{aligned}$$

- Increase system stability
- Speed up transient response and reduce overshoot
- Amplifies noise and has very sharp response to changes
- Almost never used alone

Typical Implementation:
![[Pasted images/Pasted image 20230802081749.png|400]]
Alternative Implementation (Reduce sharp response):
![[Pasted images/Pasted image 20230802081821.png|400]]

## Proportional + Derivative (PD) control
When a fast system response is important, but it is not critical to have zero steady state error.
$$D(s)=k_Ds+k_P$$

## Proportional + Integral + Derivative (PID) control
Fast response and zero steady state error
$$D(s)={k_P}+\frac{k_I}s+k_Ds=\frac{k_Ds^2+k_Ps+k_I}s$$

----
![[Pasted images/Pasted image 20230802082037.png]]

## Tuning of parameters
2 Methods exist
Methods based on the fact that many systems exhibit a similar response to a step input
### 0.25 Decay Ratio
![[Pasted images/Pasted image 20230802082216.png]]

### Ultimate sensitivity
1. Start with just proportional control
2. Increase proportional gain until system is marginally stable 
	- define this gain as $K_u$
	- define period as $P_u$

![[Pasted images/Pasted image 20230802082421.png]]