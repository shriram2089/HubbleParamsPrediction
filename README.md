# HubbleParamsPrediction
To analyze the universe's accelerated expansion by fitting a cosmological model to observational Hubble parameter data at various redshifts. The goal is to constrain the current density parameters of matter ( Ω 𝑚  ), curvature ( Ω 𝑘 ), and dark energy ( Ω Λ ), plot their marginalized probability distributions, and report uncertainties.

The universe's expansion is characterized by the Hubble parameter, 
𝐻
(
𝑧
)
H(z), which varies with redshift 
𝑧
z. The relationship is given by:

𝐻
(
𝑧
)
=
𝐻
0
[
Ω
𝑚
(
1
+
𝑧
)
3
+
Ω
𝑘
(
1
+
𝑧
)
2
+
Ω
Λ
]
1
/
2
H(z)=H 
0
​
 [Ω 
m
​
 (1+z) 
3
 +Ω 
k
​
 (1+z) 
2
 +Ω 
Λ
​
 ] 
1/2
 

where:

Ω
𝑚
Ω 
m
​
 : Current density parameter of matter (non-relativistic)
Ω
𝑘
Ω 
k
​
 : Current density parameter of curvature
Ω
Λ
Ω 
Λ
​
 : Current density parameter of dark energy
𝐻
0
H 
0
​
 : Current value of the Hubble parameter (given as 
73.04
±
1.04
73.04±1.04 km s
−
1
−1
  Mpc
−
1
−1
 )
𝐻
(
𝑧
)
H(z): Hubble parameter at redshift 
𝑧
z
The critical density of the universe, 
𝜌
cr
ρ 
cr
​
 , is given by:

𝜌
cr
=
3
𝐻
2
8
𝜋
𝐺
ρ 
cr
​
 = 
8πG
3H 
2
 
​
 

where 
𝐻
H is the Hubble parameter at the respective redshift and 
𝜌
𝑖
ρ 
i
​
  is the density of the 
𝑖
i-th component (i.e., matter, curvature, etc.).

Problem Statement:
Given a dataset containing the Hubble parameter at various redshifts along with associated errors, perform the following tasks:

Constrain and find the best fit values for 
Ω
𝑚
Ω 
m
​
 , 
Ω
𝑘
Ω 
k
​
 , and 
Ω
Λ
Ω 
Λ
​
 .
Plot the 1D and 2D marginalized probability distributions for these parameters.
Report uncertainties corresponding to the 1σ, 2σ, and 3σ confidence levels.
Methodology:
1. Data Preparation:
Load the dataset containing the Hubble parameter 
𝐻
(
𝑧
)
H(z) values and their associated errors at various redshifts.
2. Model Definition:
Define the Hubble parameter model 
𝐻
(
𝑧
)
H(z) as a function of redshift and the cosmological parameters 
Ω
𝑚
Ω 
m
​
 , 
Ω
𝑘
Ω 
k
​
 , and 
Ω
Λ
Ω 
Λ
​
 .
3. Likelihood Calculation:
Construct a likelihood function based on the given dataset and the model. The likelihood function should account for the errors in the observed 
𝐻
(
𝑧
)
H(z) values.
4. Parameter Estimation:
Use Markov Chain Monte Carlo (MCMC) methods to sample the parameter space and estimate the best fit values for 
Ω𝑚, Ω𝑘, and ΩΛ.
5. Marginalized Distributions:
Generate 1D and 2D marginalized probability distributions for the parameters.
Calculate and report the uncertainties corresponding to the 1σ, 2σ, and 3σ confidence levels.
