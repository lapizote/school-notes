## Circuits
### Circuit Equations
Current: $\displaystyle I = \frac{dQ}{dt} = n|q|v_dA$
($n$ = number of charges; $q$ = charge per particle; $v_d$ = drift velocity; $A$ = area of conductor)
Current Density: $\displaystyle \vec{J} = nq\vec{v}_d = \frac{I}{A}$
Resistivity: $\displaystyle \rho=\frac{E}{J}$
($J$ = current density; $E$ = electric field)
Resistivity :$\displaystyle \rho(T) = \rho_0[1+\alpha(T-T_0)]$ (for small temperature changes)
Resistance: $\displaystyle R = \frac{\rho L}{A}$
Ohm's Law: $V = IR$
Power: $P = V_{ab}I$
Power (to resistor): $\displaystyle P = I^2R = \frac{{V_{ab}}^2}{R}$
Conduction in metals: $\displaystyle \rho = \frac{m}{ne^2\tau}$
### Circuits
![[Circuits and EMF.png]]
Every real source of emf has some internal resistance $r$, so its terminal potential difference is always
$$
V_{ab} = \varepsilon-Ir
$$
### Resistors in Circuits
For series: $\displaystyle R_{eq} = R_1 + R_2 + \dots$
For parallel: $\displaystyle R_{eq} = \left( \frac{1}{R_1} + \frac{1}{R_2} + \dots \right)^{-1}$
### Kirchhoff's Rules:
##### Junction/Current Rule:
At any junction, the algebraic sum of the currents into a junction is zero, i.e. $\displaystyle\sum I = 0$
![[Junction Rule.png]]
##### Loop/Voltage Rule:
At any loop, the algebraic sum of the potential differences is zero, i.e. $\displaystyle \sum V = 0$
![[Loop Rule.png]]
### R-C Circuits
When a capacitor is charged by a battery in series w/ a resistor, the current and capacitor charge are not constant, i.e. the charge and current approaches zero asymptotically:
![[R-C Circuit.png]]
##### Capacitor Charging:
For the charge inside the capacitor:
$$
\begin{align}
q &= C\varepsilon(1-e^{-t/RC}) \\
&= Q_f(1-e^{-t/RC})
\end{align}
$$
For the current flowing throughout the circuit:
$$
i = \frac{dq}{dt} = \frac{\varepsilon}{R}e^{-t/RC} = I_0e^{-t/RC}
$$
##### Capacitor Discharging:
For the charge inside the capacitor:
$$
\begin{align}
q &= Q_0e^{-t/RC} \\
\end{align}
$$
For the current flowing throughout the circuit:
$$
i = \frac{dq}{dt} = -\frac{Q_0}{RC}e^{-t/RC} = I_0e^{-t/RC}
$$
## Magnetism
### Magnetic Force
Charge needs to move in a magnetic field to experience a force. For direction, refer to Fleming's hand rules (left is for force generation, right is for induction)
![[Flemings Hand Rules.png|600]]
Alternatively, right hand rule
![[Right hand rule.png]]

Can be found through either
$$
\begin{align}
F = |q|vB \sin \theta && \vec{F} = q\vec{v} \times \vec{B}
\end{align}
$$
where $B$ is the magnetic field, measured in Tesla (T) with SI units NS/Cm.

Because the force is perpendicular to the direction of the field, it can be said that no work is being done. A charge can have a circular path:
![[Magnet circular path.png|400]]
where
$$
\begin{align}
F_C &= m \frac{v^2}{R} = F_M \\
qvB &= m \frac{v^2}{R} \\
R &= \frac{mv}{qB}
\end{align}
$$
which results in a helical path.
### Magnetic Flux
Given a field $B$ going through a surface:
![[Magnetic Flux.png|400]]
$$
\Phi_B= B\perp A = BA\cos \phi
$$
where $\displaystyle B = \frac{\Phi B}{A}$ if $B$ is perpendicular to the surface area. For an irregular area, this can be expressed as
$$
\Phi_B = \int_{S}\vec{B} \cdot d\vec{A}
$$
With Gauss' law, for a closed surface, this value is 0.

### Biot-Savart Law
Length $d\vec{B}$ due to length element
$$
d\vec{B} = k_m \frac{Id\vec{L} \times \vec{r}}{r^3}
$$
Which means that for a finite length of wire:
$$
\vec{B} = k_m \int \frac{Id\vec{L} \times \vec{r}}{r^3}
$$
##### Magnetic Field of a Straight Current
Magnetic field produced by a straight current-carrying conductor of length 2a:

On the perpendicular bisector:
$$
B = k_mI \frac{2a}{x\sqrt{ x^2 + a^2 }}
$$
In the limit $a \gg x$
$$
B = 2k_m \frac{I}{x}
$$
