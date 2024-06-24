3. A proton is initially at the point $(-52,89,-8.0) \times 10^-16 \, m$ and moving with a velocity of $(3.0\hat{i}-4.0\hat{j}+1.0\hat{k} \times 10^6 \, m/s$. A second proton is at rest and located at the origin.

	a. Find the impact parameter b, which is the distance between the two protons when the moving one reaches its closest point of approach, assuming the moving proton continues to move in a straight line and the proton at rest stays at rest.

	Solution:
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

4. A ray of light is traveling along the x-axis, in the negative x-direction, when it encounters a plane mirror oriented so that its equation is 2x + 3y + 6z = 12.
	a. What point on the mirror does the ray of light strike?
	
	Solution:
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

	Solution:
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
	c. Find an equation for the line of incidence, which is the plane

	Solution: This answer to this one felt weird at first because it *feels* wrong (because x-component is 0), but it actually is correct.

	Since we already know the normal vector to the surface of $E$ and the incident of