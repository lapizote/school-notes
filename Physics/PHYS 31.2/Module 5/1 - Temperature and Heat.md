"Temperature" and "heat" have very different meanings (and should not be used interchangeably, regardless of how much it happens in regular language).

(Note that we will be focusing on large-scale or macroscopic objects).

### Temperature and Thermal Equilibrium
The temperature is a measure of "hotness" or "coldness", using a constructed temperature scale (i.e. we use a measurable property of a material that varies with "hotness" or "coldness").

In a lab, we have two typical types of thermometers:
- A liquid mercury thermometer (changes in temperature causes the liquid's volume to change)
- A pressure thermometer (changes in temperature causes the gas' pressure to change)

Two systems are in thermal equilibrium if and only if they have the same temperature.

Consider three systems A, B, and C:
//pic

Note that A and B are separated by an insulator. When $A=C$ and $B=C$, then $A=B$.

//pic

#### Zeroth Law of Thermodynamics
This is the zeroth law of thermodynamics. If $C$ is initially in thermal equilibrium with both $A$ and $B$, then $A$ and $B$ are in thermal equilibrium with each other.

### Temperature Scales
- Celsius -> 0$^\circ$C is the freezing point of pure water and 100$^\circ$C is the boiling point
- Fahrenheit -> 32$^\circ$F is freezing point of pure water and 212$^\circ$F is the boiling point
#### Gas Thermometer and the Kelvin Scale
Ideally, we should define a temperature scale that does not depend on the properties of a particular material. A gas thermometer is close to ideal, as it uses the principle ($pV = nRT$) that the pressure of a gas at a constant volume increases with temperature

//pic

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
### Thermal Expansion
Most materials tend to expand when their temperatures increases.

Consider a rod of length $L_o$. Increasing the temperature of this rod causes it to expand, such that $\Delta T$ corresponds to $\Delta L$. 

//pics of rod

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
There is a simple relationship between $\beta$ and $\alpha$ for solid materials. Consider a cube of material with side length $L$ and volume $V = L^3.

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
//pic

Note that the coefficient has a unit of $K^{-1}$ such that it is consistent with dimensional analysis.

#### Thermal Expansion of Water
Water is a special substance, because between 0$^\circ$C and 4$^\circ$C, water decreases in volume with increasing temperature (such that water is most dense at 4$^\circ$C). Because of this behavior, lakes freeze from the top down instead of from the bottom up.

#### Thermal Stress
Consider an aluminium rod. If the temperature changes but is not allowed to expand or contract (e.g. clamped on both ends), then thermal stress develops.

Engineers account for thermal stresses when designing structures (e.g. for concrete highways, gaps are made to allow for expansion and contraction of concrete)