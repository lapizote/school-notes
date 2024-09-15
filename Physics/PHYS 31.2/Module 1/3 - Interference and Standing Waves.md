### Boundary Conditions
A wave on a string reflects depending on the state of the end of the string:
- If it is a fixed end, inverted reflection occurs.
- If it is a free end, a non-inverted reflection occurs.


### Wave Interference and Superposition
When waves overlap, the resulting final displacement is the algebraic sum of each individual pulse.
#### Principle of Superposition
If we have two waves of position $y_1$ and $y_2$, then our final displacement is
$$
y(x,t) = y_1(x,t) + y_2(x,t)
$$

### Standing Waves on a String
Consider when a sinusoidal wave is reflected on a fixed end.

The resulting wave is called a **standing wave**. This is because the wave "appears" to be non-moving (aka "standing" in place). There are two parts of a standing wave:
- Nodes: points on a wave where the displacement is always 0
- Antinodes: points on a wave where displacement reaches its maximum

For a standing wave to manifest, the length of the string $L$ and the wavelength $\lambda$ should have the following relationship:
$$
L = \frac{n}{2}\lambda_n
$$
where $n$ is any integer, corresponding to the number of antinodes present in the standing wave.
#### Wave Function of a Standing Wave
Given two wave positions $y_1$ and $y_2$,
$$
\begin{align*}
	y_1(x,t) = -A\cos(kx+\omega t)
	y_2(x,t) = A\cos(kx+\omega t)
\end{align*}
$$
then the final displacement position is
$$
\begin{align*}
y(x,t) &= y_1(x,t) + y_2(x,t) \\
&= A(-\cos(kx+\omega t)+A\cos(kx+\omega t)) \\
&= (2A\sin kx)(\sin(\omega t)) \tag{using trig addition} \\
&= (A_{\text{sw}}\sin kx)(\sin(\omega t)) \tag{alternatively} \\
\end{align*}
$$
To then find the position of the nodes, we can take advantage of the fact that $y(x,t) = 0$ at these points. Because $A_\text{sw} > 0$, then $\sin(kx) = 0$. From these we can get the following values:
$$
\begin{align*}
kx = 0, \pi, 2\pi, 3\pi, ... \\
x = 0, \frac{\pi}{k},\frac{2\pi}{k}, \frac{3\pi}{k}, ...
\end{align*}
$$

### Normal Modes of a String
Since we have the relationship
$$
L = n\frac{\lambda}{2}
$$
then we can have a possible standing wave frequency related to its corresponding wavelength according to:
$$
f_n = \frac{v}{\lambda_n} = n\frac{v}{2L}
$$
where $f_1$ is the fundamental frequency.

Integer multiples of $f_1$ correspond to $2f, 3f, 4f,$ etc. These are known as harmonics or overtones.

