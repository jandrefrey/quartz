---
title: "Closed Loop Frequency Response"
---
If we assume an open loop transfer function as part of a closed loop system, we can generate the bode plot for that system.
![[Pasted image 20230809120645.png]]
At low frequencies we expect the closed loop system to have a frequency of 1. (tracking input). 
**Bandwidth** is the frequency at which the closed loop system magnitude fails to follow magnitude of input signal. Magnitude = 0.7 (-3dB). It is the limit of input frequencies our system can track accurately.
$$\omega_{BW} \approx \omega_n$$
$$\omega_n < \omega_{BW} < 2\omega_n$$
**Resonant peak, $M_r$** is where the amplitude of the closed loop system exceeds the amplitude of the input signal. It happens just before the bandwidth.