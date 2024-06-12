4. A robot is placed on a wide, flat table. It initially faces north. It has an internal variable called $\text{step\_size}$, which is initially set to 1.00 meter. It is then programmed to run the following commands in a loop forever:
	1. Move forward by $\text{step\_size}$.
	2. Divide $\text{step\_size}$ by 2.00.
	3. Turn left $45\degree$.

	After a very long time, what will the robot's displacement from its initial position?

**Final Solution:**
We can use the argand plane and assign the positive y-axis (Imaginary axis) as north.

The movement of the robot simply involves the addition of complex number components. By expressing the complex numbers through its exponential polar form, we can express the displacement after $n$ rotations as a complex number and with the series
$$
z_{\text{final}} = z_0+z_1+z_2\,+\,...+z_n 
$$
With $z_a$ referring to each step that the robot takes during $n$th rotation, we can then express the complex number after an infinite amount of turns through
$$
\begin{align}
z_\text{final} &= \sum^\infty_{n=0} \frac{r_0}{2^n}\left(\cos(\frac{\pi}{2}+\frac{\pi}{4}n) + i\sin(\frac{\pi}{2}+\frac{\pi}{4}n)\right) \\\\
&=\sum^\infty_{n=0} \frac{r_0e^{i(\frac{\pi}{2}+\frac{\pi}{4}n)}}{2^n}
\end{align}
$$
where $r_0$ is the initial value of $\text{step\_size}$.

Since $r_0$ is 1.00 meter, we can substitute as such:

$$
\begin{align}
z_\text{final} &= \sum^\infty_{n=0} \frac{e^{i(\frac{\pi}{2}+\frac{\pi}{4}n)}}{2^n}
\end{align}
$$

We can then make the summation easier for us to solve:

$$
\begin{align}
z_\text{final} &= \sum^\infty_{n=0} \frac{e^{i(\frac{\pi}{2}+\frac{\pi}{4}n)}}{2^n} \\
&= \sum^\infty_{n=0} \frac{e^{i\frac{\pi}{2}}+e^{i\frac{\pi}{4}n}}{2^n} \\
&= e^{i\frac{\pi}{2}} \sum^\infty_{n=0} \frac{e^{i\frac{\pi}{4}n}}{2^n} \\
&= e^{i\frac{\pi}{2}} \sum^\infty_{n=0} \left(\frac{e^{i\frac{\pi}{4}}}{2}\right)^n
\end{align}
$$

For our series to converge, then we must satisfy the condition $|r|<1$ where $r$ is the common ration. We can check for this by doing
$$
\begin{align}
|z| &= \left|\frac{e^{i(\frac{\pi}{4})}}{2}\right| <1 \\
&= \left| \frac{1}{2} e^{i(\frac{\pi}{4})} \right| <1 \\
&=\left|\frac{1}{2} \left(\cos\frac{\pi}{4} + i\sin\frac{\pi}{4}\right) \right| < 1 \\
&= \left| \frac{1}{2}\left(\frac{1}{\sqrt2}+i\frac{1}{\sqrt2}\right) \right| < 1 \\
&= \sqrt{\left(\frac{1}{2\sqrt2}\right)^2+\left(\frac{1}{2\sqrt2}\right)^2} < 1 \\
&= \frac{1}{2} < 1
\end{align}
$$
Since we satisfy the inequality, then the infinite sum converges. We can then find the sum through

$$S = \sum^\infty_{i=0} a_1r^i = \frac{a_1}{1-r}$$
where $a_1$ is the first term. If we let $a_1 = r_0 = 1$, then our final complex number becomes

$$
\begin{align}
z_\text{final}&= e^{i\frac{\pi}{2}} \sum^\infty_{n=0} \left(\frac{e^{i\frac{\pi}{4}}}{2}\right)^n \\
&= e^{i\frac{\pi}{2}} \left( \frac{1}{1- \frac{1}{2} e^{i(\frac{\pi}{4})} } \right) \\
&= \left( \cos\frac{\pi}{2} + i\sin\frac{\pi}{2} \right) \left(\frac{1}{1-\frac{1}{2} \left(\cos\frac{\pi}{4} + i\sin\frac{\pi}{4}\right) } \right) \\
&= \frac{ i }{ 1 - \frac{\sqrt2}{4} - \frac{\sqrt{2}}{4}i } \\
&= \frac{ i }{ \frac{4-\sqrt2}{4} - \frac{\sqrt{2}}{4}i } \\
&= \frac{ 4i }{ 4-\sqrt2 - \sqrt{2}i } \\
&= -\frac{4+5\sqrt2}{17} + \frac{16+3\sqrt{2}}{17}i
\end{align}
$$

Which means that our final displacement is
$$
\begin{align}
|z| &= \sqrt{ \left(-\frac{4+5\sqrt2}{17}\right)^2 + \left(\frac{16+3\sqrt{2}}{17}\right)^2 } \\
&= \frac{ \sqrt{340+136\sqrt{2}} }{ 17 }
\end{align}
$$

at the second quadrant, of angle $2.07$ rad from the positive x-axis.

The decimal value is around $1.357196689$.

```desmos-graph
left = -3; right = 3;
bottom = -3; top = 3;
degreeMode = radians
---
y=(\frac{16+3\sqrt{2}}{-4-5\sqrt{2}}x)|0<=y<=(16+3*2)/17
r=0.5|blue|0<=\theta<=2.07
```

#### Additional info
---
To check for our answer, I created a Python program that looks for the approximate value.

```python
import math

#find imaginary part
step = 1
imag = 0
for x in range(10000):
    imag += (1/2**x) * math.sin(((90+x*45)/180)*math.pi)
imag = step*imag

#find real part
real = 0
for x in range(10000):
    real += (1/2**x) * math.cos(((90+x*45)/180)*math.pi)
real = step*real

print(f"final complex number: {real} + {imag}i")
  
displacement = math.sqrt(real**2+imag**2)

print(f"displacement: {displacement}")
```

which gives the same answer ($1.3571966890916944$).
-Axl

#### Process w/ the Solution:
---
This was fairly tricky, especially since we had limited experience on working with infinite series.

It was easy to figure out that it was some sort of converging series considering that "a very long time" suggests a value reaching a limit and that the path taken would look like some weird spiral:

![[pset1pic1.png|400]]

The bulk of the time was us getting stuck on
$$
e^{i\frac{\pi}{2}} \sum^\infty_{n=0} \frac{e^{i\frac{\pi}{4}n}}{2^n}
$$
as we initially had no idea on how to evaluate it. We tried separating the series into the real and imaginary components
$$
\begin{align}
Re(z) = \sum^\infty_{n=0} \frac{r}{2^n}\left(\cos(\frac{\pi}{4}n)\right)\\\\

Im(z) = \sum^\infty_{n=0} i\frac{r}{2^n}\left(\sin(\frac{\pi}{4}n)\right)
\end{align}
$$
and played around with listing out the values:

| n   | r               | $\theta$                                        | $r\cos\theta$                       | $r\sin\theta$                       |
| --- | --------------- | ----------------------------------------------- | ----------------------------------- | ----------------------------------- |
| 0   | 1               | 0                                               | $1$                                 | $0$                                 |
| 1   | $\frac{1}{2}$   | $\frac{\pi}{4}$                                 | $\frac{\sqrt2}{4}$                  | $\frac{\sqrt{2}}{4}$                |
| 2   | $\frac{1}{4}$   | $\frac{\pi}{4} + \frac{\pi}{4}$                 | $0$                                 | $\frac{1}{4}$                       |
| 3   | $\frac{1}{8}$   | $\frac{\pi}{4} + \frac{\pi}{4} + \frac{\pi}{4}$ | $-\frac{\sqrt2}{16}$                | $\frac{\sqrt{2}}{16}$               |
| n   | $\frac{1}{2^n}$ | $n\frac{\pi}{4}$                                | $\frac{1}{2^n}\cos(\frac{\pi}{4}n)$ | $\frac{1}{2^n}\sin(\frac{\pi}{4}n)$ |
We even tried out multiplication operations:
$$(x+iy)(\frac{1}{\sqrt2} + \frac{1}{\sqrt{2}}i)$$
to no avail.

$$
\begin{align}
\sum^\infty_{n=0} \frac{r}{2^n} \left(1+0i\right) \left(\frac{1}{\sqrt2} + \frac{1}{\sqrt{2}}i\right)^n
\end{align}
$$
We were thinking that because we didn't really discuss it, maybe there was a solution other than using infinite series. We tried other methods like differentiation and even looked at definite integrals, but it seemed like the infinite series was our best bet.

One can imagine the dumbfounded look when one found out that you can simply take out the $n$ exponent and treat it like a geometric series.