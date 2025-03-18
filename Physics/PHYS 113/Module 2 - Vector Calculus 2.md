### Coordinate Systems
##### Cartesian Coordinates
Based on the $\hat{x}$, $\hat{y}$, and $\hat{z}$ unit vectors. Format is $(x,y,z)$
##### Cylindrical Coordinates
Based on the $\hat{\rho}$, $\hat{\phi}$, and $\hat{z}$ unit vectors. Format is $(\rho,\phi,z)$
##### Spherical Coordinates
Based on the $\hat{r}$, $\hat{\theta}$, and $\hat{\phi}$ unit vectors. Format is $(r,\theta,\phi)$

![[Coordinate System.png|400]]

### Coordinate System Equations
$$
\begin{align}
x = \rho \cos \phi && y = \rho \sin \phi && z = r \cos \theta \\
r = \sqrt{ x^2+y^2+z^2} && \rho = \sqrt{ x^2+y^2 } && \rho = r \sin \theta
\end{align}
$$
Note that $\phi$ always starts from $+x$, CCW; $\theta$ always starts from $+z$, going down to $\rho$.
### Unit Vectors
For cylindrical coordinates:
![[x y plane.png|400]]
$$
\begin{align}
\begin{bmatrix}
\hat{x} \\ \hat{y}
\end{bmatrix}
=
\begin{bmatrix}
\cos \phi & -\sin \phi \\
\sin \phi & \cos \phi
\end{bmatrix}
\begin{bmatrix}
\hat{\rho} \\
\hat{\phi}
\end{bmatrix}
&&
\begin{bmatrix}
\hat{\rho} \\ \hat{\phi}
\end{bmatrix}
=
\begin{bmatrix}
\cos \phi & \sin \phi \\
-\sin \phi & \cos \phi
\end{bmatrix}
\begin{bmatrix}
\hat{x} \\
\hat{y}
\end{bmatrix}
\end{align}
$$

![[z rho plane.png|400]]
$$
\begin{align}
\begin{bmatrix}
\hat{\theta} \\ \hat{r}
\end{bmatrix}
=
\begin{bmatrix}
\cos \phi & -\sin \phi \\
\sin \phi & \cos \phi
\end{bmatrix}
\begin{bmatrix}
\hat{\rho} \\
\hat{z}
\end{bmatrix}
&&
\begin{bmatrix}
\hat{\rho} \\ \hat{z}
\end{bmatrix}
=
\begin{bmatrix}
\cos \phi & \sin \phi \\
-\sin \phi & \cos \phi
\end{bmatrix}
\begin{bmatrix}
\hat{\theta} \\
\hat{r}
\end{bmatrix}
\end{align}
$$
This implies that the non-cartesian coordinates are position dependent, and so their unit vectors are dependent on the position of the point.
### Gradient of Cylindrical and Spherical
Given generalized coordinates $(q_1, q_2, q_3)$ with position vector $\vec{r} = x \hat{x} + y \hat{y} + z \hat{z} = \vec{r}(q_1,q_2,q_3)$:
$$
\vec{\nabla}f = \frac{1}{h_1} \frac{\partial f}{\partial q_1} + \frac{1}{h_2} \frac{\partial f}{\partial q_2} + \frac{1}{h_3} \frac{\partial f}{\partial q_3}
$$
where $\displaystyle h_1 = \left|\frac{\partial \vec{r}}{q_1}\right|$ and the same pattern for the rest of the partial derivatives.
##### Table of Coordinates

| Generalized (Curvilinear) | $h_1$ | $q_1$  | $\hat{e}_1$  | $h_2$  | $q_2$    | $\hat{e}_2$    | $h_3$          | $q_3$  | $\hat{e}_3$  |
| ------------------------- | ----- | ------ | ------------ | ------ | -------- | -------------- | -------------- | ------ | ------------ |
| Cartesian                 | $1$   | $x$    | $\hat{x}$    | $1$    | $y$      | $\hat{y}$      | $1$            | $z$    | $\hat{z}$    |
| Cylindrical               | $1$   | $\rho$ | $\hat{\rho}$ | $\rho$ | $\phi$   | $\hat{\phi}$   | $1$            | $z$    | $\hat{z}$    |
| Spherical                 | $1$   | $r$    | $\hat{r}$    | $r$    | $\theta$ | $\hat{\theta}$ | $r\sin \theta$ | $\phi$ | $\hat{\phi}$ |
### Divergence and Curl of a Generalized Coordinate Vector
Given generalized coordinates $(q_1, q_2, q_3)$ with position vector $\vec{r} = x \hat{x} + y \hat{y} + z \hat{z} = \vec{r}(q_1,q_2,q_3)$:
$$
\vec{\nabla} \cdot \vec{v} = \frac{1}{h_1h_2h_3}\left[ \frac{\partial}{\partial q_1}(h_2h_3v_1) + \frac{\partial}{\partial q_2}(h_3h_1v_2) + \frac{\partial}{\partial q_3}(h_1h_2v_3) \right]
$$
and
$$
\vec{\nabla} \times \vec{v} =
\begin{vmatrix}
h_1\hat{e}_1 & h_2\hat{e}_2 & h_3\hat{e}_3 \\
\frac{\partial}{\partial q_1} & \frac{\partial}{\partial q_2} & \frac{\partial}{\partial q_3} \\
h_1v_1 & h_2v_2 & h_3v_3
\end{vmatrix}
$$