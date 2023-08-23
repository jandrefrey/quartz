---
title: "Thevenin and Norton equivalent circuit"
---
# Thevenin and Norton equivalent circuit
## Thevenin equivalent circuit
![[Pasted image 20220404154356.png|350]]

## Norton equivalent circuit
![[Pasted image 20220404154714.png|350]]

## Steps to solve:
1. Find open circuit voltage (with any method: node, mesh, etc)
2. $\textbf{V}_t=\textbf{V}_{oc}$
3. Find short circuit current ()
4. $\textbf{I}_n = \textbf{I}_{sc}$
5. Find $Z$
	1. $Z_t = \frac{\textbf{V}_{oc}}{\textbf{I}_{sc}}$
	2. Or we can simplify circuit:
		1. Only independant sources
			Zero all independant sources
			==$V$ becomes SC, $I$ becomes OC==
		2. Dependant and indep. sources
			Zero only independant sources
			Test source:
				$Z_{dep} = \frac{V_{test}}{I_{test}}$

## Source Transformations
From [[Ohm's Law]]:
![[Pasted image 20220404160522.png|400]]


- ex
	- ![[Pasted image 20220404164010.png|400]]
	![[Pasted image 20220404164034.png|400]]