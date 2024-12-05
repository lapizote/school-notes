"Temperature" and "heat" have very different meanings (and should not be used interchangeably, regardless of how much it happens in regular language).

(Note that we will be focusing on large-scale or macroscopic objects).

### Temperature and Thermal Equilibrium
The temperature is a measure of "hotness" or "coldness", using a constructed temperature scale (i.e. we use a measurable property of a material that varies with "hotness" or "coldness").

In a lab, we have two typical types of thermometers:
- A liquid mercury thermometer (changes in temperature causes the liquid's volume to change)
- A pressure thermometer (changes in temperature causes the gas' pressure to change)

Two systems are in thermal equilibrium if and only if they have the same temperature.

Consider three systems A, B, and C:
![[Figure17.2.PNG]]

Note that A and B are separated by an insulator. When $A=C$ and $B=C$, then $A=B$.

#### Zeroth Law of Thermodynamics
This is the zeroth law of thermodynamics. If $C$ is initially in thermal equilibrium with both $A$ and $B$, then $A$ and $B$ are in thermal equilibrium with each other.

---
### Temperature Scales
- Celsius -> 0$^\circ$C is the freezing point of pure water and 100$^\circ$C is the boiling point
- Fahrenheit -> 32$^\circ$F is freezing point of pure water and 212$^\circ$F is the boiling point
#### Gas Thermometer and the Kelvin Scale
Ideally, we should define a temperature scale that does not depend on the properties of a particular material. A gas thermometer is close to ideal, as it uses the principle ($pV = nRT$) that the pressure of a gas at a constant volume increases with temperature

![[Figure17.5.PNG]]

Note that all the pressure lines all intersect at one point (extrapolated to zero pressure), this is equivalent to 0 K (-273.15$^\circ$C)

Remember that the Celsius scale has two fixed points --- normal freezing and boiling temperatures of H$_2$O. We define the Kelvin scale using a gas thermometer with only a single reference temperature.

We define the ratio of two temperatures $T_1$ and $T_2$ on the Kelvin scale as the ratio for the corresponding gas-thermometer pressures:
$$
\frac{T_2}{T_1} = \frac{p_{2}}{p_{1}}
$$
We specify the Kelvin temperature of a single specific state: triple point of water (pressure and temperature at which solid, liquid, and vapor water can all coexist). This occurs at 0.01$^\circ$C (273.16 K) and water-vapor pressure of 610 Pa (~0.006 atm)
#### Temperature Conversions
$$
\begin{align}
T_F = \frac{9}{5}T_C + 32^\circ \\
T_C = \frac{5}{9}(T_F - 32^\circ) \\
T_K = T_C + 273.15
\end{align}
$$
---
### Thermal Expansion
Most materials tend to expand when their temperatures increases.

Consider a rod of length $L_o$. Increasing the temperature of this rod causes it to expand, such that $\Delta T$ corresponds to $\Delta L$. 

![[Figure17.8.PNG]]

The change in length is given by
$$
\Delta L = aL_o\Delta T
$$
where $\alpha$ is the coefficient of linear expansion of the material. Note that this is only an approximate relationship, such that it only holds for "small" $\Delta T$ ($\leq$ 100$^\circ$C or so)

#### Molecular model for Thermal Expansion
We can understand the linear expansion if we model the atoms as being help together by springs (interatomic forces modeled as spring forces). Each atom would vibrate about its equilibrium position, where the energy and amplitude of vibration increases with temperature. When the amplitude increases, the average distance between atoms also increases.

#### Volume Expansion
Thermal expansion also applies to liquid materials. If $\Delta T$ is not high, then the increase in volume $\Delta V$ is given by
$$
\Delta V = \beta V_o\Delta TC
$$
There is a simple relationship between $\beta$ and $\alpha$ for solid materials. Consider a cube of material with side length $L$ and volume $V = L^3$.

At the initial temperature, $V = V_o$ and $L = L_o$. When temperature increases by dT, side length should increase by dL and the volume increases by an amount dV, such that
$$
dV = \frac{dV}{dL}dL = 3L^2dL
$$
We replace $L$ and $V$ by their initial values such that dL is expressed as
$$
dL = \alpha L_o dT
$$
Since $V_o = L_o^3$, dV can also be expressed as
$$
dV = 3L_o^2\alpha L_odT = 3\alpha V_odT
$$
This is consistent with $dV = \beta V_odT$ only if
$$
\beta = 3\alpha
$$

#### Coefficients of Expansion
![[Table17.1.PNG]]

Note that the coefficient has a unit of $K^{-1}$ such that it is consistent with dimensional analysis.

#### Thermal Expansion of Water
Water is a special substance, because between 0$^\circ$C and 4$^\circ$C, water decreases in volume with increasing temperature (such that water is most dense at 4$^\circ$C). Because of this behavior, lakes freeze from the top down instead of from the bottom up.

#### Thermal Stress
Consider an aluminium rod. If the temperature changes but is not allowed to expand or contract (e.g. clamped on both ends), then thermal stress develops.

Engineers account for thermal stresses when designing structures (e.g. for concrete highways, gaps are made to allow for expansion and contraction of concrete)

#### Calculating the Thermal Stress in a Clamped Rod
From the definition of Young's modulus:
$$
Y = \frac{\frac{F}{A}}{\frac{\Delta L}{L_o}}
$$
so
$$
(\frac{\Delta L}{L_o})_\text{thermal} = \frac{F}{AY}
$$
If the length is to be constant, then the total fractional change in length must be zero such that
$$
\left( \frac{\Delta L}{L_o} \right)_\text{thermal} + \left( \frac{\Delta L}{L_o} \right)_\text{tension} = \alpha\Delta T + \frac{F}{AY} = 0
$$

Then the tensile stress needed to keep the length constant:
$$
\frac{F}{A} = -Y\alpha\Delta T
$$

---
### Quantity of Heat
Energy transfer that takes place because of a temperature difference is called heat flow or heat transfer. Note that heat refers to the energy that is transferred or energy in transit due to a temperature difference, NOT the amount of energy contained within a particular system.

Meanwhile, temperature a quantitative description of the hotness and coldness of a material (a measure of the average translational kinetic energy associated with the disordered microscopic motion of atoms and molecules.)

![[Figure17.15.PNG]]

The temperature of the body can be changed by either doing work on it or by adding heat to it.

Unit of Heat: calorie is defined as the amount of heat required to raise the temperature of 1 gram of water from 14.5$^\circ$C to 15.5$^\circ$C

#### Specific Heat
The heat required for temperature change $\Delta T$ of mass $m$ is
$$
Q = mc\Delta T
$$
where $c$ is called the specific heat of the material.
For an infinitesimal temperature change $dT$ and corresponding quantity of heat $dQ$:
$$
dQ = mc\,\,dT
$$
![[Figure17.17.PNG]]

Notice that the unit of $c$ is J/kg K

The specific heat of water is approximately 4190 J/kg K or 1 cal/g C$^\circ$.

![[Table17.3.PNG]]

#### Molar Heat Capacity
Sometimes it is more convenient to describe a quantity of substance in terms of the number of moles $n$ rather than the mass $m$ of a material. The total mass $m$ of a material is now given by
$$
m = nM
$$
where $M$ is the molar mass (kg/mol) and $n$ is the number of moles.
$$
\begin{align}
Q = mc\Delta T &= nMc\Delta T \tag{$Mc$ = molar heat capacity} \\
Q &= nC\Delta T \tag{for $n$ moles}
\end{align}
$$

---
### Phase Changes
A phase refers to the specific state of matter (solid, liquid, gas), and a phase change would then be a transition from one phase to another.

In any given pressure, it would take a specific temperature for phase change to start occurring.

During a phase change, the temperature does not change until the phase change finishes, as the heat change is allocated to the phase change rather than to change the temperature.

This is defined through the heat of fusion and heat of vaporization:
- Heat of fusion, $L_f$ - heat per unit mass that is transferred in a solid-liquid phase change
	- For H$_2$O at atm: $L_f = 3.34 \times 10^5$ J/kg = 79.6 cal/g
- Heat of vaporization, $L_v$ - heat per unit mass that is transferred in a liquid-gas change.
	- For H$_2$O at atm: $L_V = 2.256 \times 10^6$ J/kg = 539 cal/g

![[Figure17.20.PNG]]

![[Table17.4.PNG]]



