### State Classification
##### Accessibility
For a Markov Chain with transition probability matrix $\mathbf{P}$, state $j$ is accessible from state $i$ denoted by $i \to j$ if $P_{ij}^{(m)} > 0$ for some $m \geq 0$.

Note:
- Accessibility is not symmetric (i.e. $i\to j$ does not imply $j \to i$).
- If $i \to j$ and $j \to k$, then $i \to k$.
##### Communication
If $i \to j$ and $j \to i$, then they are said to communicate, denoted by $i \leftrightarrow j$.

Communication is an equivalence relation:
- Reflexivity: $i \leftrightarrow i$ (because $p_{ii}^{(0)} = 1$)
- Symmetry: If $i \leftrightarrow j$, then $j \leftrightarrow i$.
- Transitivity: If $i \leftrightarrow j$ and $j \leftrightarrow k$, then  $i \leftrightarrow k$.

A set of states $\mathcal{C}$ are called a communication class if:
- For any $i, j \in C$, there is $i \leftrightarrow j$
- For any $i \in C$ and $j \not\in C$, then $i \not\leftrightarrow j$.
##### Reducible Chain
An MC is irreducible if they all communicate with one another (i.e. one class). Otherwise, it is reducible.
### State Probability
For any state $i$ define the probability that starting from state $i$, the first return to $i$ is at the $n$th transition:
$$
f_{ii}^{(n)} = P(X_1 \neq i, X_2 \neq i, \dots, X_{n-1} \neq i, X_n = i | X_0 i)
$$
Note: By definition, $f_{ii}^{(0)} := 0$.

Then the probability of returning to state $i$ at any point:
$$
f_{ii}=\sum_{n=0}^\infty f_{ii}^{(n)}
$$
If $f_{ii} = 1$, the state is recurrent. If $f_{ii} < 1$, it is transient.
##### Number of Revisits
For a state $i$, consider the expected number of visits to $i$, $E[N_i|X_0=i]$, to be:
- Recurrent: $E[N_i|X_0=i] = \infty$
- Transient: $E[N_i|X_0=i] = \frac{f_{ii}}{1-f_{ii}}$
##### Return Probability
For a state $i$, the return probability is the probability that starting from state $i$ and returns at $i$ at the $n$th transition:
$$
P_{ii}^{(n)} = P(X_n=i|X_0=i)
$$
##### Return and First Return Probability (Convolution)
These two can be combined:
$$
P_{ii}^{(n)} = \sum_{k=0}^{n} f_{ii}^{(k)}P_{ii}^{(n-k)}
$$
such that $i$ is recurrent if and only if
$$
\sum_{n=1}^\infty P_{ii}^{(n)} = \infty
$$