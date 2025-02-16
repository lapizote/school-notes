### Laplace Transform
Given a function of $t$:
$$
F(s) = \mathcal{L}(f) = \int_{0}^{\infty}e^{-st}f(t)\,dt
$$
(Note: $e^{-st}$ is known as the "kernel".)

In addition, the inverse transform:
$$
f(t) = \mathcal{L^{-1}}(F)
$$
##### Theorem 1: Linearity
Laplace transforms are linear, i.e.:
$$
\mathcal{L}(af(t)+bg(t)) = a\mathcal{f(t)} + b \mathcal{L}(g(t))
$$
##### Theorem 2: s-shifting
If $f(t)$ has the transform $F(s)$ (where $s>k$), then $e^{at}f(t)$ has the transform $F(s-a)$ (where $s-a>k$), such that
$$
\mathcal{L}(e^{at}f(t)) = F(s-a)
$$
##### Theorem 3: Existence
If $f(t))$ is defined and piecewise continuous on every finite interval on the semi-axis $f \geq 0$ and satisfies the growth condition
$$
|f(t)| \leq Me^{kt}
$$
for all $t \geq 0$ and some constants $M$ and $k$, then $\mathcal{L}(f)$ exists for all $s>k$.

### Transforms of Derivatives and Integrals
##### Theorem 1: Laplace Transform of Derivatives
$$
\begin{align}
\mathcal{L}(f') &= s\mathcal{L}(f) - f(0) \\
\mathcal{L}(f'') &= s^2\mathcal{L}(f) - sf(0) - f'(0) \\
\mathcal{L}(f''') &= s^3\mathcal{L}(f) - s^2f(0) - sf'(0) - f''(0) \\
&\text{and so on...}
\end{align}
$$
These only hold if the lower order derivatives (e.g. $f$ and $f'$ for transform input $f''$) satisfy the growth condition and the transform input itself (in the same example $f''$) is piecewise continuous on every finite interval for $t \geq 0$.
##### Theorem 2: Laplace Transform of Derivatives (Generalized)
$$
\mathcal{L}(f^{(n)}) = s^n\mathcal{L}(f) - s^{n-1}f(0) - s^{n-2}f'(0) - \dots - f^{n-1}(0)
$$
##### Theorem 3: Laplace Transform of an Integral
Let $F(s)$ be the transform of function $f(t)$. Then, for $s>0$, $s>k$, and $t>0$:
$$
\begin{align}
\mathcal{L}\left( \int_0^t f(\tau) \,d\tau \right) = \frac{1}{s}F(s) && thus && \int_{0}^t f(\tau) = \mathcal{L}^{-1}\left( \frac{1}{s} F(s) \right)
\end{align}
$$
### Laplace Transform Method (DEs, IVPs)
Consider the IVP
$$
\begin{align}
y'' + ay' + by = r(t), && y(0) = K_0, && y'(0) = K_1
\end{align}
$$
where $a$ and $b$ are constant.

##### Step 1
Set up the subsidiary equation using [[#Theorem 1 Laplace Transform of Derivatives]]:
$$
[s^2Y - sy(0) - y'(0)] + a[sY - y(0)] + bY = R(s)
$$
After collecting all the $Y$-terms, we get
$$
(s^2+as+b)Y = (s+a)y(0) + y'(0) + R(s)
$$
##### Step 2
Solve the subsidiary equation by algebra using the transfer function
$$
Q(s) = \frac{1}{s^2+as+b} = \frac{1}{\left( s+\frac{1}{2}a)^2 + b - \frac{1}{4}a^2 \right)}
$$
to get
$$
Y(s) = [(s+a)y(0) + y'(0)]Q(s) + R(s)Q(s)
$$
If $y(0) = y'(0) = 0$, then $Y=RQ$ such that
$$
Q = \frac{Y}{R} = \frac{\mathcal{L}(\text{output})}{\mathcal{L}(\text{input})}
$$
##### Step 3
We invert $Y$ to obtain $y = \mathcal{L}^{-1}(Y)$. Usually, by using partial fractions to obtain a sum of terms where we can use the Tables.

### Laplace Table
[[Laplace Table.pdf|See here for Table(s) 6.8 and 6.9]]

### Unit Step & T-Shifting
##### Theorem 1: Time Shifting
If $f(t)$ has the transform $F(s)$, then the shifted function
$$
\tilde{f}(t) = f(t-a)u(t-a) =
\begin{cases}
	0 & \text{if } t<a \\
	f(t-a) & \text{if } t>a
\end{cases}
$$
has the transform $e^{-as}F(s)$, such that if $\mathcal{L}(f(t)) = F(s)$, then
$$
\mathcal{L}(f(t-a)u(t-a)) = e^{-as}F(s)
$$
or
$$
f(t-a)u(t-a) = \mathcal{L}^{-1}(e^{-as}F(s))
$$
### Dirac's Delta Function
To add
### Convolution & Integral Equations
Note that the transform of a product is different from the product of their transforms, i.e.
$$
\mathcal{L}(fg) \neq \mathcal{L}(f)\mathcal{L}(g)
$$
##### Theorem 1: Convolution Theorem
If two functions $f$ and $g$ satisfy the assumption in the [[#Theorem 3 Existence|Existence Theorem]] so that their functions $F$ and $G$ exist, then the product $H = FG$ is the transform of $h$ given by
$$
h(t) = (f\star g)(t) = \int_0^t f(\tau)g(t - \tau) \,d\tau
$$
