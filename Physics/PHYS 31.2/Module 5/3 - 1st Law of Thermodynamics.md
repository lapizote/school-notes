### Thermodynamic Systems
We must define clearly what is and is not included in the thermodynamic system. The state of the thermodynamic system changes when it goes through a thermodynamic process.

---
### 1st Law of Thermodynamics
$$
\Delta U = Q-W
$$
where $U$ refers to the internal energy, $Q$ is heat, and $W$ is work done by the system.

#### Work Done During Volume Changes
Consider the work done by the system during a volume change.

![[Figure19.4.PNG]]

When a gas expands, it pushes outward on its boundary surfaces as they move outward. An expanding gas always does positive work.

Let
$A$: Cross sectional area of the cylinder
$p$: pressure exerted by the system at the piston face
$F = pA$: is the total force exerted by the system on the piston



When the piston moves a distance $dx$, then the work $dW$ by this force is:
$$
dW = F \, dx = pA \, dx
$$
But remember that
$$
A \, dx = dV \tag{infinitesimal change in volume}
$$
The work done by the system in this small volume change:
$$
dW = p \, dV
$$
In a finite volume change from $V_1$ to $V_2$:
$$
W = \int_{V_1}^{V_2} p \, dV
$$
In general, the pressure of the system may vary during the volume change. Let us try to find how the pressure varies as a function of volume using a pV-diagram (i.e. use the work formula to find the area under the pV curve):

![[Figure19.6.PNG]]

#### Paths Between Thermodynamic States
When a thermodynamic system changes from an initial state to a final state, it passes through a series of intermediate states (paths).

![[Figure19.7-1.PNG]] ![[Figure19.7-2.PNG]]

This shows us that the work done by the system depends not only on the initial and final states, but also the intermediate states (i.e. the path)

#### Internal Energy and the First Law of Thermodynamics
Internal energy refers to the sum of the kinetic energies of all the particles in a system, plus the sum of all the potential energy of interaction among particles.

Let $U$ be the internal energy of a thermodynamic system. Then $\Delta = U_2 - U_1$ is the change in internal energy.

There are two possible ways to change the internal energy of a system:
- Add/remove heat from the system
- Let the system do work or do work on the system

Then:
$$
\Delta U = Q - W
$$
or
$$
Q = \Delta U + W
$$
(Note that $W$ refers to work done by the system)

The first law of thermodynamics gives us an operational definition of the change in internal energy of a system.

In a thermodynamic process, the internal energy may:
- Increase ($\Delta U > 0$)
- Decrease ($\Delta < 0$)
- Remain the same ($\Delta = 0$)

Note that while $Q$ and $W$ are depends on the path, $\Delta U = Q - W$ is independent of the path.

---
### Cyclic Processes and Isolated Systems
A cyclic process is a process that returns the system to its initial state.

![[Figure19.11.PNG]]

---
### Types of Thermodynamic Proceses
#### Adiabatic Process
No heat transfer into or out of a system (such that Q = 0).
This can be accomplished by surrounding the system with thermally insulating material, or carrying out the process very swiftly such that there is not enough time for appreciable heat flow.
$$
U_2 - U_1 = \Delta U = -W
$$
#### Isochoric Process
Constant volume process.
When the volume of a system is constant, it does no work on its surroundings (W = 0)
$$
U_2 - U_1 = \Delta U = Q
$$

#### Isobaric Process
Constant pressure process.
In this case, $\Delta U$, $Q$, and $W$ are not zero, but $W$ would then be straightforward:
$$
W = p(V_2-V_1)
$$

#### Isothermal Process
Constant temperature process.
For a process to be isothermal, heat flow into or out of a system must occur slowly enough that thermal equilibrium is maintained.

---
### Internal Energy of an Ideal Gas
![[Figure19.17.PNG]]

Many experiments have shown that when a low-density gas undergoes a free expansion, its temperature does not change. This gas is essentially an ideal gas.

The internal energy of an ideal gas depends only on its temperature, not pressure nor volume.

#### Heat Capacities of an Ideal Gas
Heat capacities may be measured at a constant volume ($C_v$) or constant pressure ($C_p$).

Consider: $C_v$ and $C_p$ for an ideal gas.

At constant volume: $W = 0$
$$
Q = \Delta U
$$
At constant pressure:
$$
Q = \Delta U + W
$$

For a given temperature increase, $\Delta U$ of an ideal gas has the same value no matter the process ($U \propto T$ only). Essentially, $Q$ input at a constant pressure > $Q$ input at constant volume.

![[Figure19.19.PNG]]

Raising the temperature of an ideal gas from $T_1$ to $T_2$ by a constant-volume or a constant-pressure process. For an ideal gas, $U$ depends only on $T$, so $\Delta U$ is the same for both processes.

But for the constant-pressure process, more heat $Q$ must be added to both increase $U$ and do work $U$. Hence, $C_p > C_v$ (for air, $C_p$ is 40% greater than $C_v$).

#### Relating $C_p$ and $C_v$ for an Ideal Gas
Consider the constant volume process:
$$
dQ = nC_v \, dT
$$
$dW = 0$ as $V$ is constant.

We can take the first law in a different form:
$$
dQ = dU+ dW
$$

Now consider the constant pressure process:
$$
dQ = nC_p \, dT
$$
The work $dW$ done on the gas in terms of the ideal gas equation:


Finally, we get the relationship:
$$
C_p = C_v + R
$$

---
### Ratio of Heat Capacities
$$
\gamma = \frac{C_p}{C_v} = \frac{C_v + R}{C_v}
$$
e.g. for ideal diatomic gas:
$$
C_v = \frac{5}{2}R
$$
Thus
$$
C_p = C_v + R = \frac{5}{2}R + R = \frac{7}{2}R
$$
and
$$
\gamma = \frac{C_p}{C_v} = \frac{\frac{7}{2}R}{\frac{5}{2}R} = \frac{7}{5} = 1.40
$$
Remember that for an ideal gas:
$$
\Delta = nC_v\Delta T \tag{regardless if volume is constant}
$$

---
### Adiabatic Processes for an Ideal Gas
![[Figure19.20.PNG]]

As the gas expands from $V_a$ to $V_b$, it does postivie work $W$ on its environment, its internal energy decreases (as $\Delta = -W < 0$), and its temperature drops from $T+dT$ to $T$.

An adiabat at any point is always steeper than the isotherm passing through the same point.

Note:
- adiabatic heating -> raising the temperature
- adiabatic cooling -> lowering the temperature
- Heat $\neq$ Temperature
- In an adiabatic process, the temperature change is due to work done by or on the system, which means that there is no heat flow at all.

#### Relating V, T, and p
The change in internal energy of an ideal gas for any process is:
$$
dU = nC_vdT
$$
And the work done by an ideal gas is
$$
dW = pdV
$$

Then during an adiabatic process where $dQ = 0$:
$$
dU = dQ - dW = -dW
$$

Therefore:
$$
\begin{align}
nC_vdT &= -pdV \\
n_CvdT &= -\frac{nRTdV}{V} \\
\frac{dT}{T} + \frac{R}{C_v} \frac{dV}{V} &= 0
\end{align}
$$
Remember that
$$
\frac{R}{C_v} = \frac{C_p-C_v}{C_v} - 1 = \gamma -1
$$
so
$$
\begin{align}
\frac{dT}{T} + (\gamma-1) \frac{dV}{V} &= 0 \\
\ln T + (\gamma-1) \ln V &= a \tag{$a$ refers to a constant} \\
\ln T + \ln V^{\gamma - 1} &= a\\
\ln(TV^{\gamma-1}) &= a \\
TV^{\gamma - 1} &= b \tag{new constant $b$}
\end{align}
$$
Then, for an initial state of $(T_1, V_1)$ and a final state of $(T_2, V_2)$:
$$
T_1V_1^{\gamma-1} = T_2V_2^{\gamma-1}
$$
Now remember that
$$
T = \frac{pV}{nR}
$$
so
$$
\begin{align}
TV^{\gamma-1} &= a \\
\frac{pVV^{\gamma-1}}{nR} &= a \\
pV^\gamma &= b
\end{align}
$$Then we have
$$
p_1V_1^\gamma = p_2V_2^\gamma
$$
$$
W = nC_v(T_1-T_2)
$$