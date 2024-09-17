**Note: Uses desmos-generated graphs.

Similar to regular cartesian coordinates, complex numbers may be represented in polar form.

For example, given $z=1+i$:
```desmos-graph
left=-3; right=3; top=3; bottom=-3;
degreeMode = degrees;
---
	r=0.5|blue|0<=\theta<=45
	(0.5*\cos(45),0.5*\sin(45))|blue|open|label:`45°`
	y=x|blue|dashed|0<=y<=1
	(1,1)|blue|label:`1+i`
```

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
We can use Euler's formula $e^{i\theta} = \cos\theta + i\sin\theta$ ([[6 - Proof for Euler's Formula|see proof here]]) to determine the exponential polar form, which would be
$$
z = re^{i\theta}.
$$
So the exponential polar form (which is commonly a preferred form of polar complex numbers) for $1+i$ would be
$$
z=\sqrt{2}e^{i(45\degree)}.
$$
#### Additional Info
This form makes it easier to do exponential equations. For example,
$$(\sqrt{2}e^{i45\degree})^6$$
is much easier to evaluate than
$$(1+i)^6.$$

You can also [[7 - Finding roots of complex numbers|find the roots of complex numbers]] using this form.