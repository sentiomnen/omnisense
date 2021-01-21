@def title = "Linear Algebra"
#{{fill title}}
Linear algebra is the study of how solve the linear equations.\\
Among other things, The system of linear equations are the central problem of Linear algebra.

## Linear Equation.
Linear equation is the equations that has the first degreed unknowns.
$$ A_1 \cdot x_1 + A_2 \cdot x_2 + \cdots + A_n \cdots x_n = B \\\ \\ \sum_{i = 1}^n A_i \cdot x_i = B$$
$A_1, \cdots, A_n$ is positive integer exclude zero and it called **coefficient**. $B$ is positive integer include zero.\\
For get value of specific unknown $x_i$, transform equations to function about $x_i$.
$$ x_i = \{\ \sum_{j = 1}^{n-i} A_j  x_j + \sum_{j = i+1}^{n} A_j x_j+ B\ \}\ /\ A_i $$
\\ 


## System of Linear equations.
System of Linear equations is the set of linear equations.\
In Field F, **System of m linear equations in n unknowns** $S$ is defined :
$$About\ i \vee j \in R,\ 1 \le i \le m, 1 \le j \le n,\\\ \\
S = \begin{cases}\ A_{11} x_1 + A_{12} x_2 + \cdots + A_{1n} x_n\ \ \ = & b_1.\\
\ A_{21} x_1 + A_{22} x_2 + \cdots + A_{2n} x_n\ \ \ = & b_2.\\
\quad \vdots & \vdots \\
\ A_{m1} x_1 + A_{m2} x_2 + \cdots + A_{mn} x_n = & b_m.\ \end{cases} \\ or \\
\forall i, set\ S = \{\ \sum_{j=1}^n A_{ij} \cdot x_j = B_i \ \}$$

With follows $x_1 = s_1,\ x_2 = s_2, \cdots, x_n = s_n$, the tuple $(s_1, s_2, \cdots, s_n)$ called **solution**.\\
If $b_1 = b_2 = \cdots = b_m$, called this system to **homogeneous**. and this system has at least one solution that called **trivial solution**.\\

### [Elemination.](/linear_algebra/elemination/)
Solve the system of linear equations given below is not difficult.
$$ \begin{cases} 1x + 2y = 3 \\ 4x + 5y = 6. \end{cases} $$
You may solve to follow process given below :
$$ (4x + 5y) - 4(1x + 2y) = -6,\ given\ -3y = -6. $$
This _eliminates_ $x$ from the second equation. and it leaves one equation for y. and Immediately we know y = 2.\\
Then x comes from the first equation 1x + 2y = 3 :\\
**Back-substitution** : $1x + 2(2) = 3\ given\ x = -1$.

This process looks like easy and natural, but When we apply this process and How it works strictly?\\
[Elemination](/linear_algebra/elemination/) is the answer of this questions and others.
