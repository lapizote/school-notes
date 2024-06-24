Given vectors 
$$
\begin{align}
\vec{a} = a_x\hat{i} + a_y\hat{j} + a_z\hat{k} \\
\vec{b} = b_x\hat{i} + b_y\hat{j} + b_z\hat{k}
\end{align}
$$
Then
$$
\begin{align}
\vec{a} \times \vec{b} =
	(a_yb_z - a_zb_y)\hat{i}
	+(a_zb_x - a_xb_z)\hat{j}
	+(a_xb_y - a_yb_x)\hat{k}
\end{align}
$$

### Physicist's Definition
$\vec{a} \times \vec{b}$ is a vector that is:
- Perpendicular to both $\vec{a}$ and $\vec{b}$.
- Has magnitude $|\vec{a}||\vec{b}|\sin\theta$ (where $\theta$ is the angle between $\vec{a}$ and $\vec{b}$).
- Has a direction as given by the right hand rule (thumb is the direction of the cross product, the curl is the direction from $\vec{a}$ to $\vec{b}$).

Note that the cross product is anticommutative, so
$$
\vec{b} \times \vec{a} = - (\vec{a} \times \vec{b})
$$
### Proof for the Formula
Given unit vectors $\hat{i}$, $\hat{j}$, and $\hat{k}$,

We can then determine the cross products of the components of any vectors:
$$
\begin{align}
\hat{i} \times \hat{j} &= \hat{k} \tag{1} \\
\hat{k} \times \hat{i} &= \hat{j} \tag{2} \\
\hat{j} \times \hat{k} &= \hat{i} \tag{3}
\end{align}
$$
Using these and the [[#Physicist's Definition|anticommutative property]] of cross products, we can then derive a general formula for the cross product of two three-dimensional vectors as follows (note that $\vec{a} \times \vec{a} = 0$):
$$
\begin{align}
\vec{a} \times \vec{b} &= 
	\left(a_x\hat{i} + a_y\hat{j} + a_z\hat{k}\right) \times \left(b_x\hat{i} + b_y\hat{j} + b_z\hat{k}\right)
\\
&=
	a_xb_y\hat{k} - a_xb_z\hat{j} - a_yb_x\hat{k} + a_yb_z\hat{i} + a_zb_x\hat{j} - a_zb_y\hat{i}
\\
&=
	(a_yb_z - a_zb_y)\hat{i}
	+(a_zb_x - a_xb_z)\hat{j}
	+(a_xb_y - a_yb_x)\hat{k}
\end{align}
$$

### Matrix Notation
A cross product can also be shown through matrix notation. For example:
$$
\begin{align}
\vec{a} \times \vec{b} =
	\begin{vmatrix}
	\hat{i} & \hat{j} & \hat{k} \\
	a_x & a_y & a_z  \\
	b_x & b_y & b_z
	\end{vmatrix}
\end{align}
$$

### Scalar Triple Product
Given three vectors  $\vec{a}$, $\vec{b}$, and $\vec{c}$, we can find their triple product by:
$$
\vec{a} \cdot (\vec{b} \times \vec{c}) =
\begin{vmatrix}
	a_x & a_y & a_z \\
	b_x & b_y & b_z \\
	c_x & c_y & c_z \\
\end{vmatrix}
$$
Note that in this case $\vec{a}$ acts as the unit vector.

#### Cyclic Permutation
$\vec{a} \cdot (\vec{b} \times \vec{c})$ can also be expressed as:
$$
\begin{align}
	\vec{b} \cdot (\vec{c} \times \vec{a}) \tag{1} \\
	\vec{c} \cdot (\vec{a} \times \vec{b}) \tag{2}
\end{align}
$$
