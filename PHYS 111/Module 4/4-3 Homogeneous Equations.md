(to insert later)

A FOODE can be written as the sum
$$
M(x,y)dx + N(x,y)dy = 0
$$
Example:
$$
x^2 dy + (y^2-xy)dx = 0
$$
Normally, this equation is not separable.

However, if we use the substitution $y = vx$ (which also gives us $dy = v dx + x dv$):
$$
\begin{align}
x^2(vdx + xdv) + (v^2x^2 - x(vx))dx &= 0 \\
x^3dv + v^2x^2dx &= 0 \\
\end{align}
$$
We get something that's separable.
$$
\begin{align}
x^3dv &= -v^2x^2dx \\
\frac{1}{v^2}dv &= -\frac{1}{x}dx \\
-\frac{1}{v} &= -ln|x| + c \tag{After integrating both sides} \\
\frac{x}{y} &= ln|x|-c \tag{Note: +c can also be used} \\
e^{\frac{x}{y}} &= Ax \tag{where $A=e^{-c}$} \\
y &= \frac{x}{ln|x| + B} \tag{where $B=-C$}
\end{align}
$$