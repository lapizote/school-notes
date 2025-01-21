Recall: Transverse waves on a string
//todo: insert figure 33.21
- EM waves are also transverse waves.
- The flux of the magnetic field and the magnetic field vectors are perpendicular to each other and to the direction of propagation
- Define the direction of polarization of the EM wave to the direction of the electric field vector E
Thus, for EM wave described by:
$$
\begin{align}
\vec{E}(x,t) = \hat{j}E_\text{max}\cos(kx - \omega t) \tag{polarized in the y-direction} \\
\vec{B}(x,t) = \hat{k}B_\text{max}\cos(kx - \omega t)
\end{align}
$$
### Applications
In a broadcast antenna, electrons oscillate vertically, producing vertically polarized EM waves that propagate away from the antenna in horizontal direction.

In a light bulb, the random motion of electrons in the filament produce unpolarized light waves regardless of orientation.
#### Polaroid
The most common polarizing filter for visible light is a material known by the trade name Polaroid --- this is used for sunglasses and polarizing filters for camera lenses.

A Polaroid filter is a polymer array much like teeth on a comb, where only waves oscillating parallel to the teeth pass through the comb. This transmits $\geq 80$% of the intensity of the wave that is polarized parallel to the polarizing axis.

Consider an idealized polarizing filter:
///todo: insert figure

### Intensity of Polarized Light
The ratio of transmitted light to incident amplitude is $cos \phi$, while the ratio of transmitted light to incident intensity is $\cos^2\phi$

We then get Malus' law, i.e:
$$
I = I_0\cos^2\phi
$$
This only applies if the incident light passing through the analyzer is already linearly polarized.

### Polarization by Reflection
When unpolarized light is directed towards a reflecting surface and is incident to the polarizing angle $\theta_p$, then the reflected light becomes fully polarized (perpendicular to the plane of incidence). Meanwhile, the transmitted light is partially polarized to the plane of incidence.

If $\theta_i \neq \theta_p$, then the reflected light is partially polarized only.

//todo: insert figure

Note that $\theta_b = 90^\circ - \theta_p$. Because of this:
$$
\begin{align}
n_a\sin\theta_p &= n_b\sin\theta_b \\
n_a\sin\theta_p &= n_b\sin(90^\circ - \theta_p) = n_b\cos\theta_p
\end{align}
$$
we then get
$$
\tan{\theta_p} = \frac{n_b}{n_a}
$$
This is known as Brewster's angle.

### Scattering of Light
The observed colors in the sky depend on the scattering phenomenon. The deep blue color comes from the preferential scattering of photons of shorter wavelength in the visible spectrum.

In the same vein, clouds are white because they scatter all the wavelengths efficiently.

Rayleigh scattering:
$$
I \propto \frac{1}{\lambda^4}
$$
//todo insert figure

This is why the sky is redder as the sun is setting, as the light passes through more air that scatters the blue light out.