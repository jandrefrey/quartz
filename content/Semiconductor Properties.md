---
title: "Semiconductor Properties"
---
- **Elemental semiconductors** - made from one element (group 4)
	- At 0K pure silicon is an insulator.
- **Compound semiconductors** - made from elements in groups 3 - 5
- The elements are bonded with covalent bonds
	- In order to break the covalent bonds the valence electrons must gain a minimum energy, known as **bandgap energy** ($E_g$ )
	- $E_g = E_v-E_c$ this region is called the forbidden bandgap
		- $E_v$ is the maximum valence energy and $E_c$ is the minimum conductance energy
- The greater the bandgap the less conductive
- A semiconductor has a bandgap of about 1eV
- A semiconductor has a neutral charge
- Two types of charged particles contribute to current:
	- Negatively charged free electrons
	- Positively charged holes


## Intrinsic Semiconductors
A single-crystal semiconductor with no other types of atoms within the crystal. 
Holes and Electron counts are equal.
$$n_{i}=BT^{3/2}e^{(\frac{-Eg}{2kT})}$$
- $n_i$  - Intrinsic carrier concentration. (concentration of free electrons.)
- $B$ - Material Specific Constant
- $E_g$ - Bandgap energy (eV)
- $k$ - Boltzmann Constant ($86\times 10^{-6} \frac{eV}{K}$) 

## Extrinsic Semiconductors
**Doping** allows control of the concentration of free semiconductors by adding impurities
- **Donor impurities** are elements which add electrons which are free to move. (**n-type**)
- **Acceptor impurities** are elements which add holes which can contribute to hole current. (**p-type**)
$$n_op_o = n_i^2$$
- $n_o$ - Thermal Equilibrium concentration of free electrons
- $p_o$ - Thermal equilibrium concentration of holes.
- $n_i$ - Intrinsic carrier concentration
- At 300K: 
	- $n_o \approx N_d$ 
		- $N_d$ - Donor Concentration
		- $p_{o}=\frac{n_{i}^{2}}{N_{d}}$
	- $p_o \approx N_a$
		- $N_a$ - Acceptor Concentration
		- $n_{o}=\frac{n_{i}^{2}}{N_{a}}$

Electrons in an n-type are called majority carriers as they outnumber holes, which are minority carriers
(and vice - versa)

## Drift and Diffusion Currents
Charged electrons and holes are referred to as carriers.
### Drift Current Density
Total Drift Current given by:
$$J = J_n + J_p = \sigma E = \frac E \rho$$
- $\sigma$ - Conductivity
- $\rho$ - Resistivity

In an **n-type** semiconductor, an electric field $E$ forces the electrons in the **opposite direction**.
$$v_{dn} = \mu_n E$$
- $v_{dn}$ - Drift Velocity
- $\mu_n$ - Electron mobility ($1350 \frac {cm^2}{Vs}$ )

$$J_n = en\mu_n E$$
- $n$ - Electron concentration
- $e$ - Electron Charge

In a **p-type** semiconductor, the electrons move in the **same direction**
$$v_{dp} = \mu_p E$$
- $v_{dp}$ - Drift Velocity
- $\mu_p$ - Hole mobility ($480 \frac {cm^2}{Vs}$ )

$$J_p = ep\mu_p E$$
- $p$ - Electron concentration
- $e$ - Electron Charge
### Diffusion Current Density
Particles from a region of high concentration to lower concentration.
$$J_n = eD_p \frac{dn}{dx}$$
- $J_n$ - Diffusion current density (electrons)
- $e$ - Magnitude of electronic charge
- $\frac{dn}{dx}$ - The gradient of electron concentration
- $D_n$  - Electron diffusion coefficient


$$J_p = -eD_p \frac{dp}{dx}$$
- $J_p$ - Diffusion current density (holes)
- $e$ - Magnitude of electronic charge
- $\frac{dp}{dx}$ - The gradient of hole concentration
- $D_p$  - Hole diffusion coefficient

Then the **Einstein Relation**:
$$\frac{D_n}{\mu_n} = \frac{D_p}{\mu_p} = \frac{kT}{e} = 0.026 V$$