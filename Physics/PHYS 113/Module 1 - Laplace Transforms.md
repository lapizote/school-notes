Linear Ordinary Differential Equations can be solved through Laplace Transforms.

The simplified process is as follows:
1. Given ODE is transformed into an algebraic equation, called the subsidiary equation.
2. The subsidiary equation is solved by purely algebraic manipulations.
3. The solution is Step 2 is transformed back, resulting in the solution of the given problem.

Example:
$$
m\ddot{x} + kx = 0
$$
### Advantages of Using Laplace Transforms
I. Problems are solved more directly; Initial value problems are solved without first determining a general solution. Nonhomogenous ODEs are solved without first solving the corresponding homogeneous ODE.

II. More importantly, the use of the unit step function and Dirac's delta make the method particularly powerful for problems with inputs that have discontinuities or represent short impulses or complicated periodic functions.

### Definition
If $f(t)$ is a function defined for all $t \geq 0$ its Laplace transform is the integral of $f(t)$ times $e^-{st}$ from $t=0$ to $\infty$. It is a function of $s$, say $F(s)$, and is denoted by $mathcal$