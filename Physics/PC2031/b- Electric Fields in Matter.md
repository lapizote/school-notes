### Polarization
##### Inducing Macroscopic Polarizations
In isotropic atoms/molecules:
$$
\vec{p} = \alpha \vec{E}
$$
where $\vec{p}$ is the induced dipole moment, $\alpha$ is the polarizability, and $\vec{E}$ is the applied electric field.

In anisotropic molecules:
$$
\vec{p} = 
$$
Polarization is defined as the dipole moment per unit volume:
$$
\vec{P} = \frac{1}{V} \sum_i \vec{p}_i
$$
where then the potential induced by multiple dipoles is
$$
V(\vec{r}) = \frac{1}{4\pi\epsilon_0}\int_V \frac{\vec{P}(\vec{r}\,')\cdot \hat{\mathscr{r}}}{\mathscr{r}^2}\,d\tau'
$$
We can manipulate this integral to get
$$
V(\vec{r}) = \frac{1}{4\pi\epsilon_0}\int_V \frac{\vec{P}(\vec{r}\,')\cdot \hat{\mathscr{r}}}{\mathscr{r}^2}\,d\tau'
$$
##### Cause and Effect of Polarization
Working with
$$
\epsilon_0 \nabla \cdot \vec{E} = \rho = \rho_b + \rho_f = -\nabla \cdot \vec{P} + \rho_f
$$
where $\vec{E}$ is the total electric field, $\rho_b$ is bound charge density due to polarization, and $\rho_f$ is the free charge density that we control (not due to polarization), then
$$
\nabla \cdot(\epsilon_0\vec{E}+\vec{P})=\rho_f
$$
We define the term in the parenthesis as the electric displacement
$$
\vec{D} = \epsilon_0 \vec{E} + \vec{P}
$$
such that
$$
\nabla \cdot \vec{D} = \rho_f
$$
We then obtain the Gauss' law for displacement field:
$$
\oint \vec{D} \cdot d \vec{a} = Q_{f_\text{enc}}
$$
Properties:
- No guarantee that the curl is 0: $\nabla \times \vec{D} = \epsilon_0(\nabla \times \vec{E}) + (\nabla \times \vec{P}) = \nabla \times \vec{P} \neq 0$
- We do not have a Coulomb's law for the displacement field $\vec{D}(\vec{r})$.
-  We do not have a potential for the displacement field.
### Linear Dielectrics
When $\vec{E}$ is applied, $\vec{P}$ is induced. This $\vec{P}$ produces a field, then it adds to $\vec{E}$, which further modifies $\vec{P}$, and so on: we have an infinite regress.

To break out of this issue, we need to make an assumption:
$$
\vec{P} = \epsilon_0 \mathcal{X}_e\vec{E}
$$
where $\mathcal{X}_e$ is the electric susceptibility, which we then obtain
$$
\vec{D} = \epsilon_0\vec{E} + \epsilon_0\mathcal{X}_e\vec{E} = \epsilon_0(1+\mathcal{X}_e)\vec{E}
$$
where we can rewrite it as
$$
\vec{D} = \epsilon E \tag{$\epsilon=\epsilon_0(1+\mathcal{X}_e)$: permittivity}
$$
We can also define the relative permittivity, also known as the dielectric constant:
$$
\epsilon_r = 1 + \mathcal{X}_e = \frac{\epsilon}{\epsilon_0}
$$
This value depends on the material. (Fun fact: $\sqrt{\epsilon_r} = \text{refractive index}$)

### Capacitors
##### Energy
If we charge from $q$ to $q + dq$:
$$
\begin{align}
dW &= V(q)\,dq \\
&= \frac{q}{C}\,dq\\
W &= \int_{0}^Q \frac{q}{C}\,dq = \frac{1}{2} \frac{Q^2}{C}
\end{align}
$$
therefore,
$$
W = \frac{1}{2}CV^2
$$
i.e., the energy stored in a capacitor is increased with increasing capacitance (using dielectric).

Electrostatic energy in dielectrics can be expressed as:
$$
W = \frac{\epsilon_0}{2} \int\epsilon_rE^2\,d\tau = \frac{1}{2} \int \vec{D} \cdot \vec{E}\,d\tau
$$
versus equation in vacuum:
$$
W = \frac{\epsilon_0}{2} \int E^2\,d\tau
$$
### Boundary Conditions in Dielectrics
Previous findings still hold, though free and bound charges need to be considered for $\sigma$, such that
$$
\begin{align}
E_\text{above}^\perp - E_\text{below}^\perp &= \frac{1}{\epsilon_0}\sigma \\
\vec{E}_\text{above}^\parallel &= \vec{E}_\text{below}^\parallel
\end{align}
$$
Using the boundary conditions of $\vec{D}$:
$$
\begin{align}
D_\text{above}^\perp - D_\text{below}^\perp &= \sigma_f \\
\vec{D}_\text{above}^\parallel-\vec{D}_\text{below}^\parallel &= \vec{P}_\text{above}^\parallel - \vec{P}_\text{below}^\parallel
\end{align}
$$
For linear dielectrics:
