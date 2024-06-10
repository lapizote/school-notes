Similar to regular cartesian coordinates, complex numbers may be represented in polar form.

Given $z = x+iy$, we can then use the following properties:

$$
\begin{align}
\cos\theta = \frac{x}{r} \rightarrow x = r\cos\theta \\
\sin\theta = \frac{y}{r} \rightarrow y = r\sin\theta \\
\end{align}
$$
which then means that
$$
\begin{align}
z &= r\cos\theta + ir\sin\theta \\
&= r(\cos\theta+i\sin\theta)
\end{align}
$$
This is the polar form of a complex number.

So given a complex number $1+i$, its polar form would be:
$$
\begin{align}
r &= \sqrt{1^2+1^2} = \sqrt{2} \\
\theta &= \tan^{-1}(\frac{1}{1}) = 45\degree \\
1+i &= r(\cos\theta+i\sin\theta)\\
&= \sqrt{2}(\cos45\degree+\sin45\degree)
\end{align}
$$
We can use Euler's formula $e^{i\theta} = \cos\theta + i\sin\theta$ ([[1-6 Proof for Euler's Formula|see proof here]]) to determine the exponential polar form, which would be
$$
z = re^{i\theta}.
$$

#### Additional Info
This form makes it easier to do exponential equations. For example,
$$(\sqrt{2}e^{i45\degree})^6$$
is much easier to evaluate than
$$(1+i)^6.$$

You can also [[1-7 Finding roots of complex numbers|find the roots of complex numbers]] using this form.