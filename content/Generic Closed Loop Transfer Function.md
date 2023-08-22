---
title: "Generic Closed Loop Transfer Function"
---
![[Pasted images/Pasted image 20230801213310.png]]
- Reference Input: $R(s)$
- Disturbances: $W(s)$
- Sensor Noise: $V$
- Output: $Y(s)$
- Control Signal: $U(s)$
- Error: $E(s)$

> **Transfer Function**
> $$Y=\frac{GD}{1+GD}R+\frac{G}{1+GD}W\:-\frac{GD}{1+GD}V$$

## Sensitivity
Effect of change to one parameter with change in another parameter.
In our case: Effect of change to transfer function gain with change to a specific parameter.
$$S_{k}{}^{T}=\frac{k}{T}\frac{dT}{dk}$$
where:
- $k$ is a system parameter
- $T$ is the transfer function