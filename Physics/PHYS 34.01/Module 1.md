### Some Concepts
1. All velocities are relative
2. Relative to what? -> a frame of reference
3. The Maxwell Equations can be used to derive the wave equation
$$
\frac{\partial^2y}{\partial x} = \frac{1}{v^2} \, \frac{\partial^2y}{\partial t^2}
$$
for 1-D waves, with 
$$
\frac{1}{v^2} = \varepsilon_0\mu_{0}
$$
such that
$$
v = \frac{1}{\sqrt{ \varepsilon_0\mu_{0}}} = 2.9979\times 10^8 \,\text{ms}^{-1}
$$
showing that the speed of light $c$ is constant.
### 1. Maxwell's Equations
$$
\begin{align}
\nabla^2\vec{E} &= \varepsilon_0\mu_0 \, \frac{\partial^2\vec{E}}{\partial t^2} \\
\nabla^2\vec{B} &= \varepsilon_0\mu_0 \, \frac{\partial^2\vec{B}}{\partial t^2}
\end{align}
$$
where the $\varepsilon_0\mu_0 \, \frac{\partial^2\vec{E}}{\partial t^2}$ and $\varepsilon_0\mu_0 \, \frac{\partial^2\vec{B}}{\partial t^2}$ are the wave equations.

Taking the idea that this is true in any frame of reference and that it results in the speed of light $c$, then light always moves at speed $c$ at any frame of reference.

### 2. Special Relativity
(Einstein, 1905)
This relies on two postulates:
1. The laws of physics are the same in all [[#A.1 Inertial Reference Frames|inertial reference frames]].
2. The speed of light in a vacuum ($c$) is the same in all inertial reference frames.
##### 2.1 Einstein's Thought Experiment
Give a train travelling at a speed close to the speed of light. There are two observers, one is inside the train and another is outside the train.
![[einstein_special_relativity_thought.png|500]]
Say that at time $t=0$, the two observers are directly in front of each other. At this point, lighting strikes two ends of the train.
- In Observer C's perspective: lightning strikes both ends simultaneously
- In Observer D's perspective: lightning strikes side B before side A

This is the **Relativity of Simultaneity**.

##### 2.1.1 Additional Example
Take two setups $D$ and $P$ of same height from the mirror $y$.

In $D$, the time for light to make the round trip:
$$
t_D = \frac{2y}{c}
$$
Meanwhile, for setup $P$, the distance $d$ between the two points can be expressed as
$$
d = 2\sqrt{(vt_p/2)^2 +y^2}
$$
such that
$$
t_P = \frac{2\sqrt{(vt_p/2)^2 +y^2}}{c}
$$
We can then find $t_P$ in terms of $t_D$:
$$
\begin{align}
c^2{t_P}^2 &= 4\left( \left( \frac{vt_p}{2} \right)^2+y^2 \right) \\
&= v^2{t_P}^2 + 4y^2 \\
(c^2-v^2){t_P}^2 &= 4\left( \frac{ct_D}{2} \right)^2 \\
{t_P}^2 &= \frac{c^2}{c^2-v^2}{t_D}^2 \\
t_P &= \frac{t_D}{\sqrt{ 1-v^2 /c^2 }}
\end{align}
$$
This is the equation for [[#|time dilation]].
### Appendix
##### A.1 Inertial Reference Frames
This refers to any frame of reference that follows Newton's 1st Law (bodies do not accelerate if and only if the net force is 0).

For example, given three observers A, B, and C, all holding a ball:
- A is stationary
- B is in a train moving at constant velocity
- C is in an accelerating train
When all three observers drop the ball:
- To A and B, the ball falls straight down.
- To C, the ball curves downwards away.
Then, A and B are inertial, and C is non-inertial.

Also note that any frame of reference moving at a constant velocity relative to another inertial frame of reference is also inertial.