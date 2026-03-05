### Stationary Distributions
A distribution $(p_1,p_2,\dots)$ on state space $S$ of a Markov chain is a stationary distribution if it satisfies that if $P(X_n=i)=p_i$ (where $i=1,2,\dots$), then
$$
P(X_{n+1}=i)=p_i \tag{$i=1,2,\dots$}
$$
##### Limiting vs Stationary
![[module7-1.png]]
Notes:
- A limiting distribution is also a stationary distribution, wherein it is the only one stationary distribution.
- If the limiting distribution does not exist, then the stationary distribution may or may not be unique.
- For all intents and purposes for regular MCs, the two are the same.
### Local Balance Equations
If a distribution $\pi$ such that with a transition probability matrix $\mathbf{P}$:
$$
\pi_iP_{ij}=\pi_{j}P_{ji}
$$
then $\pi$ satisfies the local/detailed balance equations.