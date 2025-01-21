Optical effects, like interference, depend on the wave nature of light.

Recall [[3 - Interference and Standing Waves]] and [[5 - Sound Wave Interference]], where two or more waves overlap in space and is governed by the principle of superposition. This also applies to electromagnetic waves.

### Displacement
- (in the context of waves on a surface of a liquid) refers to the actual displacement of the surface above or below its normal level
- (in the context of sound) the excess or lack of pressure

### Interference in Two or Three Dimensions
Interference is most easily observed when sinusoidal waves with a single frequency $f$ and wavelength $\lambda$ is combined.

![[Figure35.1.PNG]]

We can assume that the material surrounding $S_1$ is uniform such that there is no refraction or bending. If the waves are 2D (e.g. waves on a surface of a liquid), the figure represents circular wave fronts. If they are 3D, they represent spherical wave fronts spreading away from $S_1$.

![[Figure35.2.PNG]]

Assume that we are working with monochromatic (single wavelength) waves. Now consider two identical sources of monochromatic waves $S_1$ and $S_2$ wherein they produce waves of same amplitude and wavelength (such that they are permanently in phase).

(Note that two monochromatic sources of the same frequency and constant phase relationship are said to be **coherent**.)

First, let us consider point $a$. It takes an equal amount of time to travel from $S_1$ to $a$ and $S_2$ to $a$, so the waves arrive in phase at $a$.

Now, consider point $b$. Since the distances from $S_1$ and $S_2$ are different but there is a $2\lambda$ difference, waves arrive in phase at $b$ regardless.

Remember that when waves arrive at a point in phase (i.e. path difference is an integral multiple of $\lambda$), constructive interference occurs.

Now we take a look at point $c$, where the path difference is $2.50\lambda$. Destructive interference occurs, because the path difference is a half-integral number of $\lambda$.

![[Figure35.3.PNG]]

We can then construct a diagram of antinodal curves and nodal curves (the former being points of constructive interference, the latter being points of destructive interference)

### Two-Source Interference of Light
We can now take a look at Young's double slit experiment.

![[Figure35.5-1.PNG]]

Light is directed towards a screen with a narrow slit $S_0$, while waves emerging from $S_1$ and $S_2$ are in phase, such that they are coherent sources.

![[Figure35.5-2.PNG]]

We assume that $r_1$ is parallel to $r_2$, such that the path difference between the two rays is essentially
$$
r_2 - r_1 = d\sin\theta
$$
For this assumption to be true, we need $R >> d$. Because of this, our condition for constructive interference in this experiment needs to be
$$
\begin{align}
\delta = d\sin\theta = m\lambda \tag{$m = 0, \pm1, \pm2, \dots$}
\end{align}
$$
While for destructive interference:
$$
\begin{align}
\delta = d\sin\theta = (m+\frac{1}{2})\lambda \tag{$m = 0, \pm1, \pm2, \dots$}
\end{align}
$$
![[Figure35.6.PNG]]

How about the positions of the bright bands, however? We can go back to Figure 35.5.

Let $y_m$ be the distance from the center of the pattern ($\theta = 0$) to the center of the $m^\text{th}$ bright band. Then:
$$
\begin{align}
\tan\theta = \frac{y_m}{R} &\approx \sin\theta = \frac{m\lambda}{d} \\
y_m &= R\frac{m\lambda}{d}
\end{align}
$$
(Math majors HATE this one trick!)

$m$ refers to the order of the fringe, $R$ is the distance to the screen, and $d$ is the separation of slits. Note that again, this is only valid for small angles. This means that we need $R >> d$ and $R >> y_m$.

### Intensity in Interference Patterns
Say we want to find the intensity at any point $P$ in a two-source interfence pattern. Consider two interfering waves with phase difference by phase angle $\phi$.
$$
\begin{align}
E_1(t) &= E\cos(\omega t + \phi) \\
E_2(t) &= E\cos(\omega t)
\end{align}
$$
By superposition, we find the resultant wave. We can use a phasor diagram to show the vector addition to find the amplitude $E_p$.

![[Figure35.9.PNG]]

Using the law of cosines:
$$
c^2 = a^2 + b^2 - 2ab \cos(C)
$$
$$
\begin{align}
E_p^2 &= E^2 + E^2 - 2E^2\cos(\pi - \phi) \\
&= E^2 + E^2 - 2E^2\cos(\pi) = 2E^2(1+\cos\phi) \\
&= 4E^2\cos^2(\frac{\phi}{2}) \tag{half-angle identity}
\end{align}
$$
Intensity is related to the square of the electric field:
$$
I = \frac{\epsilon_0cE^2_p}{2} = 2\epsilon_0cE^2\cos^2(\frac{\phi}{2})
$$
($\epsilon_0$ refers to permittivity of free space, i.e. ability of free space/vacuum to allow static charges.)

Considering maximum intensity $I_0 = 2\epsilon_0cE^2$:
$$
I = I_0\cos^2(\frac{\phi}{2})
$$

### Phase Difference and Path Difference
We can then determine the phase difference $\phi$ between two fields at any point $P$. Since we know that
$$
	\frac{\phi}{2\pi} = \frac{r_{2}-r_{1}}{\lambda}
$$
due to having a phase difference proportional to the path length, then
$$
\phi = \frac{2\pi}{\lambda}(r_2 - r_1) = k(r_2-r_1)
$$
(remember that wave number $k=(r_2-r_1)$).

Once again, remember through [[#Two-Source Interference of Light]] that the path difference is equal to $d\sin \theta$, such that our equation becomes
$$
\phi = k(r_2-r_1) = kd\sin \theta = \frac{2\pi d}{\lambda}\sin \theta
$$

Substituting in our intensity equation:
$$
I = I_o\cos^2\left( \frac{1}{2} kd\sin \theta \right) = I_0\cos^2\left( \frac{\pi d}{\lambda} \sin \theta \right)
$$
where the maximum intensity occurs with
$$
\begin{align}
		\frac{\pi}{\lambda}\sin \theta = m\pi \tag{$m=0, \pm 1, \pm 2, \dots$}
\end{align}
$$

Since we know that $d \sin \theta = m\lambda$:
$$
I = I_0\cos^2\left( \frac{kdy}{2R} \right) = I_0\cos^2\left( \frac{\pi dy}{\lambda R} \right)
$$

![[Figure35.10.PNG]]

### Change of Phase due to Reflection
#### Lloyd's Mirror
This is an experiment done by Humphrey Lloyd where it demonstrates an interference pattern as a result of reflections.

It should be noted that the reflected ray undergoes a 180$^\circ$ phase change. This is similar to how strings undergo a "phase change" when it is reflected on a fixed end (see [[3 - Interference and Standing Waves#Boundary Conditions]])