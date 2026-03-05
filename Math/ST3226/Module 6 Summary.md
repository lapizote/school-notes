### Periodicity
##### Period
For state $i$, let $d(i)$ be the greatest common divisor of $\{ n \geq 1, P_{ii}^{(n)} > 0 \}$ (the length of all possible paths that can arrive at $i$). If $\{ n \geq 1, P_{ii}^{(n)} > 0 \}$ is empty (starting from $i$, the chain will never revisit $i$), then $d(i) = 0$.

$d(i)$ is the period of state $i$.
##### Periodicity
With $d(i)$ as the period of state $i$, then:
- There exists an integer $N$ such that for any $n \geq N$ and $0 < k < d(i)$:
$$
P_{ii}^{(n*d(i))} > 0, P_{ii}^{(n*d(i)+k)} = 0
$$
- If there is $m > 0$ so that $P_{ji}^{(m)} > 0$, then for the same $N$, for any $n \geq N$:
$$
P_{ji}^{(m+nd(i))} > 0
$$
- If $i$ and $j$ can communicate, then
$$
d(i) = d(j)
$$
### Irreducible Markov Chains
Consider a single recurrent class $\mathcal{C}_k$, where we build an MC where
- state space: $\mathcal{C}_k$
- transition probability: $p_{ij,\mathcal{C}_k} = p_{ij}$
This is an irreducible MC< where it:
- has one communication class
- is recurrent/transient
- shares the same period $d$
##### Long-run Performance
##### Regular Markov Chains
An MC is regular if $k>0$ exists such that all elements in $\mathbf{P}^{(k)}$ are all strictly positive and non-zero.

i.e., it is irreducible, is aperiodic (period of all states is $1$), and is finite.

### Limit Theorems of Markov Chains
##### General Limit Theorem
For a recurrent irreducible MC, the mean duration between revisits is
$$
m_i = E[R_i|X_0=i] = \sum_{n=1}^\infty nf_{ii}^{(n)}
$$
and the long-run proportion is
$$
\lim_{ n \to \infty } \frac{1}{n} \sum_{k=1}^{n}P_{ij}^{(k)} = \frac{1}{m_j}
$$
##### Basic Limit Theorem
For a positive recurrent irreducible and aperiodic MC, such exists for any $i$ and $j$:
$$
\lim_{ n \to \infty } P_{ij}^{(n)} = \lim_{ n \to \infty } P_{jj}^{(n)} = \frac{1}{m_j} 
$$
where if $\pi$ is the solution for $\pi = \pi \mathbf{P}$, then
$$
\pi_j = \frac{1}{m_j}
$$
This MC is called **ergodic**.