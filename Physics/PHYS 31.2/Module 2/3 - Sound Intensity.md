#phys31-2 #waves 
### Intensity
Remember in [[2 - Wave Velocity, Energy, Power, and Intensity]] that intensity is the energy transfer per unit area perpendicular to the direction of propagation. Also note the [[1 - Formula of a Wave|formula for displacement on a wave]] and [[1 - Sound and Hearing|pressure fluctuation equation]]:
$$
\begin{align*}
y(x,t) &= A\cos(kx-\omega t) \\
p(x,t) &= BkA\sin(kx-\omega t)
\end{align*}
$$
and the velocity of a particle along $y$:
$$
v_y(x,t) = \frac{\delta y(x,t)}{\delta t} = \omega A\sin(kx-\omega t)
$$

From this we can get the power in the form $p(x,t)v_y(x,t)$ (see [[2 - Wave Velocity, Energy, Power, and Intensity]]):
$$
\begin{align}
p(x,t)v_y(x,t) &= [BkA\sin(kx-\omega t)][\omega A\sin(kx-\omega t)] \\
&= B\omega kA^2\sin^2(kx-\omega t)
\end{align}
$$

The intensity of a sound wave is the time average value of the power per unit area. The average value of $\sin^2(kx-\omega t)$ in one period $T = \frac{2\pi}{\omega}$, which then means that
$$
I = \frac{1}{2}B\omega kA^2
$$
Since we know that $\omega = vk$ and $v = \sqrt{\frac{B}{\rho}}$, then we can rewrite this as
$$
I = \frac{1}{2}\sqrt{\rho B}\omega^2A^2
$$
This is the intensity of a sinusoidal sound wave.

We can also express $I$ in terms of $p_\text{max}$:
$$
\begin{align*}
p_\text{max} &= BkA \\
I &= \frac{1}{2} B\omega KA^2 \\
&= \frac{\omega p_\text{max}^2}{2Bk} \\
&= \frac{vp_\text{max}^2}{2B}
\end{align*}
$$and then if we use the relationship $v^2 = B/\rho$ (remember [[2 - Speed of Sound Waves#Speed of Sound in Fluids]]):
$$
I = \frac{p_\text{max}^2}{2\rho v} = \frac{p_\text{max}^2}{2\sqrt{\rho B}}
$$
Note that the total average power carried across a surface by a sound wave is the product ofthe intensity and surface area (IF intensity is uniform).

### Decibel Scale
A logarithmic measure of intensity is used for sound in the context of humans. The sound intensity level is expressed through:
$$
\beta = (10dB)\log\frac{I}{I_0}
$$
where $I_0$ is the threshold of hearing at 1000 Hz ($I_0 = 1 \times 10^{-12} W/m^2$). This is expressed in decibels (dB), 1/10 of a bel.

Note that this means if a sound wave is equal in intensity to $I_0$, then $\beta = 0\,dB$. This also means that the decibel scale is based on human hearing.

### Summary:
The intensity of a sound wave can be expressed as follows:
$$
I = \frac{1}{2}\sqrt{\rho B}\omega^2A^2
$$
$$
I = \frac{p_\text{max}^2}{2\rho v} = \frac{p_\text{max}^2}{2\sqrt{\rho B}}
$$
Then to get the sound intensity level in decibels:
$$
\beta = (10dB)\log\frac{I}{I_0}
$$