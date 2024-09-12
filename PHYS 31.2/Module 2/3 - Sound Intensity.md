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

