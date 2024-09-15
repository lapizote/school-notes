#phys31-2 #waves #superposition
Consider two speakers that emit identical sinusoidal sound waves.
![[Figure16.21.PNG]]
At point $P$, the waves are in phase. Meanwhile, the waves are out of phase by $\frac{1}{2}$ at point $Q$.
This would mean that (given that each individual wave has amplitude $A$):
- At $P$, the total amplitude is $2A$ (constructive interference)
- At $Q$, the total amplitude is less than $A$ (destructive interference)

In general, constructive interference between two similar sinusoidal waves occurs when the path difference is in the form $n\lambda$ where $n$ should be an integer. Otherwise, destructive interference occurs.

See [[3 - Interference and Standing Waves#Wave Interference and Superposition]].

### Beats/Beat Frequency
When two different sound waves of same velocity but slight difference in frequency are played from the same origin, then one would notice a "wobble" as the resulting sound continuously changes from constructive interference to destructive interference and vice versa (sound gets softer, then gets louder). Hence, the name "beats".

The frequency of these "beats" is given by
$$
f_\text{beat} = |f_2 - f_1|
$$
Note that $f_1$ and $f_2$ can be interchanged.
#### Derivation
Suppose $f_a > f_b$, which means that $T_a < T_b$.

If the two waves start in phase at $t=0$, they once again go back to phase when the first wave goes through exactly one more cycle than the second wave (i.e. $t=T_\text{beat}$).

Let $n$ be the number of cycles of the first wave in $t = T_\text{beat}$. Then the number of cycles in the second wave at the same time is $n-1$. We then get:
$$
\begin{align*}
T_\text{beat} &= nT_a\\
T_\text{beat} &= (n-1)T_b
\end{align*}
$$
Through an elimination of $n$ and knowing that the period is just the reciprocal of the frequency:
$$
\begin{align}
T_\text{beat} &= \frac{T_aT_b}{T_b - T_a} \\
f_\text{beat} &= \frac{T_b - T_a}{T_aT_b} \\
&= \frac{1}{T_a} - \frac{1}{T_b} \\
\end{align}
$$
From this we can obtain:
$$
f_\text{beat} = f_a-f_b
$$

### Summary
The frequency of a "beat" is:
$$
f_\text{beat} = |f_2 - f_1|
$$