### Huygen's Principle
Christian Huygens' 1678 work reveals through geometrical analysis that every point of a wave front can be considered to be a source of secondary wavelets that spread with a speed equal to the speed of propagation of the wave.

This principle then shows us the geometrical method for finding, from the known shape of a wave front at some instant, the shape of the wave front at some later time. This new wave front at a later time is then found by construction a surface tangent to the secondary wavelets or the envelope of the wavelets.

//pic wavelets

The radius of these wavelengths would be $r = vt$.

### Introduction
The interference pattern is observed on a viewing screen when two slits are illuminated by a single wavelength light source.

//pic figure

If the light waves did not spread out after passing through the slits, no interference would occur. However, the light waves from the two slits overlap when they spread out, filling what we expect to the shadowed regions with light and producing interference fringes.

Huygen's principle requires this property, and this is how diffraction occurs.

According to geometric optics, a light source shining on an object in front of a screen should cast a sharp shadow. However, this does not occur because of diffraction.

//pic doesnt happen!!!!

Instead:
//diffraction pattern

Notice that a bright spot occurs at the center, and circular fringes extended outward from the shadow's edge. A central bright spot occurring can only be explained using the wave theory of light.

#### Applying Huygen's Principle to Parallel Wavefront Striking an Opening of Various Sizes
//pic
The wavefront bends and spreads upon encountering the opening; this is even more extreme for smaller openings. This shows the wave nature of light, even more so when the size of the object or obstruction is comparable to or smaller than the wavelength of light.

#### Note:
It is also emphasized that there is no fundamental distinction between interference and diffraction:
- Interference - effects involving waves from a small number of sources, usually two
- Diffraction - usually involves a continuous distribution of Huygen's wavelets across the area of an aperture, or a very large number of sources of apertures

Both interference and diffraction are consequences of superposition and Huygen's principle.

Consider also:
- Fresnel diffraction: point source and the screen are relatively close to the obstacle
- Fraunhofer diffraction: source, obstacle, and screen are fare enough apart such that you consider all the lines from source to obstacle and from obstacle to screen to be parallel.

### Fresnel and Fraunhofer Diffraction by a Single Slit
Below shows Fresnel (near-field) and Fraunhofer (far-field) diffraction for a single slit.
//pic comparing the two

Let us consider Fraunhofer (we refer to this when we describe the diffraction pattern caused by single slit interference). The viewing screen is located distant from the slit, and all the rays emerging from various parts of the slit can be considered to be parallel.
//pic

#### Locating the Dark Fringes
Consider the alternate geometry of Fraunhofer.
//pic of alternate geometry

We can divide the slit into two halves (remember, all the waves are in phase as they leave the slit). Notice that there will be path differences, for example, ray 1 will travel longer than ray 3. We can find that path difference through $\displaystyle \frac{a}{2}\sin \theta$. If this is equal to half a wavelength (phase difference of 180$^\circ$), then the two waves will eventually cancel each other and we get destructive interference.

Then a dark fringe occurs whenever
$$
\frac{a}{2}\sin \theta = \pm \frac{\lambda}{2} \,\,\,\, \text{or} \,\,\,\,\sin \theta = \pm \frac{\lambda}{a}
$$
Such that
$$
\sin \theta = \frac{m\lambda}{a} \tag{$m = \pm1, \pm2, \pm3, \dots$}
$$
Then for small angles
$$
\theta = \frac{m\lambda}{a} \tag{$m = \pm1, \pm2, \pm3, \dots$}
$$
If the distance from the slit to the screen is $x$, and the vertical distance of the $m^\text{th}$ dark band from the center of the pattern is $\tan \theta=\frac{y_m}{x}$.
Then for small $\theta$:
$$
y_m = x \frac{m\lambda}{a}
$$
Note that this is similar with [[1 - Wave Interference#Two-Source Interference of Light]], but instead for dark fringes.

### Intensity in the Single-Slit Pattern
We can derive an expression for the intensity distribution for the single-slit diffraction pattern through the same phasor-addition method as seen in [[1 - Wave Interference#Intensity in Interference Patterns]].

//pic of strips within slit on P

We want to know the intensity at point P. But first, let's consider the special case at point O.

//pics of O

This is the center of the pattern where $\theta = 0$, so the phasors are essentially in phase (i.e. same direction), so we have negligible path difference for $x \gg a$

Now consider wavelets arriving from different strips at point P, at an angle $\theta$ from point O.

//pics of P

Note that $\beta$ is the total phase difference between the first and last phasors, and $E_p$ is the amplitude of the resultant electric field at P (i.e. the chord).

In the limit of infinitesimally narrow strips:

//pics

We have radius $\frac{E_o}{\beta}$. From this, we can then find that
$$
\begin{align}
E_p &= 2\frac{E_o}{\beta} \sin \frac{\beta}{2} \\
&= E_o \frac{\sin\left( \frac{\beta}{2} \right)}{\frac{\beta}{2}}
\end{align}
$$
We can then define I at any point:
$$
I = I_o\left[ \frac{\sin\left( \frac{\beta}{2} \right)}{\frac{\beta}{2}} \right]^2
$$
Since we know that $\beta=\frac{2\pi}{\lambda} a\sin \theta$:
$$
I = I_o[\sin(\frac{\pi a\sin \frac{\theta}{}}{}]
$$
Notice that the central intensity peak is much larger than others, and most of the power in the wave remains within an angle $\theta$ from the perpendicular.

//pic

For dark fringes, $I = 0$.

We can find the location of the maxima by taking the derivative of $I$ with respect to $\theta$, then equating it to 0. There is an approximate solution:
$$
\beta = \pm (2m+1)\pi \tag{$m=0,1,2,\dots$}
$$
In fact, there is no maximum for $m=0$ in this expression. This central maximum is wider than the others, and occurs at $\theta = 0$. Using these approximate values of $\beta$ in the intensity, we find
$$
I_m \approx \frac{I_o}{\left( m+\frac{1}{2} \right)^2\pi^2}
$$
//table of approximation

Notice that the error decreases as $m$ increases.

The single slit diffraction pattern depends on the ratio of the slit width $a$ to the wavelength $\lambda$.

//pics

### Two Slits of Finite Width
Previously, we assumed that the slits are narrow in comparison to the wavelength, and we assume that light from each slit spreads out uniformly in all directions to the right of the slits.

Now what if we have two slits of finite width instead of very narrow widths?

//pic

In this case, we would see both the interference and diffraction of the light

//pic of graph

The peaks in the two-slit interference pattern are modulated by the single slit diffraction pattern. Then the overall pattern of the two finite-width is the product of the two patterns:
$$
\begin{align}
I = I_0\sin^2\frac{\beta}{2} \cos^2 \frac{\phi}{2} \tag{1} \\
\sin c(x) = \frac{\sin x}{x} \tag{2}
\end{align}
$$
//pic of big graph!

Notice that there is a diffraction envelope that contains peaks (which are the interference fringes). In this particular case, the slit width $a$ is 3.0$\mu$m.

#### Several Slits
Notice that in the figure below, there is an array of 8 narrow slits separated by a distance $d$ between slits.

//pic

A lens is used to give a Fraunhofer pattern on a nearby screen, and its function is to allow the pattern to be seen nearby without having the screen being really distant.

Constructive interference occurs for rays at angle $\theta$ to the normal the arrive at point P with a path difference between adjacent slits equal to an integer number of $\lambda$ (much like before). As such, maximas in the pattern occur at the same positions as for the two slits with the same spacing; recall
$$
I=I_0\cos^2\left( \frac{\phi}{2} \right)
$$
Suppose that the phase difference between light from adjacent slits is $\pi$. Then
//phasor diagram, cancels out each other

#### Interference Pattern of Several Slits
Notice the pattern for 2, 8, and 16 equally spaced narrow slits:
//patterns

When there are $N$ slits, there are $(N-1)$ minima between each pair of principal maxima. A minimum occurs when $\phi$ is an integral multiple of $\frac{2\pi}{N}$, except when $\phi$ is an integral multiple of $2\pi$ which gives a principal maximum.

The small secondary maxima between the minima becomes smaller in comparison to the principal maxima as $N$ increases.

If we have enough of these small slits, we have what's called a **diffraction grating**.

### Diffraction Grating
Given enough slits, the maxima become so narrow that their angular position (and hence the wavelength) can be measured to a very high precision. A diffraction grating is such an example, being an array of a large number of slits having the same width $a$ and an equal spacing $d$.

#### Reflection Grating
In a reflection grating, the array of equally spaced slits is