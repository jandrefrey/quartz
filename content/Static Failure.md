---
title: "Static Failure"
---
[[Failure Theory]]
## Failure modes
![[Pasted image 20230414100229.png|300]]
![[Pasted image 20230414100909.png]]

### Ductile Materials
#### Maximum Shear Stress (Tresca)
conservative, often used for design where higher reliability is desired
1. $\tau_{max}=max(|\frac{\sigma_1-\sigma_2}{2}|, \frac{\sigma_2-\sigma_3}{2}|, \frac{\sigma_1-\sigma_3}{2}|)$
2. Fail if $\tau_{max}\ge$ $\frac{S_y}{2}$
#### Distortion Energy (von Mises)
Often used for analysis where agreement with experimental data is desired.
**von Mises stress** (effective stress) given by:
For 3D:
$$
\sigma^{\prime}=\frac{1}{\sqrt{2}}\left[\left(\sigma_x-\sigma_y\right)^2+\left(\sigma_y-\sigma_z\right)^2+\left(\sigma_z-\sigma_x\right)^2+6\left(\tau_{x y}^2+\tau_{y z}^2+\tau_{z x}^2\right)\right]^{1 / 2}
$$
For 2D:
$$
\sigma^{\prime}=\left(\sigma_x^2-\sigma_x \sigma_y+\sigma_y^2+3 \tau_{x y}^2\right)^{1 / 2}
$$
In terms of principle:
$$
\sigma^{\prime}=\left(\sigma_A^2-\sigma_A \sigma_B+\sigma_B^2\right)^{1 / 2}
$$
1. Failure when $\sigma ' \ge S_y$
#### Ductile Coulomb-Mohr
For materials with different compressive and tension strengths:
$$\frac{\sigma_1}{S_t} - \frac{\sigma_3}{S_c} =1$$
### Brittle Materials
#### Maximum Normal Stress
1. Calculate Principle Stresses
2. Fail if larger than Ultimate stresses
	1. $max(|\sigma_1|, |\sigma_2|, |\sigma_3|)\ge S_u$
#### Brittle Coulomb-Mohr
very conservative in 4th quadrant.
Using **ultimate strength**
$\sigma_1 \geq \sigma_2 \geq 0 \quad \sigma_1=S_{u t}$
$\sigma_1 \geq 0 \geq \sigma_2 \quad \frac{\sigma_1}{S_{u t}}-\frac{\sigma_2}{S_{u c}}=1$
$0 \geq \sigma_1 \geq \sigma_2 \quad \sigma_2=-S_{u c}$

#### Modified Mohr
slightly conservative in 4th quadrant, but closer to experimental data.
![[Pasted image 20230414103141.png]]

## Fracture Mechanics
$$
K_I=\beta \sigma \sqrt{\pi a}
$$
where $\beta$ is found in Figures $5-25$ to $5-30$
$$
n=\frac{K_{I c}}{K_I}
$$
where $K_{I c}$ is found in Table $5-1$