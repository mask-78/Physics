# Introduction

Thermodynamics is the phenomenological(based on physical observations) description of properties of macroscopic systems in thermal equilibrium.

- Idealize the system. First examine closed, isolated system and then move onto open and interacting systems.
- A State funtion is a thermodynamic coordinate that describes the state of system. They are valid only when the system is in equilibrium w.r.t a given observation time scale. The dependence on an observation time scale makes equilibrium a subjective quatitiy.
- The relationship between these state functions is described by the Laws of Thermodynamics and their mathematical framework, which are based on emperical observations and more fundamental laws (microscopic) are needed for their justification.

# Zeroth Law

[Insert image of zeroth law]

> If two systems A and B are in equilibrium with a third system C, then they are also in equilibrium with each other.

It is assumed that each system is separately in mechanical equilibrium. If systems are allowed to work on each other then additional constraints must be put to describe their joint mechanial equilibrium.

We can describe a constaint equation b/w A, C and B, C and from the Zeroth Law this constraint must also exist b/w A,B. This gives us the definition of _emperical temerature_ *T*. There can be many potential choices of what this constraint might be but the essential idea is the existence of such a function itself.

Isotherms of a system are described by the constaint $$T = const.$$

### Ideal Gas Temp Scale 

Ideal gas is _dilute limit_ of a real gas and from emperical observations, we see that the product of Pressure and Volume remain constant along an isotherm of such ideal gas. We can describe the Kelvin temperature scale using the ideal gas. 
- 0K is the temperature at which the ideal gas attains 0 volueme.
- The ideal gas temperature is proportional to PV and at 273.16K, $$PV_{system}=PV_{triple-point-of-water}$$
- Hence, $$T=273.16*\frac{PV_{system}}{PV_{tpow}}$$

# First Law 
This is essentially the statement of **Conservation of Energy** for thermodynamical systems.
> The change in internal enrgy U of a system is due to the heat supplied Q and the work done W on the system.

$$\Delta U = \Delta Q + \Delta W$$

<details>
<summary>Convetional bullshit</summary>
The Work done $\Delta W$ is +ve when done <b><i>on the system</i></b>. Similarly the heat change $\Delta Q$ is heat supplied <i><b>to the system by a reservoir</b></i>.
</details>

### Quasi-Static Process
When a system has $\Delta Q=0$, it is said to be *adiabatically isolated*

We can change the state of the system by external work given that the sources of energy are only of mechanical origin, i.e. for an adiabatically isolated system, the work required only depends on the initial and final states and not on the path required to reach the final state. However when the system is not isolated, the total change in internal energy depends on both the work done and heat supplied. This means that work and heat are themselves no longer state functions as they depend on the means of production of work and not just on final states. W and Q depend on path, we can therefore represent first law as, $$dU=đQ+đW$$

Internal energy is a state function and can be obtained via differentiation. Let $X_i$ be thermodynamic coordinate, then $dE=\sum_{i} \partial_i E dX_i$.

*Quasi-Static Process* is performed sufficiently slowly so that the system is infitessimally close to equilibrium at all times. In such a process the thermodynamic coordinates exist and in principle always be computed. We can divide statefucntion into a set of *generalized displacement* **$x_i$** and a their conjugate  *generalized forces* **$J_i$**, which for a quasi-static process will give, $$đW=\sum_i J_i dx_i$$ 

The displacements are generally _extensive_ properties (they scale with the size of the system) while the forces are _intensive_ properties (they are inherent to the system). The uniformity of generalized forces, e.g. Pressure exerted on the wall of a gas chamber (without any external potential), is an indicator of equilibrium. Similarly Temperature is also a generalized force, with Volume of the system acting as a generalized displacement (also for Pressure).

### Response Functions
Usual methods for charecterizing the macroscopic behaiviour of a system are _Response functions_, these are experimentally measured using external probes. Some common response functions are, 

* *Heat capacities* describe the relationship between the change of temperature and heat supply to the system. Heat is not a state funtion hence the path must be satisfied,
	- When volume is kept constant $W=PdV=0$, $$C_v=\left. \frac{dQ}{\dT}\right|_v = \left. \frac{\partial U}{\partial T}\right|_v $$
	- When pressure is kept constant, $$C_p=\left. \frac{dQ}{\dT}\right|_p=\left. \frac{\partial U}{\partial T}\right|_p+\left. P\frac{\partial V}{\partial T}\right|_p$$
	- Since U is only a function of temperature $$C_p-C_v=\left. P\frac{\partial V}{\partial T}\right|_p=Nk_b$$.

* *Force constants* are a infinitesimal ration of displacements to force and are generalization of spring constant. e.g. isothermal compressibility, magnetic susceptibility, etc.
* *Thermal responses* describe the change in thermodynamic coordinate w.r.t temperature. 

# Second Law


















