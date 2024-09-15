#phys31-2 #waves #wave-equation
$$
\begin{align}
	k &= \frac{2\pi}{\lambda} \\
	\omega &= \frac{2\pi}{T}  
\end{align}
$$
$$
y(x,t) = A\cos(kx\pm \omega t)
$$
where $A$ is amplitude, $k$ is the wave number, and $\omega$ is the angular frequency.

By working to find the [[Partial Derivatives|second partial derivatives]] with respect to $t$ and $x$, namely
$$
\begin{align}
	\frac{\delta^2y(x,t)}{\delta t^2} = -\omega^2A\cos(kx-\omega t) \\
	\frac{\delta^2y(x,t)}{\delta x^2} = -k^2A\cos(kx-\omega t)
\end{align}
$$
And then finding the relationship between these two partial derivatives:
$$
\begin{align}
	\frac
		{\frac{\delta^2y(x,t)}{\delta t^2}}
		{\frac{\delta^2y(x,t)}{\delta x^2}}
	= \frac{\omega^2}{k^2} = v^2
\end{align}
$$
Then we get the wave equation:
$$
\frac{\delta^2y(x,t)}{\delta x^2} = \frac{1}{v^2} \frac{\delta^2y(x,t)}{\delta t^2}
$$
Note: In a lot of instances the speed of light $c$ is used in place of $v$.

### Summary
Function of a particle in a wave:
$$
y(x,t) = A\cos(kx\pm \omega t)
$$
Its components:
- Wave number $k = \frac{2\pi}{\lambda}$
- Angular frequency $\omega = 2\pi f = \frac{2\pi}{T}$
- Amplitude $A$