$$
\begin{align}
\int_0^1 \int_0^1 \frac{1}{1-xy} \, dx dy
&= \int_0^1 \int_0^1 \sum_{n=0}^\infty y^nx^n \, dx dy \\
&= \int_0^1 \sum_{n=0}^\infty \frac{y^nx^{n+1}}{n+1} \Bigg|_0^1 \, dy \\
&= \int_0^1 \sum_{n=0}^\infty \frac{y^n}{n+1} \, dy \\
&=\sum_{n=0}^\infty \frac{y^{n+1}}{(n+1)^2} \Bigg|_0^1 \, dy \\
&=\sum_{n=0}^\infty \frac{1}{(n+1)^2} \\
&=\sum_{n=1}^\infty \frac{1}{n^2} \\
\end{align}

$$
