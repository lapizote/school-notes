### Sound Pressure
When sound passes through a medium (fluid), there is a change in volume as follows:
$$
\begin{align}
\frac{dv}{V} &= \lim_{\Delta x \rightarrow 0} \frac{S(y(x+\Delta x, t)-y(x,t))}{S\Delta x} \\
\frac{dv}{V} &= \frac{\delta y(x,t)}{\delta x}
\end{align}
$$
Note that the bulk modulus $B$ is represented in terms of pressure and change in volume:
$$
B = \frac{-p(x,t)}{\frac{dv}{V}}
$$
These two equations can then be combined and rearranged to get the pressure equation:
$$
p(x,t) = BkA\sin(kx-\omega t)
$$
where $B$ is the bulk modulus.

The maximum pressure can then be found through:
$$
\begin{align*}
p_\text{max} = BkA \tag{of a sinusoidal sound wave}
\end{align*}
$$

### Sound Velocity
We can express velocity in terms of the Bulk or Young's Modulus.
````col
```col-md
For liquids
$$
v = \sqrt{\frac{B}{\rho}}
$$
```
```col-md
For solids
$$
v = \sqrt{\frac{B}{\rho}}
$$
```
````

We can also find the velocity in gas in terms of the heat capacity ration $\gamma$:
$$
v = \sqrt{\frac{\gamma RT}{M}}
$$
where:
- $T$ = absolute temperature (K)
- $M$ = molar mass
- $R$ = gas constant, $8.314$ J/mole-K
- $\gamma$ = heat capacity ratio

### Sound Intensity
The intensity of a sound wave can be expressed as follows:
````col
```col-md
$$
I = \frac{1}{2}\sqrt{\rho B}\omega^2A^2
$$

```
```col-md
$$
I = \frac{p_\text{max}^2}{2\rho v} = \frac{p_\text{max}^2}{2\sqrt{\rho B}}
$$
```
````
Then to get the sound intensity level in decibels:
$$
\beta = (10dB)\log\frac{I}{I_0}
$$

### Standing Sound Wave
````col
```col-md
Open Pipe (Open both sides)
$$
f_n = n\frac{v}{2L} \,\, \text{(n = 1, 2, 3, ...)}

$$
```
```col-md
Stopped Pipe (Closed one side)
$$
f_n = n\frac{v}{4L} \,\, \text{(n = 1, 3, 5, ...)}
$$
```
````
Their fundamental frequencies would then be:
$$
\begin{align}
f_1 &= \frac{v}{2L} \tag{for an open pipe} \\
f_1 &= \frac{v}{4L} \tag{for a closed pipe}
\end{align}
$$
### Beat Frequency
The frequency of a "beat" is:
$$
f_\text{beat} = |f_2 - f_1|
$$

### Doppler Effect & Shock Wave
````col
```col-md
Doppler Effect
$$
f_L = \frac{v \pm v_L}{v \pm v_s}f_s
$$
where the sign of $v_L$ and $v_s$ depends on the direction of the movement of the listener and source. When moving towards the other, then the velocity is a positive. If moving away from the other, then the velocity is a negative.
```
```col-md
Shock Wave
$$
\sin\alpha = \frac{vt}{v_st} = \frac{v}{v_s}
$$
```
````