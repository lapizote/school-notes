### Processes
- Outcome space: $\Omega$ (Outcome $\omega \in \Omega$)
- Events: $\mathcal{F}$ (Element $\mathit{A} \in \mathcal{F}$)
- Probability Measure: $P$
	- Mapping: $\mathit{P} : \mathcal{F} \rightarrow [0,1]$
- Random Variable: $X(\omega) : \Omega \rightarrow (-\infty, \infty)$
- Definition: Collection of random variables such that $\{X(t,\omega) : t \in T\}$
### Indicator Function
Indicator function $I(A)$ of event $A \subset \Omega$:
$$
I[A](\omega) =
\begin{cases}
1, \omega \in A \\
0, \omega \not\in A
\end{cases}
$$
where:
- $I(A) : \Omega \rightarrow \{0,1\}$
### Discrete Random Variables:
- Bernoulli $Ber(p)$:
$$
P(X=x) = p^x(1-p)^{1-x} \tag{$x=0,1$}
$$
- Binomial $Bin(n,p)$:
$$
P(X=x) = \binom{n}{p}p^x(1-p)^{n-x} \tag{$x=0,1,2,\dots,n$}
$$
- Geometric $Geo(p)$:
$$
P(X=x) = p(1-p)^{x-1} \tag{$x=1,2,\dots$}
$$
- Poisson $Pois(\lambda)$:
$$
P(X=x) = e^{-\lambda} \frac{\lambda^x}{x!} \tag{$x=0,1,2,\dots$}
$$
### Expectation/Mean
Defined as
$$
E(X) = \sum_{x \in R_X} xP(X=x)
$$
Properties:
- If $X \geq 0$, $E[X] \geq 0$
- If $X \geq 0, E[X]=0$, then $P(X=0)=1$
- Shifting and multiplication: $E[a+bX]=a+bE[X]$
- Linear Additivity: $E\left[ \sum X \right] = \sum E[X]$
- Linear Transformation: $E[X]$ minimizes $E[(X-c)^2]$ where the former is the center

### Variance
Defined as
$$
Var(X) = E[(X-E(X))^2]
$$
or
$$
Var(X) = E[X^2]-(E[X])^2
$$
Properties:
- Standard deviation: $\sqrt{ Var(X) }$
- If $Var(X) = 0$, $P(X=E[X]) = 1$
- Linear Transformation: $Var(a+bX) = b^2Var(X)$
### Moment Generating Function
Defined as
$$
M_x(t) = E(e^{tX})
$$
(Note: Function of $t$, not $x$)

Used to generate k-th moment:
$$
E[X^k] = \frac{d^k}{dt^k}M_X(t)\biggr\rvert_{t=0}
$$
Properties:
- If two random variables have the same moment generating function, then they have the same distribution.
- Linear transformation: $M_{aX+b}(t) = e^{bt}M_X(at)$
![[module1-1.png|500]]
### Independence and Dependence
##### Independence
Discrete random variables $X_1, \dots, X_n$ are independent if for any $x_1, \dots, x_n$:
$$
P(X_1 = x_1, \dots, X_n = x_n) = \prod_{i=1}^{n} P(X_i=x_i)
$$
Properties include

### Conditional Random Variables
##### Bayes' Theorem
$$
P(X=x|Y=y)= \frac{P(Y=y|X=x)P(X=x)}{P(Y=y)}
$$
##### Multiplication Law
This is to find out joint probability.
$$
P(X=x,Y=y)=P(X=x|Y=y)P(Y=y) = P(Y=y|X=x)P(X=x)
$$
##### Law of Total Probability
This is to find out marginal probability
$$
P(X=x)=\sum_{y\in S} P(X=x|Y=y)P(Y=y)
$$
