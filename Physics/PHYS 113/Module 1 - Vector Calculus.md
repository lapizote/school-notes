### Review
Vectors in 3d space can be expressed as
$$
\vec{v} = v_x \hat{i} + v_y \hat{j} + v_z \hat{k}
$$
Adding vectors involves adding their individual components, and scalar multiplication involves multiplying all the components by a factor.

##### Dot Product:
$$
\begin{align}
\vec{v} \cdot \vec{w} &= v_x w_x + v_y w_y + v_z w_z \\
&= |\vec{v}||\vec{w}|\cos \theta \\
&= \text{proj}_w(\vec{v}) \cdot |\vec{w}| \\
&= \text{proj}_v(\vec{w}) \cdot |\vec{v}|
\end{align}
$$
##### Cross Product:
$$
\begin{align}
	\vec{v} \times \vec{w} &= 
	\det\left(\begin{vmatrix}
	 \hat{i} & \hat{j} & \hat{k} \\
	\hat{v_x} & \hat{v_y} & \hat{v_z} \\
	\hat{w_x} & \hat{w_y} & \hat{w_z}
	\end{vmatrix}\right) \\
\end{align}
$$
Also remember that
$$
|\vec{v} \times \vec{w}| = |\vec{v}||\vec{w}| \sin \theta
$$
### Precise Definition of a Vector
##### (In 2-D)
A vector is a pair of quantities $(v_x, v_y)$ whose components transform in the same way as the coordinates when the coordinate system is rotated. In other words, in a new coordinate system that is rotated $\theta$ counterclockwise from the original:
$$
\begin{align}
v_{x'} &= v_x \cos \theta + v_y \sin \theta \\
v_{y'} &= -v_x \sin \theta + v_y \cos \theta \\
\end{align}
$$
or
$$
\begin{bmatrix}
v_{x'} \\
v_{y'}
\end{bmatrix}
=
\begin{bmatrix}
\cos \theta  & \sin \theta \\
-\sin \theta  &  \cos \theta
\end{bmatrix}
\begin{bmatrix}
v_x \\
v_y
\end{bmatrix}
$$
(A scalar would then be a quantity that is the same in all coordinate systems.)

##### (In 3-D)
$$
\begin{bmatrix}
v_{x'} \\
v_{y'} \\
v_{z'}
\end{bmatrix}
=
\begin{bmatrix}
\cos \theta_{x'x} & \cos \theta_{x'y} & \cos \theta_{x'z} \\
\cos \theta_{y'x} & \cos \theta_{y'y} & \cos \theta_{y'z} \\
\cos \theta_{z'x} & \cos \theta_{z'y} & \cos \theta_{z'z}
\end{bmatrix}
\begin{bmatrix}
v_x \\
v_y \\
v_z
\end{bmatrix}
$$
### Directional Derivative
The rate of change of a scalar field when moving along a direction.
Example:
$$
\begin{align}
	\frac{\partial f}{\partial q} &= a\frac{\partial f}{\partial x} + b\frac{\partial f}{\partial y} + c\frac{\partial f}{\partial z} \\
	&= (a\hat{i} + b\hat{j} + c\hat{k}) \cdot (\frac{\partial f}{\partial x} \hat{i} + \frac{\partial f}{\partial y} \hat{j} + \frac{\partial f}{\partial z} \hat{k}) \\
	&= \hat{e} \cdot \vec{\nabla}f 
\end{align}
$$
The first term is the direction. The second term is the gradient of the scalar field $f$.
##### Gradient
The gradient is a vector in the greatest rate of change, whose magnitude is the rate of change. It can also act as a differential operator:
$$
\vec{\nabla} = \frac{\partial}{\partial x}\hat{i} + \frac{\partial}{\partial y}\hat{j} + \frac{\partial}{\partial z}\hat{k}
$$
In any level surface, the direction of this gradient at a point will be perpendicular to the tangent plane at that same point (i.e. it is perpendicular to any tangent line at that point). This is important for [[#Surface Integrals]].

The gradient of any scalar field is a vector field.

## Line Integrals and Surface Integrals
### Line Integrals
A line integral of a vector field along a path is
$$
\int_C \vec{v}\cdot d\vec{r}
$$
where $d\vec{r}$ is the infinitesimal displacement, i.e. $dx \hat{i} + dy \hat{j} + dz \hat{k}$.

#### Strategies to Solve Line Integrals:
##### Manual
Express everything as a single variable. Use polar coordinates or parametric equations if necessary.
##### Fundamental Theorem of Gradients/Line Integrals
This only applies to gradients.
$\vec{\nabla}f \cdot d\vec{r} = df$, so
$$
\int_C \vec{\nabla}f \cdot d\vec{r} = \int_C df = f(\vec{r_2}) - f(\vec{r_1})
$$
#### Stokes' Theorem and Curl
The curl of a vector is
$$
\vec{\nabla} \times \vec{v}
= \begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
v_x & v_y & v_z
\end{vmatrix}
$$
Physically, it can be interpreted as the axis at which a vector field rotates/curls around.

Through Stokes' theorem, we can use the curl to find closed line integrals.
$$
\oint_C \vec{v}\cdot d\vec{l} = \int_S(\vec{\nabla}\times \vec{v})\cdot d\vec{A}
$$
This applies regardless if planar or non-planar surfaces are considered.

### Surface Integrals/Flux
Given a vector field and a level surface:
$$
\int_S \vec{v} \cdot \hat{n} \,dA = \int_S \vec{v} \cdot d\vec{A}
$$
where $d\vec{A}$ is the vector with magnitude $dA$ and a direction perpendicular to the surface.
#### Closed/Gaussian Surface
$$
\oint_S \vec{v} \cdot d\vec{A} \tag{$d\vec{A}$ is always outward}
$$
Generally, it is evaluated separately for each face as we are trying to measure divergence.
Alternatively, we can use the Gauss' Divergence Theorem:
$$
\oint_S \vec{v}\cdot d\vec{A} = \int_V(\vec{\nabla} \cdot \vec{v}) \,d\tau
$$
where $\tau$ is $dxdydz$.

Intuitively, flux can be described in the analogy of fluid moving in or out a surface, where if it is multiplied by the density, it is the rate at which water exits the volume. A positive flux means it is losing fluid, negative means gaining fluid, and 0 means a steady flow.

