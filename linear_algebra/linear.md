@def title = "Linear Algebra"

# {{fill title}}
Solving the system of linear equations ( Sets of linear equations ) is the central problem of Linear algebra.\\

**In Field F, System of m linear equations in n unknowns are :**\\
$x_i$ that $1 \le i \le n$ is unknowns and $ A_{ij},\ b_i$ that $\ 1 \le i \le m, 1 \le j \le n, i \vee j \in R$ is constant.
$$ \begin{cases}\ A_{11} x_1 + A_{12} x_2 + \cdots + A_{1n} x_n\ \ \ = & b_1.\\
\ A_{21} x_1 + A_{22} x_2 + \cdots + A_{2n} x_n\ \ \ = & b_2.\\
\quad \vdots & \vdots \\
\ A_{m1} x_1 + A_{m2} x_2 + \cdots + A_{mn} x_n = & b_m.\ \end{cases} $$

With follows $x_1 = s_1,\ x_2 = s_2, \cdots, x_n = s_n$, the tuple $(s_1, s_2, \cdots, s_n)$ called **solution**.\\
If $b_1 = b_2 = \cdots = b_m$, called this system to **homogeneous**. and this system has at least one solution that called **trivial solution**.\\
Systems can sorted with solution set if :
+ the solution set is a empty set, the system sorted in _inconsistent_.
+ the solution set is not a empty set, the system sorted in _consistent_.

## [Elemination.](/linear_algebra/elemination/)
Think about how solve the system of linear equations given below that not difficulut.
$$ \begin{cases} 1x + 2y = 3 \\ 4x + 5y = 6. \end{cases} $$
You may get the solution follow process given below :\\
Subtract 4 times the first equation from the second equation.
$$ (4x + 5y) - 4(1x + 2y) = -6,\ given\ -3y = -6. $$
This _eliminates_ x from the second equation. and it leaves one equation for y. and Immediately we know y = 2.\\
Then x comes from the first equation 1x + 2y = 3 :\\
**Back-substitution** : $1x + 2(2) = 3\ given\ x = -1$.

This process looks like easy and natural, but When we apply this process and How it works strictly?\\
[Elemination](/linear_algebra/elemination/) is the answer of this questions and others.
