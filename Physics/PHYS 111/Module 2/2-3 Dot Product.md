Given two vectors $\vec{a}$ and $\vec{b}$, their dot product can be expressed as follows:
$$
\begin{align}
\vec{a} \cdot \vec{b} = a_xb_x + a_yb_y + a_zb_z 
\end{align}
$$
This also implies that the dot product is a scalar quantity.

**Example:**
Given $\vec{a}= -3\hat{i} + -\hat{j} + 2\hat{k}$ and $\vec{b} = 4\hat{i} - 3\hat{j} + 2\hat{k}$,
$$
\begin{align}
\vec{a} \, \cdot \, \vec{b} &= (-3)(4) + (-1)(-3) + (2)(2) \\
&= -12 + 3 + 4 \\
&= -5
\end{align}
$$
#### Properties
Notice that
$$\vec{a} \cdot \vec{a} = a_x^2 + a_y^2 + a_z^2
$$, which also means that
$$
\vec{a} \cdot \vec{a} = \left|\vec{a}\right|^2
$$
or
$$
\left|\vec{a}\right| = \sqrt{\vec{a} \cdot \vec{a}}
$$

### Physicist's Definition of Dot Product
Given two vectors $\vec{a}$ and $\vec{b}$,
$$
\vec{a} \cdot \vec{b} = \left|\vec{a}\right|\left|\vec{b}\right|\cos\theta
$$

#### Proof
Given the following vectors $\vec{a}$ and $\vec{b}$,

Since $\left| \vec{a} - \vec{b} \right| = (\vec{a} \cdot \vec{b}) \cdot (\vec{a} \cdot \vec{b})$ and using the cosine rule,
$$
\begin{align}
\left| \vec{a}-\vec{b} \right|^2 &= |\vec{a}|^2 + |\vec{b}|^2 - 2|\vec{a}|\vec{b}|\cos\theta \\

(\vec{a} \cdot \vec{b}) \cdot (\vec{a} \cdot \vec{b}) &= |\vec{a}|^2 + |\vec{b}|^2 - 2|\vec{a}|\vec{b}|\cos\theta \\

\vec{a} \cdot \vec{a} - \vec{a} \cdot \vec{b} - \vec{b} \cdot \vec{a} + \vec{b} \cdot \vec{b} &= |\vec{a}|^2 + |\vec{b}|^2 - 2|\vec{a}|\vec{b}|\cos\theta \\

-2\vec{a} \cdot \vec{b} &= -2|\vec{a}||\vec{b}|\cos\theta \\

\vec{a} \cdot \vec{b} &= |\vec{a}||\vec{b}|\cos\theta
\end{align}
$$

