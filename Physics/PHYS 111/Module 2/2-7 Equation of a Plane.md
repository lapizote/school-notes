 The equation of a plane is
$$
Ax + By + Cz = D
$$
where $A$, $B$, $C$, and $D$ are constants.

#### Proof
In 3-D spaces, there is a unique perpendicular direction to any given plane.

Given two vectors $\vec{r}$ and $\vec{r_0}$ whose endpoints lie on the plane and $\vec{N}$ which is a vector perpendicular to the surface of the plane:
![[plane1.PNG]]
We can say that $\vec{r}-\vec{r_0}$ is perpendicular to $\vec{N}$ as it lies on the plane. This means that
$$
(\vec{r}-\vec{r_0}) \cdot \vec{N} = 0
$$
since $\cos90\degree = 0$.

We can then expand the LHS and separate the components of $\vec{r}$ and $\vec{r_0}$:
$$
\begin{align}
(x-x_0)N_x + (y-y_0)N_y + (z-z_0)N_z &= 0 \\
N_xx + N_yy + N_zz &= N_xx_0 + N_yy_0 + N_zz_0
\end{align}
$$
The components of $\vec{N}$ and $\vec{r_0}$ are constants, so
$$
\begin{align}
A &= N_x \tag{1} \\
B &= N_y \tag{2} \\
C &= N_z \tag{3} \\
D &= N_xx_0 + N_yy_0 + N_zz_0 \tag{4}
\end{align}
$$

