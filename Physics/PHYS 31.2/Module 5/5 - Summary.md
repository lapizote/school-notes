### Common Constants
$$
\begin{align}
N_A &= 6.02\times 10^{23} \tag {avogadro's constant} \\
R &= 8.314 \, \text{J/mol K} \tag{ideal gas} \\

\end{align}
$$
### 1 - Temperature and Heat
##### Kelvin-Celsius Conversion:
$$
T_K = T_C + 273.15
$$
##### Linear and Volume Expansion:
$$
\Delta L = \alpha L_o\Delta T \quad \text{and} \quad \Delta V = \beta V_o\Delta T \tag{where $3\alpha = \beta$}
$$
##### Tensile Strength-Expansion Relation
$$
\frac{F}{A} = -Y\alpha\Delta T
$$
##### Specific Heat
$$
Q = mc\Delta T \quad \text{and} \quad Q = nC\Delta T \tag{$C$ is molar specific heat}
$$

### 2- Thermal Properties of Matter
##### Ideal gas law:
$$
pV = nRT = NkT
$$
(where the latter is expressed on a per-molecule basis)

##### Average translational kinetic energy of $n$ moles of ideal gas:
$$
K_\text{tr} = \frac{3}{2}nRT
$$
##### Average translational kinetic energy of a gas molecule:
$$
\frac{1}{2}m(v^2)_\text{av} = \frac{3}{2}kT
$$
(note that $m$ refers to the mass of a single molecule)

##### Root mean-square speed of a gas molecule:
$$
\begin{align}
v_\text{rms} &= \sqrt{(v^2)_\text{av}} \\
&= \sqrt{\frac{3kT}{m}} = \sqrt{ \frac{3RT}{M} }
\end{align}
$$
##### Molar specific heat (constant volume):
$$
\begin{align}
C_v &= \frac{3}{2}R = 12.47 \, \text{J/mol K} \tag{ideal gas of point particles} \\
C_v &= \frac{5}{2}R = 20.79\,\text{J/mol K} \tag{diatomic gas, including rotation} \\
C_V &= 3R = 24.9 \text{J/mol K} \tag{Rule of Dulong and Petit}
\end{align}
$$
### 3 - 1st Law of Thermodynamics
##### 1st Law of Thermodynamics (Internal Energy $U$):
$$
\Delta U = Q-W
$$
##### Work done (pV graph)
$$
W = \int_{V_1}^{V_2} p \, dV \tag{or area under the pV curve}
$$
(Note: Internal Energy $U$ is independent of path taken)

##### Adiabatic Process:
No heat transfer into or out of a system (such that Q = 0).
$$
U_2 - U_1 = \Delta U = -W
$$
###### Isochoric Process:
Constant volume process.
When the volume of a system is constant, it does no work on its surroundings (W = 0)
$$
U_2 - U_1 = \Delta U = Q
$$

##### Isobaric Process:
Constant pressure process.
In this case, $\Delta U$, $Q$, and $W$ are not zero, but $W$ would then be straightforward:
$$
W = p(V_2-V_1)
$$

##### Isothermal Process:
Constant temperature process.
For a process to be isothermal, heat flow into or out of a system must occur slowly enough that thermal equilibrium is maintained.

##### Heat Capacities
Heat capacities can be measured for constant volume or constant pressure ($C_v$ vs $C_p$).

##### Constant Volume and Pressure Relation
$$
C_p = C_v + R
$$
##### Ratio of Heat Capacities
$$
\gamma = \frac{C_p}{C_v} = \frac{C_v+R}{C_v} = 1 + \frac{R}{C_v}
$$
##### Change in Internal Energy for Ideal Gases:
$$
dU = nC_vdT
$$
##### Adiabatic Process in Ideal Gas:
$$
T_1V_1^{\gamma-1} = T_2V_2^{\gamma-1}
$$
$$
p_1V_1^\gamma = p_2V_2^\gamma
$$
$$
W = nC_v(T_1-T_2) = \frac{C_v}{R}(p_1V_1 - p_2V_2) = \frac{1}{\gamma - 1}(p_1V_1 - p_2V_2)
$$
### 4 - 2nd Law of Thermodynamics
The state of entropy of the entire universe will always increase over time.

##### Reservoirs:
$$
W = Q = Q_h + Q_c = |Q_h| - |Q_c|
$$
##### Thermal Efficiency:
$$
e = 1 + \frac{Q_c}{Q_h} = 1 - \left|\frac{Q_c}{Q_h}\right|
$$

##### Refrigerators:
$$
|Q_h| = Q_c + |W|
$$
##### Clausius Statement:
"Heat never flows spontaneously from lower temperature to higher temperature without work."

##### Carnot Engine:
Heat transfer in a Carnot Engine:
$$
\frac{Q_c}{Q_h} = -\frac{T_c}{T_h} \,\,\,\text{or}\,\,\, \frac{|Q_c|}{|Q_h|} = \frac{T_c}{T_h}
$$
Efficiency:
$$
e_\text{carnot} = 1-\frac{T_c}{T_h} = \frac{{T_h-T_c}}{T_h}
$$