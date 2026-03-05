### Stopping Time
Let $\{ X_n \}_{n \geq 0}$ be a Markov chain on $(\Omega, \mathcal{F}, P)$.  A random variable $T : \omega \rightarrow \{ 0,1,2,\dots,\infty \}$ is called the stopping time, if for every $n\geq0$, the event $\{T=n\}$ depends solely on $X_1,X_2,\dots,X_n$.

At time $n$, one can decide to stop based on info available up to time $n$ (without knowledge of the future). When $T$ happens, we don't care about what happens afterwards.

##### Absorbing States
If state $i$ satisfies that $p_{ij} = 0$ for all $j \neq i$, then it is an absorbing state.
### First Step Analysis
- Step 1: Conditional on first step, set up an equation through the [[Module 1 Summary#Law of Total Probability|Law of Total Probability]]
- Step 2: Set up series of variables $u_i$ for $i \in S$ to express the unknown terms.
- Step 3: For each initial state $i$, set up the equation about $u_i$ based on first step analysis.
- Step 4: Solve the linear system.
##### Example
Gambler's ruin problem: we quit if $X=0$ or $X=4$.
![[module4-1.png|300]]
The states $0$ and $4$ absorbs the random walker.

We begin with starting state $X=2$.
$$
P(X_T=0|X_0=2) = \sum_{k=1}^\infty P(X_T=0|X_0=2,T=k)P(T=k|X_0=2)
$$
Through [[Module 2 Summary#Chapman-Kolmogorov Equations|Chapman-Kolmogorov]]:
$$
\begin{align}
P(X_T=0|X_0=2) &= \sum_{i\in S}P(X_T=0, X_1=i|X_0=2) \\
&= \sum_{i\in S}P(X_T=0| X_1=i)P(X_1=i|X_0=2) \\
&= p_{21}P(X_T=0| X_1=1) + p_{23}P(X_T=0|X_1=3) \\
\end{align}
$$
We set up $Y_n=X_{n+1}$ for $n=0,1,\dots$ such that 
$$YTP(X_T+0|X_1=1) = P(Y_{T-1}=-|Y_0=1)
$$
Since $\{ Y_n \}$ has the same probabilistic structure as $\{ X_n \}$:
$$
P(X_T=0| X_1=1) = P(Y_{T-1}|Y_0=1) = P(X_T=0|X_0=1)
$$
Then:
$$
\begin{align}
P(X_T=0|X_0=2) = p_{21}P(X_T=0| X_0=1) + p_{23}P(X_T=0|X_0=3)
\end{align}
$$
With $u_i = P(X_T=0 | X_0=i)$ and inserting the :
$$
\begin{align}
P(X_T=0|X_0=2) &= \frac{2}{3}u_1 + \frac{1}{3}u_3 \\
\end{align}
$$
This is repeated for every $u_i$ until a linear equation system is formed. In this system:
- $u_0=1$
- $u_1=\frac{14}{15}$
- $u_2=\frac{12}{15}$
- $u_3=\frac{8}{15}$
- $u_4=1$

If we then want to find $E[T|X_0 = 3]$, then
$$
\begin{align}
E[T|X_0=3] &= \sum_{t=0}^\infty tP(t=T|x_0=3)
\end{align}
$$

### General Case for Gambler's Ruin
Gambler stops with $N$ dollars or is broke. Winning probability is $p$, and $q=1-p$.
They start with $0<k<N$ in hand.
##### General Case: First Step Analysis
Starting with $u_k = P(X_T=0|X_0=k)$,
For a fair game ($p=q$):
$$
u_k=u_0-\frac{k}{N}
$$
For an unfair game ($p\neq q$):
$$
u_k=u_0-\left( \frac{1-(q / p)^k}{1-(q / p)^N} \right)
$$
##### General Case: Expectation
Starting with $v_k=E[T|X_0=k]$,
For a fair game ($p=q$):
$$
v_k=k(N-k)
$$
For an unfair game ($p \neq q$):
$$
v_k=\frac{1}{p-q}\left[ \frac{N(1-(q / p)^k)}{1-(q /p)^N} -k \right]
$$