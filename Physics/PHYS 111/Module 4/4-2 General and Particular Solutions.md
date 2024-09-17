### General Solution
Given a FOODE, we can solve for a general solution generally by separating the two variables into the LHS and RHS.

For example:
$$
\begin{align}
\frac{dy}{dx} &= xy \\
\frac{1}{y}dy &= xdx \\
\int\frac{1}{y}dy &= \int xdx \\
|y| &= e^{\frac{x^2}{2}+c} \\
&= e^{\frac{x^2}{2}}e^c \\
&= Ae^{\frac{x^2}{2}} \tag{with $A = e^c$ and $A>0$} \\
y &= \pm Ae^{\frac{x^2}{2}}
\end{align}
$$
And since we want a general solution:
$$
y=Ae^{\frac{x^2}{2}}
$$
### Particular Solution
Then, given initial values, we can then find a specific solution.

For example, if the latter equation had the initial values $y=2$ when $x=0$, then
$$
\begin{align}
2 &= Ae^{\frac{0^2}{2}} \\
A &= 2
\end{align}
$$
which then gives us the particular solution
$$
y=2e^{\frac{x^2}{2}}
$$

(In general, DE + IL = Initial value problem aka. IVP)