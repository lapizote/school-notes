### Methods on Solving:
#### 1. Separable Equations
**Condition:** Given a FOODE, we can separate and isolate the two variables so we get $f(x) dx = g(y) dy$.

**Steps:**
1. Separate the two variables into the LHS and RHS.
2. Integrate both sides.
3. ???
4. Profit!
#### 2. Homogeneous Equations
**Condition:** Given an inseparable FOODE in the form
$$
M(x,y)\,dx + N(x,y)\,dy = 0 
$$
where $M(x,y)$ and $N(x,y)$ are [[Homogeneous Function|homogeneous functions]] of the same degree.

**Steps:**
1. Use the substitution $y = vx$ or $v = \frac{y}{x}$.
2. Using the substitution in Step 1, find that $dy = v\,dx + x\,dv$ (through the product rule).
3. Substitute $dy$ and $y$ with the equations that we found in Steps 1 and 2.
4. If the condition is met, certain terms should add up (or cancel out) such that we get a separable equation.
#### 3. Linear Equation
**Condition:** Given a linear FOODE that we can write in the form
$$
\frac{dy}{dx} + P(x)y = Q(x)
$$
where $P(x)$ and $Q(x)$ are functions solely in terms of $x$.

**Steps:**
1. Find the integrating factor, $\mu(x) = e^{\int P(x)\,dx}$.
2. Multiply both sides by $\mu(x)$.
3. The LHS can then be written as an exact derivative $\frac{d}{dx}(\mu(x)y)$ (thanks to the product rule).
4. Integrate both sides.

#### 4. Exact Functions of 2 Variables
**Condition:** Given an exact FOODE in the form
$$
M(x,y)\,dx + N(x,y)\,dy = 0 
$$
there should exist a $f(x,y)$ such that when
$$
\begin{align}
\frac{\delta f}{\delta x} = M(x,y) \,;
\frac{\delta f}{\delta y} = N(x,y)
\end{align}
$$
then
$$
\frac{\delta M}{\delta y} = \frac{\delta N}{\delta x}
$$

**Steps (Method 1):**
1. Integrate $\frac{\delta f}{\delta x} = M(x,y)$ (with respect to $x$) and $\frac{\delta f}{\delta y} = N(x,y)$ (with respect to $y$) to get $f(x,y) = \int M(x,y) + C(x)$ and $f(x,y) = \int M(x,y)\,dx + C(x)$ and $f(x,y) = \int N(x,y)\,dy + D(y)$.
2. There should be common terms and uncommon terms. The uncommon terms should be the values of $C(x)$ and $D(y)$.
3.  Construct the final expression using these terms.
4. Since $M(x,y)\,dx + N(x,y)\,dy=0$ should be interpreted as $df=0$, then simply equate the final expression to $C$.

**Steps (Method 2):**
1. Integrate $\frac{\delta f}{\delta x} = M(x,y)$ (with respect to $x$) to get $f(x,y) = \int M(x,y)\,dx + C(x)$.
2. We can then differentiate both sides to get $\frac{\delta f}{\delta x} = M(x,y) + \frac{dC}{dy}$.
3. We can then equate the equation found in Step 2 with $\frac{\delta f}{\delta y} = N(x,y)$.
4. Find $C(y)$ and then construct the final equation found from Step 1.
5. Since $M(x,y)\,dx + N(x,y)\,dy=0$ should be interpreted as $df=0$, then simply equate the final expression to $C$.
