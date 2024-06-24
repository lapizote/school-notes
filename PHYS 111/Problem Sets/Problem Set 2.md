1. The Valence Shell Electron Pair Repulsion (VSEPR) Theory predicts that, in a molecule such as methane ($CH_4$), where the carbon atom is covalently bonded to four hydrogen atoms, the atoms will be positioned at the vertices of a tetrahedron centered at the carbon atom. Thus, if $\hat{e}_1$, $\hat{e}_2$ $\hat{e}_3$ and $\hat{e}_4$ are unit vectors from the carbon atom to each hydrogen atom, then symmetry implies that $\hat{e}_1 + \hat{e}_2 + \hat{e}_3 + \hat{e}_4 = \vec{0}$, and also the angle between any two of these unit vectors in the same. Find the *exact* value of this angle, and its approximate value in degrees.

	**Solution:**
	We had this question before in PHYS 31.1, so we had an idea of how this works.

	![[pset2-1.PNG]]

	Let $\theta$ be the angle between any two unit vectors $\hat{e}_i$.

	Note that $(1)$ can apply to any two pairs of unit vectors.
	$$
	\begin{align}
	\hat{e}_1 \cdot \hat{e}_2 &= \cos\theta \tag{1} \\\\

	\hat{e}_1 + \hat{e}_2 + \hat{e}_3 + \hat{e}_4 &= \vec{0} \\
	\hat{e}_1 \cdot (\hat{e}_1 + \hat{e}_2 + \hat{e}_3 + \hat{e}_4) &= \hat{e}_1 \cdot \vec{0} \\
	1 + \hat{e}_1 \cdot \hat{e}_2 + \hat{e}_1 \cdot \hat{e}_3 + \hat{e}_1 \cdot \hat{e}_4 &= 0 \tag{2}
	\end{align}
	$$

	By $(1)$ and $(2)$:
	$$
	\begin{align}
	1 + 3 \cos\theta &= 0\\
	\cos\theta &= -\frac{1}{3} \\
	\theta &= \cos^{-1}\left({-\frac{1}{3}}\right) \approx 109.47\degree
	\end{align}
	$$
2. Let $\hat{n}$ be a fixed unit vector, and $\theta$ a real number. Define the function $R_{\theta\hat{n}}$ acting on a vector $\vec{v}$ as follows:
	$$
	R_{\theta\hat{n}}(\vec{v}) = (\vec{v} \cdot \hat{n})\hat{n} + (\cos\theta)[\vec{v} - (\vec{v} \cdot \hat{n})\hat{n}] + (\sin\theta)(\hat{n} \times \vec{v})
	$$
	Determine, and express in your own words, the geometric relationship between an arbitrary vector $\vec{v}$ and $R_{\theta\hat{n}}(\vec{v})$. Draw as many diagrams as needed to visualize your explanation.

	**Solution (and process):**
	To be honest we saved this question for last. Doing the other questions first kind of helped us understand this problem more, as we realized that
	- $(\vec{v} \cdot \hat{n})\hat{n}$ is essentially $\text{proj}_\hat{n}d$, or the component of $\vec{v}$ parallel to $\hat{n}$.
	- $(\vec{v} - (\vec{v} \cdot \hat{n})\hat{n})$ is the component of $\vec{v}$ perpendicular to $\hat{n}$.
	- $\hat{n} \times \vec{v}$ is a direction that is perpendicular to both $\hat{n}$ and $\vec{v}$.

	![[pset_2-2_2.PNG]]
	
	Essentially, you can imagine three axes that all have the direction of $\hat{n}$ as a reference point, as shown above.
	
	So one can interpret $R_{\theta\hat{n}}(\vec{v})$ as decomposed into three different terms:

	The first term can be interpreted as is (which is $\text{proj}_\hat{n}d$), where it is a value that is parallel to the first axis (directed by $\hat{n}$). The lower the angle between $\vec{v}$ and $\hat{n}$, the higher this value.

	The second term is the perpendicular component that scales with $\cos\theta$, such that it gets closer to 0 as $\theta$ gets closer to either of the two extremes ($0\degree$ and $90\degree$) meaning that the max value is somewhere between those extremes. This is parallel to the second axis (that is perpendicular to $\hat{n}$).
	
	![[pset2-2_1.PNG]]
	
	The third term can be interpreted as a value parallel to the third dimension/axis that simply scales inversely with $\cos\theta$, since the former increases as the latter decreases (and vice versa).
	
3. A proton is initially at the point $(-52,89,-8.0) \times 10^-16 \, m$ and moving with a velocity of $(3.0\hat{i}-4.0\hat{j}+1.0\hat{k} \times 10^6 \, m/s$. A second proton is at rest and located at the origin.

	a. Find the impact parameter b, which is the distance between the two protons when the moving one reaches its closest point of approach, assuming the moving proton continues to move in a straight line and the proton at rest stays at rest.

	**Solution:**
	This is similar to an example that we did in class, so this was not too hard to figure out.
	We defined the function of the moving proton's position as
	 $$
		 P_1(t) = (-52\hat{i} + 89\hat{j} - 8\hat{k})\times10^-16\,m
		 + t(3\hat{i} - 4\hat{j} + \hat{k}) \times 10^6
	 $$
	where $t$ is the time elapsed and the stationary proton's position as
	 $$
		 P_2(t) = 0
	 $$
	To save time, we used the graphical solution instead of the calculus solution.

	We can then construct a graph involving the movement of the proton, its initial point, and the position of the second proton.

	As we have established in class, we can find distance $d$ through
	![[pset2-3_1.PNG]]
	$$
	d = \sin\theta|\vec{s}|
	$$
	and
	$$
	|\vec{v} \times \vec{s}| = |\vec{v}| |\vec{s}| \sin\theta
	$$
	where $\vec{v}$ is the velocity of $P_1$ and $\vec{s}$ is the initial distance of $P_1$ from $P_2$.

	Isolating $|\vec{s}|\sin\theta$ and finding $|\vec{v}|$:
	$$
	\begin{align}
	|\vec{v}| &= \sqrt{3^2+4^2+1^2} \times 10^6 = \sqrt{26} \times 10^6 m/s \tag{1} \\
	
	|\vec{s}| \sin\theta &= \frac{|\vec{v} \times \vec{s}|}{|\vec{v}|} \tag{2} \\

	|\vec{v} \times \vec{s}| &= \begin{vmatrix}
			\hat{i} & \hat{j} & \hat{k} \\
			3 \times 10^6 & -4 \times 10^6 & 10^6 \\
			-52 \times 10^{-16} & 89 \times 10^{-16} & -8 \times 10^{-16}
		\end{vmatrix} \tag{3} \\\\\\
		
	&= | -5.7 \times 10^{-9} -2.8 \times 10^{-9} +0.59 \times 10^{-8} | \\
	&= \sqrt{7.514 \times 10^{-17}} \\\\

	|\vec{s}| \sin\theta &= \frac{\sqrt{7.514 \times 10^{-17}}}{\sqrt{26} \times 10^6} \tag{1 and 2 and 3} \\

	&= 1.7 \times 10^{-15} \, m
	\end{align}
	$$

	b. If a moving proton continues to move at constant velocity, at what time will it reach its closest point of approach to the stationary proton?

	**Solution:**
	First, we find $|\vec{s}|$.
	$$
	\begin{align}
	|\vec{s}| &= \sqrt{((-52)^2+89^2+(-8)^2)\times(10^{-16})^2} \\
	&= \sqrt{1.0689\times10^{-28}}
	\end{align}
	$$
	
	We can use both Pythagorean and the displacement formula to our advantage:
	![[pset2-3_2.PNG]]
	$$
	\begin{align}
	|a|^2 + (1.7\times10^{-15})^2 &= 1.0689 \times 10^{-28} \\
	|a| &= \sqrt{ 1.0689 \times 10^{-28} - (1.7\times10^{-15})^2 } \tag{1} \\\\
	\end{align}
	$$
	$$
	\begin{align}
	a &= P_1(t) - (-52\hat{i} + 89\hat{j} - 8\hat{k}) \times 10^{-16} \\
	a &= (3 \times 10^6\hat{i} - 4 \times 10^6\hat{j} + 10^6\hat{k})t \\
	|a| &= t\sqrt{ (3 \times 10^6)^2 + (-4 \times 10^6)^2 + (10^6)^2 } \tag{2}
	\end{align}
	$$
	We can then use $(1)$ and $(2)$:
	$$
	\begin{align}
	t &= 
	\frac{
		\sqrt{ 1.0689 \times 10^{-28} - (1.7\times10^-15)^2 }
	}
	{
		\sqrt{ (3 \times 10^6)^2 + (-4 \times 10^6)^2 + (10^6)^2 }
	} \\
	&= 2\times10^{-21}\, s
	\end{align}
	$$

	c. What are the coordinates of this closest point of approach?

	**Solution:**
	We can simply use both the time and parametric equations formed from the position function:
	$$
	\begin{align}
	x &= -52\times10^{-16} + 2\times10^{-21} \times 3 \times 10^6 m \\
	y &= 89\times10^{-16} + 2\times10^{-21} \times -4 \times 10^6 m \\
	z &= -8\times10^{-16} + 2\times10^{-21} \times 10^6 m \\\\

	x &= 8\times10^{-16} m \\
	y &= 9\times10^{-16} m \\
	z &= 12\times10^{-16} m \\
	\end{align}
	$$

	so our coordinates are $(8, 9, 12)\times10^{-16} \,m$.
	
4. A ray of light is traveling along the x-axis, in the negative x-direction, when it encounters a plane mirror oriented so that its equation is 2x + 3y + 6z = 12.
	a. What point on the mirror does the ray of light strike?
	
	**Solution:**
	We know that the light only moves along the x-axis, so it will always have its y-coordinates and z-coordinates as zero. As such, we then know that its point of intersection with the mirror is at position $(x, 0, 0)$.

	To find $x$, we can simply make use of the plane equation by substituting $y$ and $z$ with our known values:
	$$
	\begin{align}
	2x + 3(0) + 6(z) &= 12 \\
	2x &= 12 \\
	x &= 6
	\end{align}
	$$
	So that means our point of intersection is $(6, 0, 0)$.

	b. Find a unit vector normal to the mirror.

	**Solution:**
	Let us define the mirror as plane $E$.
	Through the proof used to obtain the equation of a plane:
	$$
	\begin{align}
	N_xx + N_yy + N_zz &= 2x + 3y + 6z \tag{1} \\\\
	\end{align}
	$$
	$$
	\begin{align}
	\vec{N} &= N_x\hat{i} + N_y\hat{j} + N_z\hat{k} \\
	&= 2\hat{i} + 3\hat{j} + 6\hat{k} \tag{through (1)}
	\end{align}
	$$
	And to find the unit vector:
	$$
	\begin{align}
	\hat{n} &= \frac{\vec{N}}{|\vec{N}|} \\
	&= \frac{2\hat{i} + 3\hat{j} + 6\hat{k}}{\sqrt{2^2 + 3^2 + 6^2}} \\
	&= \frac{2}{7}\hat{i} + \frac{3}{7}\hat{j} + \frac{6}{7}\hat{k}
	\end{align}
	$$
	c. Find an equation for the plane of incidence, which is the plane

	Solution: This answer to this one felt weird at first because it *feels* wrong (because x-component is 0), but it actually is correct.

	Since we already know the normal vector to the surface of $E$ and the vector of the incident ray, we can simply use
	$$
	\vec{N_i} = \vec{N} + \vec{v}
	$$
	where $\vec{N_i}$ is the normal of the incident plane, $\vec{N}$ is the normal of the plane of the glass, and $\vec{v}$ is the vector of the incident ray.

	So
	$$
	\begin{align}
	\vec{N_i} &=
		\begin{vmatrix}
			\hat{i} & \hat{j} & \hat{k} \\
			2 & 3 & 6 \\
			-1 & 0 & 0
		\end{vmatrix} \\
	
	&= -6\hat{j} + 3\hat{k}
	\end{align}
	$$
	After using the point $(-1, 0, 0)$ (from $\vec{v}$), our plane would then be $-6y+3z = 0$ or $6y-3z = 0$.

	d. Find a unit vector along the reflected ray.

	**Solution:**
	Pretty confusing at first, and we were stumped on this. However, we did come to realize that a reflection of a vector can be defined as the "reversal" of a vector's component parallel to the normal (much like how a bouncing ball has its vertical velocity "reversed" after it hits the ground).

	Finding the components of $\vec{v}$ parallel and perpendicular to $\vec{N}$:

	$$
	\begin{align}
	\vec{v}_\parallel &= \frac{\vec{v} \cdot \vec{N}}{|\vec{N}|^2}\vec{N} \\
	&= \frac{(-\hat{i}) \cdot (2\hat{i} + 3\hat{j} + 6\hat{k})}{49} (2\hat{i} + 3\hat{j} + 6\hat{k}) \\
	&= (2\hat{i} + 3\hat{j} + 6\hat{k})(-\frac{2}{49}) \\
	&= -\frac{4}{49}\hat{i} - \frac{6}{49}\hat{j} - \frac{12}{49}\hat{k}
	\end{align}
	$$
	$$
	\begin{align}
	\vec{v}_\perp &= \vec{v} - \vec{v}_\parallel \\
	&= -\hat{i} - (-\frac{4}{49}\hat{i} - \frac{6}{49}\hat{j} - \frac{12}{49}\hat{k}) \\
	&= -\frac{45}{49}\hat{i} + \frac{6}{49}\hat{j} + \frac{12}{49}\hat{k}
	\end{align}
	$$
	We then multiply the parallel component by $-1$ to get $\frac{4}{49}\hat{i} + \frac{6}{49}\hat{j} + \frac{12}{49}\hat{k}$. Adding this with $\vec{v}_\perp$ gives us
	$$
	-\frac{41}{49}\hat{i} + \frac{12}{49}\hat{j} + \frac{24}{49}\hat{k}
	$$
	The magnitude is $1$, so this is the answer for 4d.

	*"Fun fact: This video reminds me of the youtube video 'Fast Inverse Square Root - A Quake III Algorithm' which talked about Id's black sorcery that is the 0x5f3759df algorithm. Very cool application of vectors." - Axl*