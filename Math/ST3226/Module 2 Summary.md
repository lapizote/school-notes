### Stochastic Processes
A collection of random variables:
$$
\{ X(t,\omega) : t \in T \}
$$
where a sample path given an outcome $\omega$:
$$
X(\cdot,\omega) : T\rightarrow S
$$
where $T$ is the index set (usually time) and $S$ is the state space (all possible states).
##### Classification
- If $T$ is countable: discrete-time
- If $T$ is continuum: continuous-time
- If $S$ is countable: discrete-state
	- If $S$ is finite: finite-state
- If $S$ is continuum: real-state
- Example: Gambling game is a discrete-time, discrete-state stochastic process.
### Markov Chain
Let $\{ X_n: n \in T \}$ be a stochastic process with discrete-state space $S$ and discrete-time set $T$ satisfying the Markovian property, then $\{ X_n: n \in T \}$ is a **Markov chain** (MC).

##### Markovian property
Given $X_n$, what happens afterwards is independent with what happened in the past.

Such that for any set of states $i_0, i_1,\dots,i_{n-1},i,j \in S$ and $n \geq 0$:
$$
P(X_{n+1}=j|X_n=i,X_{n-1}=i_{n-1},\dots,X_0=i_0) = P(X_{n+1}=j|X_n=i)
$$
### One-step Transition Probability
Definition:
$$
p_{ij}^{n,n+1} = P(X_{n+1} = j|X_n=i)
$$
where $i,j \in S, n \in T$.
##### One-step Transition Probability Matrix
![[Pasted image 20251004163823.png|500]]

The sum of each row is exactly 1.

### Chapman-Kolmogorov Equations
With one-step transition probability matrix $\mathbf{P}$:
$$
\begin{align}
\mathbf{P}^{n,n+m+1} &= \mathbf{P}^{n,n+1}*\mathbf{P}^{n+1,n+m+1} \\
&= \mathbf{P}^{n,n+m}*\mathbf{P}^{n+m,n+m+1}
\end{align}
$$
### Stationary Transition Probability
A Markov chain has a stationary transition probability if
$$
p_{ij}^{n,n+1} = p_{ij}
$$
i.e. the one-step probability does not change when $n$ changes.
![[Pasted image 20251004164202.png|500]]

In addition, for any $m$-step transition probability matrices:
$$
\mathbf{P} = \mathbf{P}^m \tag{$m=0,1,2,\dots$}
$$
Requirements for identification of stationary MC: $S, T, P$