## For Sequences
Given any sequence $a_n$, if there exists a $\displaystyle \lim_{n\rightarrow\infty} a_n = L$, then the sequence is convergent. If not, then the sequence is divergent.
### Monotonic Sequence Theorem
A sequence $\{a_n\}$ is increasing if $a_n < a_{n+1}$ for all $n \geq 1$. It is decreasing if $a_n > a_{n+1}$ for all $n \geq 1$.
In either case, it is monotonic. To find if it is monotonic, you can:
1. Compare $a_n$ and $a_{n+1}$ by checking $\displaystyle\frac{a_{n+1}}{a_n}$.
2. Check its first derivative.
3. (For recursive sequences) Find if $a_{n+1} - a_n$ is positive or negative. If positive, it is increasing. If negative, it is decreasing.

A sequence $\{a_n\}$ is **bounded above** if there is a number $M$ such that $a_n \leq M$ for all $n \geq 1$.
It is **bounded below** if there is a number $m$ such that $a_n \geq m$ for all $n \geq 1$.
It is **bounded** if it is both bounded above and bounded below.

If a sequence is both **bounded** and **monotonic**, then it is convergent.

---

## For Series
### Divergence Test
Given
$$
\sum_{n=1}^{\infty}a_n
$$
Then if $\displaystyle \lim_{n\rightarrow\infty} a_n \neq 0$, then $\displaystyle \sum_{n=1}^{\infty}a_n$ will diverge.
Note that this does NOT mean that $\displaystyle \sum_{n=1}^{\infty}a_n$ will converge if $\displaystyle \lim_{n\rightarrow\infty} a_n = 0$.
### Integral Test
Given
$$
\sum_{n=1}^{\infty}a_n
$$
Let $f(x)$ be a function satisfying:
1. $a_n = f(n)$
2. $f$ should be positive, continuous, and decreasing on $[1,\infty)$.
(If there is no $f(x)$ that satisfies both conditions, then we cannot use the integral test.)

Then:
1. If $\displaystyle \int_1^\infty f(x) dx$ is convergent, then $\displaystyle \sum_{n=1}^{\infty}a_n$ is convergent.
2. If $\displaystyle \int_1^\infty f(x) dx$ is divergent, then $\displaystyle \sum_{n=1}^{\infty}a_n$ is divergent.
### Direct Comparison Test
Given $\displaystyle \sum a_n$ and $\displaystyle \sum b_n$, with $a_n, b_n \geq 0$ for all $n$ and $a_n \leq b_n$ for all $n,
Then
1. If $\displaystyle \sum b_n$ is convergent, then $\displaystyle \sum a_n$ is convergent.
2. If $\displaystyle \sum a_n$ is divergent, then $\displaystyle \sum b_n$ is divergent.
### Limit Comparison Test
Given
$$
\lim_{n\rightarrow\infty} \frac{a_n}{b_n} = c
$$
where $c$ is positive and finite:
1. If $\displaystyle \sum_{n=1}^{\infty} b_n$ converges, then $\displaystyle \sum_{n=1}^{\infty} a_n$ converges.
2. If $\displaystyle \sum_{n=1}^{\infty} b_n$ diverges, then $\displaystyle \sum_{n=1}^{\infty} a_n$ diverges.
### Alternating Series Test
Given
$$
\sum_{n=1}^{\infty} (-1)^{n-1}a_n
$$
If $\displaystyle\lim_{n\rightarrow\infty} a_n = 0$ and $\{b_n\}$ is decreasing, then the sequence is convergent.

Note that this can ONLY conclude convergence.

#### An Extension of the Test
There are two types of convergent series:
1. Absolutely Convergent Series: convergent regardless if absolute values are taken
2. Conditionally Convergent: series becomes divergent if absolute values are taken.
Then, if $\displaystyle\sum_{n=1}^\infty |a_n|$ is convergent, then $\displaystyle\sum_{n=1}^\infty a_n$ is convergent. This is helpful when it is easier to find the former than the latter.

### Common Series & Sequences (for Comparison Tests)
#### P-series
The series in the form
$$
\sum_{n=1}^\infty \frac{1}{n^p}
$$
where $p$ is any real value.
For this series:
1. It is convergent for $p > 1$.
2. It is divergent for $p \leq 1$. ($p=1$ is known as the harmonic series).

#### Geometric Sequence & Series
The geometric sequence is in the form
$$
a_n = ar^{n-1}
$$
where $r$ is any value.
When turned into the series
$$
\sum_{n=1}^\infty ar^{n-1}
$$
It is:
1. Convergent when $r<1$ (where its sum becomes $\displaystyle \frac{a}{1-r}$)
2. Divergent when $r \geq 1$
