- A theorem that allows for evaluating limits of indeterminate forms
- Very powerful!
Given a limit that is in the indeterminate form, then it would be equal to the limit of the derivatives of their numerator and denominator components, that is to say:
$$
\begin{align}
\lim_{x\rightarrow c}\frac{f(x)}{g(x)} = \lim_{x\rightarrow c}\frac{f'(x)}{g'(x)} 
\end{align} 
$$
#### Indeterminate Forms:
They can take various forms, such as the following:
- $\frac{0}{0}$
- $\frac{\pm\infty}{\pm\infty}$
- $\infty-\infty$ (and consequently, $-\infty+\infty$)
- $0 \cdot \pm \infty$
- $0^0$ (e.g. $\lim_{x\rightarrow0^+}x^x$)
- $1^{\pm\infty}$
- $\pm\infty^0$

#### Common situations:
##### If $\infty \cdot 0$ or $0 \cdot \infty$, (i.e. usually something involving $\ln(x)$):
Just place one of the terms into the denominator, usually you want to leave the $ln$ function at the numerator.

**Example:**
$$
\begin{align}
\lim_{x\rightarrow -\infty} x\ln(1-\frac{1}{x})
&= \lim_{x\rightarrow c} \frac{ln(1-\frac{1}{x})}{x^{-1}}
\tag{form: $-\infty\cdot0$ to $\frac{0}{0}$} \\


&= \lim_{x\rightarrow -\infty} \frac{\frac{1}{1-\frac{1}{x}}(\frac{1}{x^2})}{-x^{-2}} \tag{we find the derivatives} \\

&= \lim_{x\rightarrow -\infty} -\frac{1}{1-\frac{1}{x}} \tag{simplify} \\
&= -1

\end{align}
$$
##### If $1^\infty$, (i.e. usually something involving a value that cannot be separated into numerator and denominator):
Given
$$
\begin{align}
\lim_{x\rightarrow c}f(x)
\end{align} 
$$
we can say that $y = f(x)$ and then do $\ln y = \ln(f(x))$.

**Example:**
$$
\begin{align}
\lim_{x\rightarrow \infty} &\ln(1+\frac{1}{x})^x \tag{form: $1^\infty$} \\
y &= \ln(1+\frac{1}{x})^x
\end{align}
$$
then
$$
\begin{align}
\lim_{x\rightarrow \infty} \ln y = \lim_{x\rightarrow \infty} xln(1+\frac{1}{x}) \tag{form: $-\infty\cdot 0$}
\end{align}
$$
Using the same method as seen in [[#If $ infty cdot 0$ or $0 cdot infty$, (i.e. usually something involving $ ln(x)$)|the previous situation]]:
$$
\begin{align}
\lim_{x\rightarrow \infty} \ln y &= 1 \\
\end{align}
$$
Since $x$ is continuous in $\ln(f(x))$, we can do $\ln(\lim_{x\rightarrow \infty} y)$:
$$
\begin{align}
\lim_{x\rightarrow \infty} y &= e \\
\lim_{x\rightarrow \infty} (1+\frac{1}{x})^x &= e
\end{align}
$$
##### If $\infty - \infty$:
We can use the LCD to transform it into something in the form $\frac{0}{0}$.

**Example:**
$$
\begin{align}
\lim_{x\rightarrow 0^+} (\frac{1}{\tan^{-1}x} - \frac{1}{x})
&= \lim_{x\rightarrow 0^+} \frac{x-\tan^{-1}(x)}{xtan^{-1}(x)} \tag{form: $\frac{0}{0}$} \\

&= \lim_{x\rightarrow 0^+} \frac{1-\frac{1}{1+x^2}}{tan^{-1}(x)+x(\frac{1}{1+x^2})} \tag{find derivatives} \\

&= \lim_{x\rightarrow 0^+} \frac{x^2}{x+(1+x^2)tan^{-1}x} \tag{form: $\frac{0}{0}$} \\

&= \lim_{x\rightarrow 0^+} \frac{2x}{1+(1+x^2)(\frac{1}{x^2+1})+tan^{-1}(x)(2x)}
\tag{find derivatives} \\

&= \frac{0}{2} = 0
\end{align}
$$