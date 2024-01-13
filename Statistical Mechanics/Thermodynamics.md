# Introduction


Thermodynamics is the phenomenological(based on physical observations) description of properties of macroscopic systems in thermal equilibrium.

- Idealise the system. First examine closed, isolated system and then move onto open and interacting systems.
- A State function is a thermodynamic coordinate that describes the state of system. They are valid only when the system is in equilibrium w.r.t a given observation time scale. The dependence on an observation time scale makes equilibrium a subjective quantity.
- The relationship between these state functions is described by the Laws of Thermodynamics and their mathematical framework, which are based on empirical observations and more fundamental laws (microscopic) are needed for their justification.

# Zeroth Law


[Insert image of zeroth law]

> If two systems A and B are in equilibrium with a third system C, then they are also in equilibrium with each other.

It is assumed that each system is separately in mechanical equilibrium. If systems are allowed to work on each other then additional constraints must be put to describe their joint mechanical equilibrium.

We can describe a constraint equation b/w A, C and B, C and from the Zeroth Law this constraint must also exist b/w A,B. This gives us the definition of _empirical temperature_ *T*. There can be many potential choices of what this constraint might be but the essential idea is the existence of such a function itself.

Isotherms of a system are described by the constraint $$T = const.$$
### Ideal Gas Temp Scale 

Ideal gas is _dilute limit_ of a real gas and from empirical observations, we see that the product of Pressure and Volume remain constant along an isotherm of such ideal gas. We can describe the Kelvin temperature scale using the ideal gas. 
- 0K is the temperature at which the ideal gas attains 0 volume.
- The ideal gas temperature is proportional to PV and at 273.16K, $$PV_{system}=PV_{triple-point-of-water}$$
- Hence, $$T=273.16\frac{PV_{system}}{PV_{triple-point-of-water}}$$

# First Law 


This is essentially the statement of **Conservation of Energy** for thermodynamic systems.
> The change in internal energy U of a system is due to the heat supplied Q and the work done W on the system.

$$\Delta U = \Delta Q + \Delta W$$

<details>
<summary>Convetional bullshit</summary>
The Work done $\Delta W$ is +ve when done <b><i>on the system</i></b>. Similarly the heat change $\Delta Q$ is heat supplied <i><b>to the system by a reservoir</b></i>.
</details>
### Quasi-Static Process

When a system has $\Delta Q=0$, it is said to be *adiabatically isolated*

We can change the state of the system by external work given that the sources of energy are only of mechanical origin, i.e. for an adiabatically isolated system, the work required only depends on the initial and final states and not on the path required to reach the final state. However when the system is not isolated, the total change in internal energy depends on both the work done and heat supplied. This means that work and heat are themselves no longer state functions as they depend on the means of production of work and not just on final states. W and Q depend on path, we can therefore represent first law as, $$dU=đQ+đW$$

Internal energy is a state function and can be obtained via differentiation. Let $X_i$ be thermodynamic coordinate, then $dE=\sum_{i} \partial_i E dX_i$.

*Quasi-Static Process* is performed sufficiently slowly so that the system is infinitesimally close to equilibrium at all times. In such a process the thermodynamic coordinates exist and in principle can always be computed. We can divide statefucntion into a set of *generalised displacement* **$x_i$** and a their conjugate  *generalised forces* **$J_i$**, which for a quasi-static process will give, $$đW=\sum_i J_i dx_i$$ 

The displacements are generally _extensive_ properties (they scale with the size of the system) while the forces are _intensive_ properties (they are inherent to the system). The uniformity of generalised forces, e.g. Pressure exerted on the wall of a gas chamber (without any external potential), is an indicator of equilibrium. Similarly Temperature is also a generalised force, with Volume of the system acting as a generalised displacement (also for Pressure).

### Response Functions

Usual methods for characterising the macroscopic behaviour of a system are _Response functions_, these are experimentally measured using external probes. Some common response functions are, 

* *Heat capacities* describe the relationship between the change of temperature and heat supply to the system. Heat is not a state function hence the path must be satisfied,
	- When volume is kept constant $W=PdV=0$, $$C_v=\left. \frac{dQ}{dt}\right|_v = \left. \frac{\partial U}{\partial T}\right|_v $$
	- When pressure is kept constant, $$C_p=\left. \frac{dQ}{dt}\right|_p=\left. \frac{\partial U}{\partial T}\right|_p+\left. P\frac{\partial V}{\partial T}\right|_p$$
	- Since U is only a function of temperature, $$C_p-C_v=\left. P\frac{\partial V}{\partial T}\right|_p=Nk_b$$

* *Force constants* are a infinitesimal ration of displacements to force and are generalisation of spring constant. e.g. isothermal compressibility, magnetic susceptibility, etc.
* *Thermal responses* describe the change in thermodynamic coordinate w.r.t temperature. 

# Second Law


### Heat Engine

An idea _heat engines_ take $Q_H$ amount of heat from a reservoir and do work $W$ and reject $Q_C$ amount of heat to a sink. An ideal *refrigerator* work in the opposite way, they perform work $W$ on the system to extract heat $Q_C$ from a cold system and dumping $Q_H$ to a hotter system/exhaust. 

[insert image of heat engine]

**Kelvin's statement** 
>No process is possible whose sole result is conversion of heat into work.

**Clausius's statement**
>No process is possible whose sole result is transfer of heat from a colder to hotter body.
<define>
</define>
<details>
<summary> Equivalence of the two statements </summary>
The two statements of second law are equivalent to each other. <br>
One can prove this by assuming one of the statement to be false and creating an machine as such. We can then attach that machine to its conjugate machine (heat engine and refrigerator are conjugate of each other) and show that the other statement is also violated, proving that both statements are equivalent.
</details>

**Efficiency of a heat engine**: It is the work done by an engine per unit heat supplied by the reservior.
$$\eta=\frac{W}{Q_H}$$
Since $W = Q_H-Q_C,\ \ \eta<1$ 

For reservoir of temperature $T_H$ and sink of temperature $T_C$, and from the fact that $Q \propto T$:
$$\eta=1-\frac{T_C}{T_H}$$
### Carnot Engine

