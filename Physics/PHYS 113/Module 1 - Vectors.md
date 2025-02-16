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
