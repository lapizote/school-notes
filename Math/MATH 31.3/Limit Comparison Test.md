Consider
$$
\sum_{n=1}^{\infty} \frac{2n^3-1}{n^3}; \,\,\, a_n = \frac{2n^2-1}{n^3} > 0
$$
If we try to do the direct comparison test:
$$
\begin{align*}
2n^2 - 1 &< 2n^2 \\
\frac{2n^2-1}{n^3} & < \frac{2n^2}{n^3} = \frac{2}{n}
\end{align*}
$$
so
$$
\begin{align}
\sum_{n=1}^{\infty} \frac{2n^3-1}{n^3} < \sum_{n=1}^{\infty} \frac{2}{n} = 2\sum_{n=1}^{\infty} \frac{1}{n}
\end{align}
$$
The latter summations are divergent, so direct comparison test **does not work** here.

Going back:
$$
\begin{align}
\sum_{n=1}^{\infty} \frac{2n^3-1}{n^3}; \,\,\, a_n = \frac{2n^2-1}{n^3} \sim \frac{2n^2}{n^3} = \frac{2}{n}
\end{align}
$$
(Note that $\sim$ means "related to")
Then:
$$
\begin{align}
\lim_{n\rightarrow\infty} \frac{\frac{2n^2-1}{n^3}}{\frac{2}{n}} &= \lim_{n\rightarrow\infty} \frac{2n^2-1}{n^3} \cdot \frac{n}{2} \\
&= \lim_{n\rightarrow\infty} \frac{2n^3-1}{2n^3} \\
&= \lim_{n\rightarrow\infty} \frac{2-\frac{1}{n^2}}{2} \tag{multiply by $\frac{1/n^3}{1/n^3}$} \\
&= 1
\end{align}
$$
(alternatively, L'Hospital's rule also works here)

As $n\rightarrow\infty$, $\displaystyle \frac{2n^2-1}{n^3} = \frac{2}{n}$.

Since $\displaystyle \sum_{n=1}^{\infty}\frac{2}{n}$ is divergent, then $\displaystyle \sum_{n=1}^{\infty} \frac{2n^3-1}{n^3}$ is divergent.

This is called the **limit comparison test**.

### Summary of Limit Comparison Test
In summary, given
$$
\lim_{n\rightarrow\infty} \frac{a_n}{b_n} = c
$$
where $c$ is positive and finite:
1. If $\displaystyle \sum_{n=1}^{\infty} b_n$ converges, then $\displaystyle \sum_{n=1}^{\infty} a_n$ converges.
2. If $\displaystyle \sum_{n=1}^{\infty} b_n$ diverges, then $\displaystyle \sum_{n=1}^{\infty} a_n$ diverges.

### Example 1
$$
\sum_{n=1}^{\infty} \frac{\sqrt[3]{4n^7-3n^2+4}}{\sqrt{4n^9+n+2}};
$$
Then
$$
a_n = \frac{\sqrt[3]{4n^7-3n^2+4}}{\sqrt{4n^9+n+2}} \sim \frac{\sqrt[3]{n^7}}{\sqrt{n^9}} = \frac{1}{n^{13/6}}
$$
and $a_n > 0$

So
$$
\begin{align}
\lim_{n\rightarrow\infty} \frac{\frac{\sqrt[3]{4n^7-3n^2+4}}{\sqrt{4n^9+n+2}}}{\frac{\sqrt[3]{n^7}}{\sqrt{n^9}}} &= \lim_{n\rightarrow\infty} \frac{\frac{\sqrt[3]{4n^7-3n^2+4}}{n^7}}{\frac{\sqrt{4n^9+n+2}}{n^9}} \\
&= \lim_{n\rightarrow\infty} \frac{\sqrt[3]{4-3/n^5+4/n^7}}{\sqrt{4+1/n^8+2/n^9}} \\
&= \frac{\sqrt[3]{4}}{\sqrt{4}}
\end{align}
$$
This is a positive and finite. We can then use the LCT.
$$
\sum_{n=1}^{\infty} \frac{1}{n^{13/6}} \text{convergent}
\Longrightarrow_{\text{limit comparison test}} \sum_{n=1}^{\infty} \frac{\sqrt[3]{4n^7-3n^2+4}}{\sqrt{4n^9+n+2}} \text{convergent}
$$
($\frac{1}{n^{13/6}}$ is a p-series with $p = \frac{13}{6} > 1$)
### Example 2
$$
\sum_{n=1}^{\infty} \sin^4\frac{1}{n}; \,\,\,\, a_n=\sin^4\frac{1}{n} > 0
$$
Remember that $\sin x \approx x$ for very small $x$ since
$$
\lim_{x\rightarrow 0} \frac{\sin x}{x} = 1
$$
Then
$$
a_n = \sin^4\frac{1}{n} \sim \frac{1}{n^4}
$$
$$
\begin{align}
\lim_{n\rightarrow\infty} \frac{\sin^4\frac{1}{n}}{\frac{1}{n^4}} &= \lim_{n\rightarrow\infty} \left(\frac{\sin\frac{1}{n}}{\frac{1}{n}}\right)^4 \\
&= 1^4 \\
&= 1
\end{align}
$$
This is positive and finite. We can then use the LCT.
$$
\sum_{n=1}^{\infty} \frac{1}{n^4} \text{convergent}
\Longrightarrow_{\text{limit comparison test}}
\sum_{n=1}^{\infty} \sin^4\frac{1}{n} \text{convergent}
$$
