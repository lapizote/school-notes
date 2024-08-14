## Module 1
$$
\sqrt{-1} =i
$$
#### Rectangular and Polar Forms
##### Rectangular to Polar Form:
1. Plot the complex number on the graph.
2. Determine the angle $\theta$ from positive x-axis (CCW is positive, CW is negative)
3. Determine the magnitude of the complex number through Pythagora's:
	$r = |z| = \sqrt{Re(z)^2+Im(z)^2}$
4. Polar form is $re^{i\theta}$
##### Polar Form to Rectangular
1. Just use the formula $r(\cos\theta + i\sin\theta)$.

#### Complex Conjugates
Given $z = x + iy$, its complex conjugate is $z^* = \bar{z} = x -iy$.
#### Finding roots
1. Convert to polar.
2. Find the angle equivalents (e.g. $\theta = -120\degree = 240\degree = 600\degree = 960\degree$). You will want to find as many angles as the degree of the root. Construct the polar expressions using those angles.
3. Find the $n^\text{th}$ root of each expression such that $$^{n}\sqrt{2}e^{\frac{i\theta}{n}}$$
#### Tips
1. Complex conjugate $z^*$ is just $z$ reflected across the $Re(x)$ axis.
2. $iz$ is $z$ rotated $90\degree$ CCW.
3. $|z_2-z_1|$ is the distance between $z_2$ and $z_1$.
---
## Module 2
#### Dot Product
Given two 3D vectors $\vec{a}$ and $\vec{b}$:
$$
\begin{align}
\vec{a} \cdot \vec{b} = a_xb_x + a_yb_y + a_zb_z = |\vec{a}||\vec{b}|\cos\theta
\end{align}
$$
Note that a dot product of the same vector gives us $\vec{a} \cdot \vec{a} = |\vec{a}|^2$.
#### Unit Vector
If $|\vec{a}| = 1$, then it is a unit vector.
To then find unit vector $\hat{n}$:
$$
\hat{n} = \frac{\vec{n}}{|\vec{n}|}
$$
#### Cross Product
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
##### Geometric interpretation:
$\vec{a} \times \vec{b}$ is a vector that is:
- Perpendicular to both $\vec{a}$ and $\vec{b}$.
- Has magnitude $|\vec{a}||\vec{b}|\sin\theta$ (where $\theta$ is the angle between $\vec{a}$ and $\vec{b}$).
- Has a direction as given by the right hand rule (thumb is the direction of the cross product, the curl is the direction from $\vec{a}$ to $\vec{b}$).

Note that the cross product is anticommutative, so
$$
\vec{b} \times \vec{a} = - (\vec{a} \times \vec{b})
$$
##### Cross Triple Product:
$$
\vec{a} \times (\vec{b} \times \vec{c})
$$
There also exists an identity for the cross triple product such that
$$
\vec{a} \times (\vec{b} \times \vec{c}) = \vec{b}(\vec{a} \cdot \vec{c}) - \vec{c}(\vec{a} \cdot \vec{b})
$$
#### Parametric Equations
Given $\vec{r}(t) = \vec{r_0} + \vec{v}t$:
Its parametric equations are:
$$
\begin{align}
	x = x_0 + v_xt \\
	y = y_0 + v_yt \\
	z = z_0 + v_zt
\end{align}
$$
#### Equation of a Plane
Given equation of a plane $Ax + By + Cz = D$ where where $A$, $B$, $C$, and $D$ are constants,
the normal vector $\vec{N}$ is $A\hat{i} + B\hat{j} + C\hat{k}$.

#### Projection of a vector
A projection of vector $\vec{a}$ onto $\vec{b}$ is:
$$
\text{proj}_{\vec{b}}\vec{a} = \frac{\vec{a}\cdot\vec{b}}{|\vec{b}|^2}\vec{b}
$$
Notice that $\frac{\vec{a}\cdot\vec{b}}{|\vec{b}|^2}$ scales down $\vec{b}$ for it to become a projection of $\vec{a}$ onto it.
Other alternative interpretations include:
$$
\begin{align}
\text{proj}_{\vec{\hat{n}}}\vec{v} &= (\vec{v} \cdot \hat{n})\hat{n} \tag{vector $\vec{v}$ to direction $\hat{n}$} \\
|\text{proj}_{\vec{b}}\vec{a}| &= |\vec{a}|\cos\theta \\
&= \frac{|\vec{a}|\vec{b}|\cos\theta}{|\vec{b}|}
\end{align}
$$
#### Tips
1. Given a vector line equation $\vec{r}(t)$ and any point on the plane, you can determine the plane parallel to it by finding the [[#Geometric interpretation|cross product]] of the line vector of $\vec{r}(t)$ and a vector between the point and any random point on $\vec{r}(t)$. (This also works with 3 points, just find the two vectors connecting at a single point)
2. In the plane equation, $D$ changes the "level" of the plane along its normal vector. Because of this, any plane with the same LHS but differing $D$ would be parallel to each other. (*wink wink problem 6 in LE2*)
3. A projection of a point onto a plane can be determined by creating a vector line equation. The point is $\vec{r}_0$, the normal vector line is $\vec{v}$. Then simply find $t$ by making use of the plane equation $Ax + By + Cz = D$, where $x$, $y$, and $z$ are the coordinates found through $\vec{r}(t)$.
4. A reflection of a vector is just its component parallel to the perpendicular of the surface turned negative (i.e. "reflected").
5. Distances between a point and a line can be determined by drawing a triangle with the point, a random point on the line, and the projection of the point on the line as vertices.
---
## Module 3
#### Transformations
##### 2D
$$
\begin{align}
R_\theta &=
	\begin{bmatrix}
		\cos\theta & -\sin\theta \\
		\sin\theta & \cos\theta
	\end{bmatrix} \tag{CCW Rotation at $\theta\degree$} \\

P_x &=
\begin{bmatrix}
		1 & 0 \\
		0 & 0
	\end{bmatrix} \tag{Projection at x-axis} \\

P_y &=
\begin{bmatrix}
		0 & 0 \\
		0 & 1
	\end{bmatrix} \tag{Projection at y-axis} \\

S_x &=
\begin{bmatrix}
		1 & 0 \\
		0 & -1
	\end{bmatrix} \tag{Reflection along x-axis} \\
	
S_y &=
\begin{bmatrix}
		-1 & 0 \\
		0 & 1
	\end{bmatrix} \tag{Reflection along y-axis} \\
\end{align}
$$
##### 3D
(Note: Multiply these matrices to the vector)

**Matrix that finds components of a vector to $\hat{n}$**
(Note: this is also the projection matrix onto unit vector $\hat{n}$)
$$
\begin{align}
P_{\parallel\hat{n}} = \hat{n}\hat{n}^T
\end{align}
$$
**To find vector perpendicular to $\hat{n}$:**
$$
\begin{align}
P_{\perp\hat{n}} = I_3 - P_{\parallel\hat{n}}
\end{align}
$$
**Reflection along $\hat{n}$**
$$
S_{\perp\hat{n}} = I_3-2P_{\perp\hat{n}}
$$
#### Algebraic Properties:
Note: $A$, $B$, and $C$ are matrices, $c$ and $d$ are scalar
1. $A + B$ = $B+A$
2. $(A+B) + C = A + (B + C)$
3. $c(A+B) = cA + cB$
4. $(c+d)A = cA + dA$
5. $c(dA) = (cd)A$
6. 
	-  $A(B+E) = AB + AE$
	- $(A+B)E = AE + BE$
1. $(AB)E = A(BE)$
2. $(A+B)^T = A^T + B^T$
3. $(cA)^T = cA^T$
4. $(AB)^T = B^TA^T$
5. $A(cB) = c(AB) = cAB$
#### Relation with Vectors
**Vectors as a matrix:**
$$
\vec{v} = \vec{v}_x\hat{i} + \vec{v}_y\hat{j} + \vec{v}_z\hat{k} =
	\begin{bmatrix}
		v_x \\ v_y \\ v_z
	\end{bmatrix}
$$
**Dot Product:** $$\vec{a} \cdot \vec{b} = \vec{a}^T\vec{b}$$

#### Determinants
##### Recursive Method (3D)
Given
$$
\begin{align}
A =
	\begin{vmatrix}
		a & b & c \\
		d & e & f \\
		g & h & i \\
	\end{vmatrix}
\end{align}
$$
Its determinant would then be
$$
\begin{align}
	a\det\left(\begin{vmatrix}
		e & f\\
		h & i
	\end{vmatrix}\right)
	-
	b\det\left(\begin{vmatrix}
		d & f\\
		g & i
	\end{vmatrix}\right)
	+
	c\det\left(\begin{vmatrix}
		d & e\\
		g & h
	\end{vmatrix}\right)
\end{align}
$$
where the smaller matrices are **cofactors**.
(Refer to the "checkerboard pattern" for determining whether the cofactor is positive or negative)
##### Theorems:
1. $\det(A^T) = \det(A)$
2. $\det(AB) = \det(A)\det(B)$
3. Determinant is unchanged if a multiple of one row is added to another row (or multiple of one column to another column).
#### Inverse of a Matrix
$$
A^{-1} = \frac{(\text{cof}(A))^T}{\det} = \frac{\text{adj}(A)}{\det{A}}
$$
#### Finding Eigenvalues
(with initial matrix $A$)
**Steps:**
1. Start with $\det(A-I_n\lambda) = 0$.
2. Find $\lambda$. These are your eigenvalues.
3. Through $A\vec{x} = \lambda\vec{x}$, use the resulting system of equations to find the values of $\vec{x}$.
#### Tips:
- A lot of the proving questions can be solved by introducing the inverse of a matrix (i.e. multiplying it into both LHS and RHS).
---
## Module 4
#### 1. Separable Equations
**Condition:** Given a FOODE, we can separate and isolate the two variables so we get $f(x) dx = g(y) dy$.

**Steps:**
1. Separate the two variables into the LHS and RHS.
2. Integrate both sides.
3. ???
4. Profit!
#### 2. Homogeneous Equations
**Condition:** Given an inseparable FOODE in the form
$$
M(x,y)\,dx + N(x,y)\,dy = 0 
$$
where $M(x,y)$ and $N(x,y)$ are [[Homogeneous Function|homogeneous functions]] of the same degree.

**Steps:**
1. Use the substitution $y = vx$ or $v = \frac{y}{x}$.
2. Using the substitution in Step 1, find that $dy = v\,dx + x\,dv$ (through the product rule).
3. Substitute $dy$ and $y$ with the equations that we found in Steps 1 and 2.
4. If the condition is met, certain terms should add up (or cancel out) such that we get a separable equation.
#### 3. Linear Equation
**Condition:** Given a linear FOODE that we can write in the form
$$
\frac{dy}{dx} + P(x)y = Q(x)
$$
where $P(x)$ and $Q(x)$ are functions solely in terms of $x$.

**Steps:**
1. Find the integrating factor, $\mu(x) = e^{\int P(x)\,dx}$.
2. Multiply both sides by $\mu(x)$.
3. The LHS can then be written as an exact derivative $\frac{d}{dx}(\mu(x)y)$ (thanks to the product rule).
4. Integrate both sides.

#### 4. Exact Functions of 2 Variables
**Condition:** Given an exact FOODE in the form
$$
M(x,y)\,dx + N(x,y)\,dy = 0 
$$
there should exist a $f(x,y)$ such that when
$$
\begin{align}
\frac{\delta f}{\delta x} = M(x,y) \,;
\frac{\delta f}{\delta y} = N(x,y)
\end{align}
$$
then
$$
\frac{\delta M}{\delta y} = \frac{\delta N}{\delta x}
$$

**Steps (Method 1):**
1. Integrate $\frac{\delta f}{\delta x} = M(x,y)$ (with respect to $x$) and $\frac{\delta f}{\delta y} = N(x,y)$ (with respect to $y$) to get $f(x,y) = \int M(x,y) + C(x)$ and $f(x,y) = \int M(x,y)\,dx + C(x)$ and $f(x,y) = \int N(x,y)\,dy + D(y)$.
2. There should be common terms and uncommon terms. The uncommon terms should be the values of $C(x)$ and $D(y)$.
3.  Construct the final expression using these terms.
4. Since $M(x,y)\,dx + N(x,y)\,dy=0$ should be interpreted as $df=0$, then simply equate the final expression to $C$.

**Steps (Method 2):**
1. Integrate $\frac{\delta f}{\delta x} = M(x,y)$ (with respect to $x$) to get $f(x,y) = \int M(x,y)\,dx + C(x)$.
2. We can then differentiate both sides to get $\frac{\delta f}{\delta x} = M(x,y) + \frac{dC}{dy}$.
3. We can then equate the equation found in Step 2 with $\frac{\delta f}{\delta y} = N(x,y)$.
4. Find $C(y)$ and then construct the final equation found from Step 1.
5. Since $M(x,y)\,dx + N(x,y)\,dy=0$ should be interpreted as $df=0$, then simply equate the final expression to $C$.
#### Tip:
When in doubt, try 1 first. Then check if they are exact (4). Then check if they are homogenous (2). Then check if you can make it linear (3). If none work, either you've done an algebra error or you need to do a non-standard change of variable (good luck!)
