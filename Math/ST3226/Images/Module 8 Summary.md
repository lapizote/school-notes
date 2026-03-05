### PageRank
A graph of webpages in a website can be thought of as a Markov chain, which each node being a state (the webpage that the user is on).

For every state:
- Webpages with more hyperlinks have a higher probability to stay
- As $n$ increases, the time on important webpage increases

In the long run:
- A limiting distribution forms, indicating importance ranking

The initial distribution would have $X_0$ set to be uniformly distributed on $S$.

##### General Case
Let state space $S$ be the series of webpages, the time index as $\{ 0,1,2,\dots \}$, and the transition probability matrix be
$$
\begin{align}
P_{ij} = \begin{cases}
\frac{1}{\text{Number of Hyperlinks on $i$}} \,\,\,\,\,\, i\to j \\
0, \,\,\,\,\,\, \text{otherwise}
\end{cases}
\end{align}
$$
such that it is a stationary Markov chain and
$$
\pi^{(0)} = \left( \frac{1}{|S|}, \frac{1}{|S|},\dots\frac{1}{|S|}  \right)
$$
If it is ergodic:
$$
\pi = \lim_{ n \to \infty } \pi^{(0)}\mathbf{P}^n
$$
and we order the webpages such that
$$
\pi_{(1)} \geq \pi_{(2)} \geq \dots \geq \pi_{|S|}
$$
If it is not a regular MC:
- It has multiple classes
- It may have absorbing states
As such, we update it with the consideration that $X_0 \sim \pi_0$ and we set the transition probability matrix as
$$
\tilde{\mathbf{P}} = \lambda \mathbf{P} + (1-\lambda)\pi_0 \mathbf{1}^T
$$
where:
- $\tilde{\mathbf{P}}$ has no negative entries, has row sum $1$, and is irreducible and aperiodic w/ finite states
- $\lambda$ is the damping factor
Then:
$$
\pi_{n+1} = \lambda \pi_n \mathbf{P} + (1-\lambda)\pi_0
$$
##### Variants
- Weighted PageRank
- Distributed Learning of PageRank
- Advertisements
- Personalized Ranking
##### Applications
- Citation anaylsis
- Protein-problem network analysis
- Neuroscience

Requirement: Given a webpage network, students should be able to write out the corresponding random walk parameters, find the limiting distribution, and sue the limiting distribution to rank. Students are also able to execute PageRank with damping factor $\lambda$ for several runs (using calculator), to then present the ranking.