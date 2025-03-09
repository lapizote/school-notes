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