Sound is:
- A longitudinal wave in a medium (can propagate through liquid and solid).

Consider (for now) that sound is:
- in an idealized case of a sound wave
- propagating in the $+x$-direction *only*.

Then we have the wave function $y(x,t)$ as the displacement $y$ of a particle at position $x$ and time $t$. Essentially, we use the same function [[1 - Formula of a Wave|as previously]],
$$
y(x,t) = A\cos(kx - \omega t)
$$
but the displacement would then be parallel to propagation.

### Sound as pressure fluctuations
Let $p(x,t)$ be the instantaneous pressure fluctuation at point $x$ and time $t$. Note that:
- this is similar to gauge pressure
- to find the absolute pressure (given atmospheric pressure $pa$): $pa + p(x,t)$

Now consider an imaginary cylinder with a wave medium and cross-sectional area $S$.
![[Figure16.2.PNG]]

When a wave is present at time $t$, then the end of the cylinder at $x$ is displaced by $y_1 = y(x,t)$, while the end of the cylinder at $x+ \Delta x$ is displaced by $y_2 = (x + \Delta x, t)$.

When a wave is then present:
- If $y_2 > y_1$, then the cylinder volume increases (i.e. pressure decreases)
- If $y_2 < y_1$, then the cylinder volume decreases (i.e. pressure increases)
- Note that $V \propto \frac{1}{p}$.

The change in volume of the cylinder will then be
$$
\Delta V = S(y_2 - y_1) = S(y(x+\Delta x, t)-y(x,t))
$$
In the limit of $\Delta x \rightarrow 0$ of the fractional change $\frac{\Delta v}{V}$ of the cylinder:
$$
\begin{align*}
\frac{dv}{V} &= \lim_{\Delta x \rightarrow 0} \frac{S(y(x+\Delta x, t)-y(x,t))}{S\Delta x} \\
&= \frac{\delta y(x,t)}{\delta x}
\end{align*}
$$
Now recall that the fractional change in volume is related to the pressure fluctuation by bulk modulus $B$:
$$
B = \frac{-p(x,t)}{\frac{dv}{V}}
$$
where $\frac{dv}{V}$ is the equivalent to the compressibility of the medium. Then by using the previous equation $\frac{dv}{V} = \frac{\delta y(x,t)}{\delta x}$, then we can rearrange it to get:
$$
p(x,t) = BkA\sin(kx-\omega t)
$$
which then implies that the pressure amplitude is
$$
\begin{align*}
p_\text{max} = BkA \tag{of a sinusoidal sound wave}
\end{align*}
$$
So now we can view sound waves three different ways:
![[Figure16.3.PNG]]


### Example Problem:
In a sinusoidal wave of moderate loudness, the max pressure is $3.0 \times 10^{-2}\,Pa$ above and below $pa$. Find the corresponding max displacement if the frequency of the wave is $1000\,Hz$. In air at normal atmospheric pressure and density, $v_s = 344\,ms^{-1}$ and bulk modulus is $1.42 \times 10^5\,Pa$.

**Solution:**

