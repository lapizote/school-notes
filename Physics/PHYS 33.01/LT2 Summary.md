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
![[Circuits and EMF.png|center|250]]
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
![[Junction Rule.png|center|250]]
##### Loop/Voltage Rule:
At any loop, the algebraic sum of the potential differences is zero, i.e. $\displaystyle \sum V = 0$
![[Loop Rule.png|center|250]]
### R-C Circuits
When a capacitor is charged by a battery in series w/ a resistor, the current and capacitor charge are not constant, i.e. the charge and current approaches zero asymptotically:
![[R-C Circuit.png|center|250]]
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
##### On Charged Particles
Charge needs to move in a magnetic field to experience a force. For direction, refer to Fleming's hand rules (left is for force generation, right is for induction)
![[Flemings Hand Rules.png|center|350]]
Alternatively, right hand rule
![[Right hand rule.png|center|300]]

Can be found through either
$$
\begin{align}
F = |q|vB \sin \theta && \vec{F} = q\vec{v} \times \vec{B}
\end{align}
$$
where $B$ is the magnetic field, measured in Tesla (T) with SI units NS/Cm.

Because the force is perpendicular to the direction of the field, it can be said that no work is being done. A charge can have a circular path:
![[Magnet circular path.png|center|300]]
where
$$
\begin{align}
F_C &= m \frac{v^2}{R} = F_M \\
qvB &= m \frac{v^2}{R} \\
R &= \frac{mv}{qB}
\end{align}
$$
which results in a helical path.
##### On Current-carrying Conductor
$$
\begin{align}
F_M &= \Delta q vB \sin \theta \\
&= \left( \frac{\Delta q}{\Delta t} \right) (v\Delta t)B \sin \theta \\
&= I(\Delta L)B \sin \theta
\end{align}
$$
where its vector form will be
$$
\vec{F} = I(\vec{L} \times \vec{B})
$$
If conductor is not a straight line, divide into segments $dL$:
$$
d\vec{F} = I(d\vec{L} \times \vec{B})
$$
such that
$$
\vec{F} = \int I(d\vec{L} \times \vec{B})
$$
##### Force and Torque on a Current Loop
![[current loop.png|center|300]]
Net force is zero, but net torque is not zero.
$$
\begin{align}
\tau &= 2(ILB)\left( \frac{1}{2} W\sin \phi \right) \\
&= I(LW)B \sin \phi \\
&= IAB \sin \phi
\end{align}
$$
where $A = LW$ is the area of the loop.
![[current loop mu.png | center]]
For loop with $N$ turns:
$$
\tau = NIAB \sin \phi
$$
In vector form:
$$
\vec{\tau} = \vec{\mu} \times \vec{B}
$$
where $\mu = NIA$
### Magnetic Flux
Given a field $B$ going through a surface:
![[Magnetic Flux.png|center|250]]
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
=======
### Applications of Motion of Charged Particles
Velocity Selector and Thomson's Experiment
$$
\begin{align}
v = \frac{E}{B} && \frac{e}{m} = \frac{E^2}{2VB^2}
\end{align}
$$
Mass Spectrometer
For circular path:
$$
r = \frac{mv}{qB}
$$
such that the energy of particle
$$
\begin{align}
\frac{1}{2}mv^2 &= qV \\
m &= \left( \frac{qr^2}{2V} \right)B^2
\end{align}
$$
### Hall Effect
Hall voltage:
$$
\begin{align}
V_H &= E_e\Delta z = v_dB_y\Delta z \\
&= \frac{J_xB_y\Delta z}{nq}
\end{align}
$$
### Magnetic Sources
Current carrying wires can produce magnetic fields.
The force between parallel wires:
$$
F = 2k_m \frac{I_1I_2}{d} L
$$
A moving point charge q:
$$
\begin{align}
B = k_m \frac{|q|v\sin\phi}{r^2} && \vec{B} = k_m \frac{|q|\vec{v}\times \vec{r}}{r^3}
\end{align}
$$
where $k_m = \frac{\mu_0}{4\pi} = 1 \times 10^{-7} T \cdot m / A$
The direction is dictated by right hand rule.

##### Biot-Savart Law
![[Biot-Savart.png|center|200]]
Given the above:
$$
\begin{align}
d\vec{B} &= k_m \frac{Id\vec{L} \times \vec{r}}{r^3} \\
\vec{B} &= k_m \int \frac{I d\vec{L} \times \vec{r}}{r^3} = k_m \int \frac{I d\vec{L} \times \hat{r}}{r^2}
\end{align}
$$
##### Ampere's Law
The line integral of $B$ along a closed path is always the same.
$$
\oint \vec{B} \cdot d\vec{l} = \mu_0I
$$
Because of this, in a current-carrying solenoid:
Inside the solenoid: $B_\text{total} = \mu_0nI$ (where $n$ is the number of turns)
Outside the solenoid: $B_\text{total} = 0$
Outside the solenoid: $B_\text{total} = 0$
$
