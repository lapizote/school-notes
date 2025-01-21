### Directions of Thermodynamic Processes
Thermodynamic processes that occur in nature are irreversible processes (e.g. flow of heat from a hot body to a cooler boy, free expansion of gas).

The second law of thermodynamics determines the preferred direction of such processes.

However, there are some idealized processes that would be reversible, where these reversible processes are very close (i.e. infinitesimally) to being in thermodynamic equilibrium with itself and its surroundings.

![[Figure20.1.PNG]]

---
### Heat Engines
These include gasoline engines, jet engines, steam turbines, etc. This refers to a device that converts heat into work or mechanical energy.

**Working Substance**
A quantity of matter inside the engine that undergoes inflow and outflow of heat, expansion and compression, and sometimes change of phase (e.g. water in a steam turbine, or mixture of air and fuel in an internal-combustion engine).

Now consider a cyclic process (a sequence of processes that leaves the working substance in the same state it started)
$$
\Delta = U_2-U_1 = 0 = Q-W
$$
therefore
$$
Q = W
$$
#### Hot and Cold Reservoirs
![[Figure20.3.PNG]]

We would have $Q_h > 0$ as heat is transferred to the working substance and $Q_c < 0$ as heat leaves the working substance. Then the net heat absorbed per cycle is
$$
Q = Q_h + Q_c = |Q_h| - |Q_c|
$$
Then through the first law:
$$
W = Q = Q_h + Q_c = |Q_h| - |Q_c|
$$

We define the thermal efficiency of an engine to be
$$
e = \frac{W}{Q_h}
$$
so we can get
$$
e = 1 + \frac{Q_c}{Q_h} = 1 - \left|\frac{Q_c}{Q_h}\right|
$$
---
### Internal Combustion Engines
![[Figure20.5.PNG]]
#### Otto Cycle
The following is a pV diagram for the Otto cycle an idealized model of the thermodynamic processes in a gasoline engine.

![[Figure20.6.PNG]]

---
### Refrigerators
These are essentially heat engines operating in reverse, where heat is taken from a cold place and is given to a warmer place. This requires a net input of mechanical work, as it is a non-natural process.

![[Figure20.8.PNG]]

$Q_c$ would be positive and $Q_h, W$ would be negative, where $Q_h > Q_c$ such that
$$
Q_h + Q_c - W = 0
$$

Because $Q_h$ and $W$ are negative, then
$$
|Q_h| = Q_c + |W|
$$

We can get a refrigerator's coefficient of performance K:
$$
K = \left|Q_c\right|
$$
#### Practical Refrigerators
![[Figure20.9.PNG]]

#### Clausius Statement
"Heat never flows spontaneously from lower temperature to higher temperature without work."

---
### Carnot Cycle
No heat engine can have 100% efficiency.
Sadi Carnot then asks: "What is the maximum possible efficiency can an engine have, given two heat reservoirs at temperatures $T_h$ and $T_c$?" He then answers this in 1824, where he develops an idealized heat engine that has the maximum possible efficiency consistent with the second law.

To get maximum heat-engine efficiency, we avoid all irreversible process. During heat transfer in a Carnot cycle, there must be no finite temperature drop. In addition, when temperature of working substance is between $T_h$ and $T_c$, there must be no heat transfer between the engine and reservoir.

We would then have two reversible isothermal and two reversible adiabatic processes:

![[Figure20.13.PNG]]

The heat transfer in a Carnot engine would be equivalent to
$$
\frac{Q_c}{Q_h} = -\frac{T_c}{T_h} \,\,\,\text{or}\,\,\, \frac{|Q_c|}{|Q_h|} = \frac{T_c}{T_h}
$$
and our efficiency would be
$$
e_\text{carnot} = 1-\frac{T_c}{T_h} = \frac{{T_h-T_c}}{T_h}
$$
These can be derived by looking through the  processes one by one.
In the isothermal expansion from point a to b:
$$
Q_h = W_{ab} = \int p\,dV = \int_a^b \frac{nRT_h}{V}\,dV = nRT_h\ln(\frac{V_b}{V_a})
$$
Similarly, in the isothermal compression from c to d:
$$
Q_C = W_{cd} = \int p\,dV = \int_c^d \frac{nRT_c}{V}\,dV = nRT_c\ln\left( \frac{V_d}{V_c} \right) = -nRT_c\ln\left( \frac{V_c}{V_d} \right)
$$
Such that we can get the ratio
$$
\frac{Q_c}{Q_H} = -\frac{T_c\ln\left( \frac{V_c}{V_d} \right)}{T_h\ln\left( \frac{V_b}{V_a} \right)}
$$
Now we can take a look at the adiabatic processes at b to c and d to a:
$$
\frac{V_b^{\gamma-1}}{V_a^{\gamma-1}} = \frac{V_c^{\gamma-1}}{V_d^{\gamma-1}}
$$
which is equivalent to
$$
\frac{V_b}{V_a} = \frac{V_c}{V_d}
$$
So then we have
$$
\frac{Q_c}{Q_H} = -\frac{T_c\ln\left( \frac{V_c}{V_d} \right)}{T_h\ln\left( \frac{V_b}{V_a} \right)} = -\frac{T_c}{T_h}
$$
---
### Entropy
Entropy provides a quantitative measure of randomness. Examples of increasing randomness of natural processes include:
- Irreversible heat flow
- Addition of heat to a body
- Free expansion of a gas

Consider an infinitesimal isothermal expansion of an ideal gas (heat dQ is added and the gas expands just enough to keep the temperature constant). Since the U is constant (dU = 0), then
$$
dQ = dW = pdV = \frac{nRT}{V} dV
$$
so that
$$
\frac{dV}{V} = \frac{dQ}{nRT}
$$
We define dS as the infinitesimal change in entropy during an infinitesimal reversible process at absolute temperature T:
$$
dS = \frac{dQ}{T}
$$
If the total amount of heat Q is added during a reversible isothermal process at absolute temperature T, the total entropy change $\Delta S$ would be
$$
\Delta S = S_2 - S_1 = \frac{Q}{T}
$$
#### In Reversible Processes (Not Necessarily Isothermal)
We generalize the definition of entropy change for any reversible processes leading from an initial state to a final state — regardless if its isothermal.

Imagine the process to be composed of a series of infinitesimal reversible steps. During a typical step, the infinitesimal quantity of heat dQ is added to a system at absolute temperature T. We then sum:
$$
\Delta s = \int_1^2 \frac{dQ}{T}
$$
Change in entropy $\Delta S$ does not depend on the path but is the same for all possible processes from state 1 to state 2. Since entropy is a function only of the state of a system, entropy changes can also be calculated for irreversible (nonequilibrium) processes.

This means that a gas that expands adiabatically and reversibly has zero change in entropy, i.e. it is also an isentropic process.

#### Entropy in Cyclic Process
The total entropy change during any reversible cycle is zero:
$$
\int \frac{dQ}{T} = 0
$$

####  Entropy and Second Law
When all systems taking part in a process are included, the entropy either remains constant or increases. No process is possible where entropy decreases.