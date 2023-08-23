---
title: "Free Vibrations"
---
Considering a spring-mass system:
![[Pasted images/Pasted image 20230731201134.png]]

The spring force:
$$
f_k(t)=k(\delta_st+x(t))
$$

Considering Newton's Laws:
$$
\begin{gathered}\sum F_x(t)=m\ddot{x}(t)\\\\mg-k(\delta_st+x(t))=m\ddot{x}(t)\end{gathered}
$$
Note that $k\delta_s t = mg$:
$$
m\ddot{x}(t)+kx(t)=0
$$

> Some other cases:
> - Shaft and Disk
> 	$$
> 	J\ddot{\theta}+k\theta=0
> 	$$
> - Simple Pendulum:
> 	$$
> 	\ddot{\theta}+\frac{g}{l}\theta=0
> 	$$

## Observational Solution
Guess initially:
$$
x(t)=A\sin(\omega_nt+\phi)
$$
$$
\dot{x}(t)=\omega_nA\cos(\omega_nt+\phi)
$$
$$
\ddot{x}(t)=-\omega_n^2A\sin(\omega_nt+\phi)
$$
Then the motion equation becomes:
$$
-m\omega_n^2A\sin(\omega_nt+\phi)=-kA\sin(\omega_nt+\phi)
$$
with **Natural Frequency**, $\omega_n = \sqrt{\frac k m}$

Substituting the Initial Conditions:
$$
\begin{aligned}A&=\frac{\sqrt{\omega_n^2x_0^2+v_0^2}}{\omega_n}\\\phi&=\tan^{-1}\frac{\omega_nx_0}{v_0}\end{aligned}
$$
Finally,
$$
x(t)=\frac{\sqrt{\omega_n^2x_0^2+v_0^2}}{\omega_n}\sin\left(\omega_nt+\tan^{-1}\frac{\omega_nx_0}{v_0}\right)
$$



## Analytical Solution
Considering [[Solving Differential Equations]]:

Assuming the solution has the form $x(t) = ae^{\lambda t}$:
$$
m\lambda^2ae^{\lambda t}+kae^{\lambda t}=0
$$
Thus the **characteristic equation**:
$$
m \lambda^2 + k = 0
$$
with roots: $\lambda = \pm \omega_n j = \pm j\sqrt{\frac k m }$
Thus:
$$
x(t)=a_1e^{j\omega_nt}+a_2e^{-j\omega_nt}
$$
Considering Euler relations:
$$
A\sin(\omega_nt+\phi)=A_1\sin(\omega_nt)+A_2\cos(\omega_nt)
$$

## Qualification of Vibration
Average value:
$$
\bar{x}=\lim\limits_{T\to\infty}\frac{1}{T}\int_0^Tx(t)dt
$$
And the **RMS-value**:
$$
x_{rms}=\left(\lim_{T\to\infty}\frac{1}{T}\int_0^Tx^2(t)dt\right)^{\frac{1}{2}}
$$
And on decibel scale:
$$
dB=10\log_{10}\left(\frac{x_{rms}}{x_{ref}}\right)^2=20\log_{10}\frac{x_{rms}}{x_{ref}}
$$
