### PV curves at constant temperature—isotherms
A single experiment can measure how the pressure changes as volume changes—this is known as an isothermal curve. This is a graphical representation of the ideal gas equation of state.

![[Figure18.6.PNG]]
Many isothermal curves together make a three-dimensional phase surface.

We can use this graph to predict what happens to a material in a sealed, rigid container if temperature is increased.

![[Figure18.7.PNG]]

Notice the points of zero slope at points where phase change occurs.
### Ideal-Gas Equation
$$
pV = nRT
$$
where $R = 8.314$ J/mol K

In terms of mass of gas and molar mass $M$ where $m_\text{total} = nM$, then
$$
\begin{align}
pV &= \frac{m_\text{total}}{M} RT \\
\frac{m_\text{total}}{V} &= \frac{pM}{RT} \\
\rho &= \frac{pM}{RT} \tag{using density formula}
\end{align}
$$

### Van Der Waals Equation
$$
\left( p+\frac{an^2}{V^2} \right)(V - nb) = nRT
$$
where b represents the volume of a mole of molecules and n is the number of moles.

### Avogadro's Number
The number of a molecules in a mole is Avogadro's number, $6.02214179 \times 10^{23}$ molecules/mol
and the molar mass M is the mass of 1 mole of a compound. This is equal to the mass m of a single molecule multiplied by Avogadro's number.

### Molecule collisions and Pressure
The change in the x-component of momentum of a single molecule is
$$
m|v_x| - (-m|v_x|) = 2m|v_x|
$$
and we have the volume of the cylinder
$$
V = A|v_x|dt
$$
from which we can get the number of molecules in the cylinder assuming that the number of molecules per unit volume is uniform (N/V):
$$
\left( \frac{N}{V} \right)A|v_x|dt
$$
On average, half the molecules would be moving towards the wall and the other half is away from it. Then the number of collisions with A during dt would be
$$
\frac{1}{2}\left( \frac{N}{V} \right)A|v_x|dt
$$

For the system of all molecules in the gas, then the total momentum change $dP_x$ during $dt$ should be
$$
dP_x = \frac{1}{2}\left( \frac{N}{V} \right)(A|v_x|dt)(2m|v_x|) = \frac{NAmv_x^2}{V}dt
$$
which then gives us the rate of change of momentum component $P_x$:

$$
\frac{dPx}{dt} = \frac{NAmv_x^2}{V}
$$

#### Pressure and Molecular Kinetic Energies
The speed $v$ of a molecule is related to the velocity components by
$$
v^2 = v_x^2 + v_y^2 + v_z^2
$$
and we can express the average over all molecules as
$$
(v^2)_\text{av} = (v_x^2)_\text{av} + (v_y^2)_\text{av} + (v_z^2)_\text{av}
$$
There shouldn't be any real difference between the x, y, and z-directions in the model, so we get
$$
(v_x^2)_\text{av} = \frac{1}{3}(v^2)_\text{av}
$$
Remember that pressure is the magnitude of the force exerted on the wall per unit area. Then we should get
$$
p = \frac{F}{A} = \frac{Nmv_x^2}{V}
$$
where we can get
$$
\begin{align}
pV &= \frac{1}{3}Nm(v^2)_\text{av} \\
&= \frac{2}{3}N\left[ \frac{1}{2} m(v^2)_\text{av} \right]
\end{align}
$$
Notice that the expression in the brackets is essentially the kinetic energy equation. Combining this with the ideal-gas equation, we should get
$$
\begin{align}
pV &= \frac{2}{3}K_\text{tr} = nRT \\
K_\text{tr} &= \frac{3}{2}nRT
\end{align}
$$
where we get the average translational kinetic energy of n moles of an ideal gas.

Note that we can also do
$$
\frac{1}{2}m(v^2)_\text{av} = \frac{3}{2}kT
$$
to get the average translational kinetic energy of a gas molecule, where $k$ is the Boltzmann's constant where
$$
k = \frac{R}{N_A} = 1.381 \times 10^{-23} \text{J/molecule K}
$$
From here we can get the root-mean-square speed $v_\text{rms}$ of a gas molecule through
$$
\begin{align}
v_\text{rms} &= \sqrt{(v^2)_\text{av}} \\
&= \sqrt{\frac{3kT}{m}} = \sqrt{ \frac{3RT}{M} }
\end{align}
$$
### How much energy can ensembles contain?
Consider a fixed volume V of a monoatomic ideal gas with point-like molecules.

![[Figure18.17.PNG]]

When an amount of heat dQ is added to the gas, the total translational kinetic energy increases by
$$
dQ = nC_v \, dT \rightarrow dK_\text{tr}=\frac{3}{2} nR \, dT
$$
then we have
$$
\begin{align}
nC_v\,dT = \frac{3}{2}nR\,dT\\
C_v = \frac{3}{2}R = 12.47 \, \text{J/mol K} \tag{ideal gas of point particles}
\end{align}
$$

![[Table18.1.PNG]]
The point-molecule model is good enough for monoatomic gases, but does not correctly predict for diatomic and polyatomic gases.

This occurs because diatomic molecules can be represented by two point masses. There can be additional kinetic energy asociated with the rotation about axes through its center of mass, and may also have vibrating motion associated with them.

#### Principle of Equipartition of Energy
We find the energy associated with each additional kind of motion of a complex molecule through the Principle of Equipartition of Energy.

This states that each velocity component (linear or angular) has, on average, an associated kinetic energy per molecule of $\frac{1}{2}kT$.
- Degrees of freedom -> number of velocity components needed to describe the motion of a molecule completely
- e.g. for monoatomic gas -

We then assign 5 degrees of freedom for a diatomic molecule (such that $\frac{5}{2}kT$) so that we get the kinetic energy of $n$ moles:
$$
K_\text{total} = N\left( \frac{5}{2}kT \right) = \frac{5}{2}nRT
$$
so then we get
$$
C_v = \frac{5}{2}R = 20.79\,\text{J/mol K} \tag{diatomic gas, including rotation}
$$

#### What about vibration?
For most diatomic gases, vibration motion does not contribute appreciably to heat capacity.

![[Table 18.18.PNG]]

A high amount of heat energy is required to 

#### For monoatomic solids
We visualize the forces between neighboring atoms in a crystal, and we envision every atom as being attached to its neighbors by springs.

![[Figure18.20.PNG]]

We get 3 degrees of freedom corresponding to the vibrational motion, each with KE of $\frac{1}{2}kT$, where each atom has potential energy associated with elastic deformation. For SHM, the average kinetic energy is equal to the average potential energy.

If a crystal has $N$ atoms or $n$ moles, then

$$
C_V = 3R = 24.9 \text{J/mol K} \tag{Rule of Dulong and Petit}
$$
### Summary:
Ideal gas law:
$$
pV = nRT = NkT
$$
(where the latter is expressed on a per-molecule basis)

Average translational kinetic energy of $n$ moles of ideal gas:
$$
K_\text{tr} = \frac{3}{2}nRT
$$
Average translational kinetic energy of a gas molecule:
$$
\frac{1}{2}m(v^2)_\text{av} = \frac{3}{2}kT
$$
(note that $m$ refers to the mass of a single molecule)

Root mean-square speed of a gas molecule:
$$
\begin{align}
v_\text{rms} &= \sqrt{(v^2)_\text{av}} \\
&= \sqrt{\frac{3kT}{m}} = \sqrt{ \frac{3RT}{M} }
\end{align}
$$