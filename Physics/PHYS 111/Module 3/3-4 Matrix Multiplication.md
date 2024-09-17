Conditions for Matrix Multiplication, given matrices $A$ and $B$ and $A \times B$:
- Amount of columns of $A$ should be the same as the amount of columns of $B$

Algebraic expression for matrix multiplication, given $A \times B = C$ and $_{ij}$ being the row and column location of an element (respectively) in the resulting matrix:
$$
C_{ij} = \sum_{k=1}^n A_{ik} B_{kj}
$$
#### Examples:
$$
\begin{align}
A &=
	\begin{bmatrix}
		5 & -2 \\
		1 & 3
	\end{bmatrix}
\\
B &=
	\begin{bmatrix}
		3 & 1 \\
		-2 & 0
	\end{bmatrix}
\\\\
A \times B &=  
	\begin{bmatrix}
		19 & 5 \\
		-3 & 3
	\end{bmatrix}
\end{align}
$$