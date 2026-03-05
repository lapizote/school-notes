### Electric Field
##### Coulomb's Law
Defined as
$$
F_i = \frac{1}{4\pi \epsilon_0} \frac{q_iQ}{\mathscr{r}_i^2} \hat{\mathscr{r}}_i
$$
where $\mathscr{r} = r-r_i'$

Force induced by an electric field is
$$
\vec{F} = Q\vec{E}
$$
where electric field (induced by discrete charges) is
$$
\vec{E}(r) = \frac{1}{4\pi \epsilon_0} \sum_{i=1}^n \frac{q_{i}}{\mathscr{r}_i^2}\hat{\mathscr{r}}_i
$$
where principle of superposition holds. If we only care about one source charge $q$, then
$$
\vec{E}(r) = \frac{1}{4\pi\epsilon_0} \frac{q}{r^2}\hat{r}
$$

For continuous charge distribution:
$$
\vec{E}(r) = \frac{1}{4\pi\epsilon_0}\int \frac{1}{\mathscr{r}^2}\hat{\mathscr{r}}\,dq
= \frac{1}{4\pi\epsilon_0} \int \frac{\rho(\vec{r}')}{\mathscr{r}^2}\hat{\mathscr{r}}\,d\tau
$$
where $\rho$ refers to a given charge distribution over a spatial unit $\tau$.

### Gauss' Law
Electric field flux is defined as
$$
\Phi_E = \int_S \vec{E} \cdot d\vec{a}
$$
i.e. the measure of the number of field lines passing through area surface $S$.

Gauss' law relates this to the flux of a closed surface as
$$
\oint \vec{E}\cdot d\vec{a} = \frac{1}{\epsilon_0}Q_\text{enc}
$$
where $Q_\text{enc}$ refers to the enclosed charge in the surface.

In differential form, Gauss' Law can be expressed as
$$
\nabla \cdot \vec{E} = \frac{1}{\epsilon_0}\rho
$$
### Dirac Delta Function
Not a function per se---infinitely high, infinitesimally narrow, defined as
$$
\delta(x) = \begin{cases}
0, &\text{if $x\neq 0$}\\
\infty, &\text{otherwise}
\end{cases}
$$
such that
$$
\int_{-\infty}^{\infty} \delta(x)\,dx = 1
$$
##### Properties
Since $f(x)\delta(x) = f(0)\delta(x)$,
$$
\int_{-\infty}^{\infty}f(x)\delta(x)\,dx = f(0)
$$
Shifting property:
$$
\int_{-\infty}^{\infty}f(x)\delta(x-a)\,dx=f(a)
$$
and
$$
\int_{-\infty}^{\infty}f(x)\delta(kx)\,dx=\frac{1}{|k|}f(0)
$$

##### 3D Dirac Delta
The 3D Dirac Delta function is defined as
$$
\delta^3(\vec{r}) = \delta(x)\delta(y)\delta(z)
$$
such that
$$
\int_\text{all space}\delta^3(\vec{r})\,d\tau=\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}\delta(x)\delta(y)\delta(z)\,dxdydz = 1
$$
### Curl of Electric Field
For any closed loop, we know that $\oint \vec{E} \cdot d\vec{l} = 0$.
Using [[Stoke's Theorem]]:
$$
\nabla \times \vec{E} = 0
$$
### Potential
Electric potential is defined as
$$
V(\vec{r}) = -\int_{\mathcal{O}}^r \vec{E} \cdot d\vec{l}
$$
where $\mathcal{O}$ is the reference point.

Since integral does not depend on the path, then the following are equivalent:
- $\displaystyle \nabla \times \vec{E} = 0$
- $\displaystyle \oint \vec{E} \cdot d\vec{l} = 0$
- $\displaystyle \int_a^b \vec{E} \cdot d\vec{l}$ is path independent
[[Gradient Theorem]] also gives us
$$
\vec{E} = -\nabla V
$$
