#phys31-2 #waves 
### Velocity of Waves on a String
Speed of a transverse wave on a string:
$$
	v = \sqrt{\frac{F}{\mu}}
$$
where $F$ is the tension of the string and $\mu$ is the linear mass density of the string.
In other words, this can be expressed as
$$
\text{velocity} = \sqrt{\frac{\text{Restoring force returning to equil.}}{\text{Inertia resisting return}}}
$$
### Energy & Power in Wave Motion
#### Energy
$\frac{F_y}{F}$ is equal to the slope of the string. Then:
$$
F_y(x,t) = -F\frac{\delta y(x,t)}{\delta x}
$$
#### Power
Since we know that $P = Fv$, then
$$
P(x,t) = F_y(x,t)v_y(x,t) = -F\frac{\delta y(x,t)}{\delta x} \frac{\delta y (x,t)}{\delta t}
$$
This is valid for any point on the string.

For a sinusoidal wave, this then becomes
$$
P(x,t) = Fk\omega A^2\sin^2(kx-\omega t)
$$
Then with $\omega=vk$ and $v^2=\frac{F}{\mu}$,
$$
P(x,t) = \sqrt{\mu F}\omega^2A^2\sin^2(kx-\omega t)
$$
which also implies that the maximum power at any point on the wave is
$$
P_\text{max} = \sqrt{\mu F}\omega^2A^2
$$

### Intensity
Intensity (aka flux) is used to measure a radiant energy.

Consider waves where energy is transported omnidirectionally (e.g. sound in air).
Now consider two points of the wave with values $r_i$ (radius) and $I_i$ (intensity). Say that we get two points $i=1$ and $i=2$, where $i=2$ is farther from the wave source. Then we can assume the following relationships:

$$
\begin{align}
I_2 < I_1 && r_1<r_2
\end{align}
$$
We can also get the relationship between $r$ and $I$:
$$
\begin{align*}
I \propto \frac{1}{r^2}; && I=\frac{P}{4\pi r^2}; && \frac{I_1}{I_2} = \frac{(r_2)^2}{(r_1)^2}
\end{align*}
$$
The third equation is due to the inverse square law.

### Summary:
1. (Propagation) Speed of a Transverse Wave on a String: $v = \sqrt{\frac{F}{\mu}}$
2. Power of a wave: $P(x,t) = \sqrt{\mu F}\omega^2A^2\sin^2(kx-\omega t)$