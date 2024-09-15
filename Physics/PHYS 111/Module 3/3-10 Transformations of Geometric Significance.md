Matrix of a rotation by an angle $\theta$
$$
R_\theta = 
	\begin{bmatrix}
		\cos\theta & -\sin\theta \\
		\sin\theta & \cos\theta
	\end{bmatrix}
$$
With a perpendicular rotation:
$$
	R =
	\begin{bmatrix}
		0 & -1 \\
		1 & 0
	\end{bmatrix}
$$

#### Intuitive Proof(?)
Given $\vec{v} = \begin{bmatrix} 1 \\ - 3 \end{bmatrix}$
Then
$$
\begin{align}
R_\theta\vec{v} &=
	\begin{bmatrix}
		\cos\theta & 3\sin\theta \\
		\sin\theta & -3\cos\theta
	\end{bmatrix}
\\\\
\vec{v} \cdot (R\vec{v}) &= |\vec{v}||R\vec{v}|\cos\theta
\\
&= \frac{ \vec{v} \cdot R\vec{v} }{ |\vec{v}||R\vec{v}| }
\\
&= \frac{ (\cos\theta + 3\sin\theta) - 3(\sin\theta - 3\cos\theta) }{ \sqrt{10}\sqrt{(\cos\theta + 3\sin\theta)^2 + (\sin\theta - 3\cos\theta)^2} }
\\
&= \frac{10\cos\theta}{\sqrt{10}\sqrt{10}} = \frac{10\cos\theta}{10}
\\
&= \cos\theta
\end{align}
$$