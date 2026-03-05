### Magnetic Materials
In a practical sense, all materials should have a magnetic response, where:
- Orbiting electrons around the nuclei act as magnetic dipoles
- Electron spins also contributes to magnetic dipoles (this is a quantum object, having no classical analog, so we ignore this for now).

Magnetization can be defined as:
$$
\vec{M} = \frac{1}{V}\sum_i \vec{m}_i
$$
Alternatively, it can be viewed as the magnetic dipole moment per unit volume.

In some cases, magnets can have uniform magnetization.

There are three types of responses of matter to a magnetic field:
- Paramagnets: magnetization $\vec{M}$ parallel to applied $\vec{B}$
	- Closest analogue to linear dielectrics
- Diamagnets: magnetization $\vec{M}$ opposite to applied $\vec{B}$
- Ferromagnets: finite magnetization $\vec{M}$ even without $\vec{B}$
### Magnetic Dipole Response to Field
##### Paramagnetic Response
We suppose a rectangle current loop with side lengths $a$ and $b$. Then,
$$
\vec{N} = aF\sin \theta \hat{x} \to \vec{N}=I
$$
Materials can show paramagnetic responses depending on their electronic configuration (partially complete electron shells)
##### Diamagnetic Response
We make a modification to an atomic orbit,
$$
I = -\frac{e}{T} = -\frac{ev}{2\pi R} \to \vec{m} = -\frac{1}{2}evR\hat{z}
$$
such that
$$
\Delta \vec{m} = -\frac{1}{2}e(\Delta v)R\hat{z} = -\frac{e^2R^2}{4m_e}\vec{B}
$$
Note that all materials show all diamagnetic responses, but can sometimes just be overshadowed by other stronger responses (e.g. paramagnetic).

### Field of Magnetic Objects
With the field inside a sphere as
$$
\vec{B} = \frac{2}{3} \mu_0\vec{M}
$$
$\vec{M}$ actually induces $\vec{B}$, which means that it actually boosts its own internal magnetic field.

A paramagnetic material actually enhances the magnetic field, such that the field "leaks" out

### Nonlinear magnetic media
##### Ferromagnets
Where
$$
\vec{M} \neq 0
$$
without applying any field. This demonstrates a violation of linear relation
$$
\vec{M} = \chi_m\vec{H}
$$
It represents a quantum phenomena, with exchange interaction
$$
U = -2J \sum_{p=1}^N \vec{S}_p \cdot \vec{S}_{p+1} \tag{J >0}
$$
where it prefers a spontaneous parallel alignment of spins. It takes a lot of energy to flip the first few spins.

Analogous to human behavior involving a crowd.