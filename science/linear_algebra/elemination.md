@def title = "Elemination"

# {{fill title}}
Elmination solves the system of linear equation by _eliminating_ the unknowns and produces the necessary conditions of solution.\\
If the necessary conditions are contradiction, The system of linear equations is inconsistent. 
if not, the system of linear equations is consistent.

Think about how solve the system of linear equations given below that not difficulut.
$$ \begin{cases} 1x + 2y = 3 \\ 4x + 5y = 6. \end{cases} $$
You may get the solution follow process given below :\\
Subtract 4 times the first equation from the second equation.
$$ (4x + 5y) - 4(1x + 2y) = -6,\ given\ -3y = -6. $$
This _eliminates_ x from the second equation. and it leaves one equation for y. and Immediately we know y = 2.\\
Then x comes from the first equation 1x + 2y = 3 :\\
**Back-substitution** : $1x + 2(2) = 3\ given\ x = -1$.

This process looks like easy and natural, but When we apply this process and How it works strictly?\\
Elemination is the answer of this questions and others.

## [Matrix.](/linear_algebra/matrix/)
[For more informtaions about Matrix, goto Matrix page to click here or title of this chapter.](/linear_algebra/matrix/)\\
You may notice the unknowns are not important to solve system of linear equations.\\
Because of this, We represent the system of linear equations given above to arrange of numbers without unknowns.
$$ A = \begin{bmatrix}\ 1 & 2\ \\\ 4 & 5\ \end{bmatrix},\ X = \begin{bmatrix} x \\\ y \end{bmatrix},\ Y = \begin{bmatrix}\ 3\ \\\ 6\ \end{bmatrix}
\\\ \\AX = Y. $$
Or represent the coefficients together with the right side of equations.\\
Comparatively, the first one called **coefficient matrix** and the last one called **argumented matrix**.
$$ A = \begin{bmatrix}\ 1 & 2 & 3 \ \\\ 4 & 5 & 6\ \end{bmatrix} $$


## Equivalent.
For solving the system of linear equations by performing operations, The operations must keep solution set.\\
When the two different system of linear equations have same solution set, The binary relation between two system is **Equivalent**.\\
Then we know the necessary conditions of operations that performed to solve are :\\
About the operation $e$ and m x n matrix A and B that $e(A) = B$, the solution set of $AX = Y$ and $BX = Y$ is same.

### Definition 2. Elementary row operation.
+ Scaling :$\quad e(A)_{ij} = A_{ij},\ if\ i \neq r,\ e(A)_{rj} = cA_{rj}.$
+ Interchange :$\quad e(A)_{ij},\ if\ i \neq r\ and\ s,\ e(A)_{rj} = A_{sj}, e(A)_{sj} = A_{rj}.$
+ Replacement :$\quad e(A)_{ij} = A_{rj} + cA_{sj}.$
The Elementary row operation is foundation of Elimination and assure the validity of elimination.\\
**Theorem 2-1.** System of linear equations that performed elementary row operation has same solution set with before performed.[^1]\\
**Theorem 2-2.** $\ \forall e,\ \exists e',\ e'(\ e(A)\ ) = e(\ e'(A)\ ) = A. $\\
proof : we can get proper e' for each case like that :
+ $e(A)_ij = cA_ij, define e'(A)_ij = c^-1 A_ij.$
+ $e(A)_ij = A_ij + cA_rj, define e'(A)_ij = A_ij - cA_rj.$
+ $e(A)_ij = A_rj, e(A)_rj = A_ij, define e' = e.$

### Definition 3. Row equivalent.
About m x n matrix B and A can get B by operate finite elementary row operation to A, _Called $B\ is\ row-equivalent\ to\ A$._\\
모든 행렬은 자기자신과 행 동치이다.\\
A가 B, C와 행 동치라면 B와 C는 행 동치이다.\\
행 동치인 행렬 A, B에 대하여, homogeneous system AX=0, BX=0은 동일한 해를 갖는다

that is, row-equivalent is equivalence relation.


## Elimination
lorem ipsum

### Definition 4. Row reduced
m x n matrix R is row-reduced if :
영행이 아닌 행의 첫번째 0이 아닌 원소를 선도원소leading entry라고 한다.
1. 선도 원소가 1이다.
2. 어떤 행의 선도 원소를 갖는 열의 다른 원소는 0이다.
   ->        기본 행 연산을 수행하여 얻고자하는 형태.

**Theorem 3.** $Every\ m \times n\ matrix\ is\ row\ equivalent\ to\ a\ row-reduced\ matrix.$\\
행 1의 선도 원소가 있는 열을 k라고 하자 ( A_ij != 0, 0 < k in j, not exists r in j, r < k )
행 1에 A_1k^-1을 row-multiplying하면 선도원소를 1로 얻을 수 있다. (a)를 만족한다.
행 i에 (i >= 2) (-A_ik) x A1를 더하면 k열의 다른 원소를 0으로 얻을 수 있다. (b)를 만족한다.

### Definition 5. Row-reduced echelon matrix
It is the Row-reduced m x n matrix satisfy follows.
$$ R = \begin{bmatrix}\ 0 & 1 & 0 & * & 0 & * & *\ \\\ 0 & 0 & 1 & * & 0 & * & *\ \\\ 0 & 0 & 0 & 0& 1 & * & *\ \\\ 0 & 0 & 0 & 0 & 0 & 0 & 0\ \\ \end{bmatrix} $$
영행은 영행이 아닌 행의 아래에 나타난다.\\
i번째 행의 선도원소의 열을 k_i라고 할때, k_1 < k_2 < ... < k_i.\\
즉, *가 임의의 수라고 할때, 4 x 6 기약 행 사다리꼴 행렬 R의 예 다음과 같다 :\\

**Theorem 4.** $Every\ m \times n\ matrix\ A\ is\ row\ equivalent\ to\ a\ row reduced\ echelon\ matrix.$\\
We know that A is row-equivalent ro a row-reduced matrix.\\
All that we need observe is that by performing a finite number of row interchanges on a row-reduced matrix.\\
we can bring it to row-reduced echelon form.

Row-reduced echelon matrix R, RX = 0 의 해 :\\
1, ..., r = non-zero rows of R, k_i = coloumn of leading entry of i row.\\

**Theorem 6**. $about\ m \times n\ matrix\ A\ that\ m < n,\ AX = 0\ has\ a\ non-trivial\ solution.$\\
Let $R$ be a row-reduced echelon matrix which is row-equivalent to $A$.
Then the system $AX = 0$ and $RX = 0$ have the same solution by [Theorem 3](#theorem_3_every_m_x_n_matrix_is_row-equivalent_to_a_row-reduced_matrix).\\
If $r$ is the number of non-zero rows in $R$, then certainly $r \leqslant m$, and since $r < n$.\\
It follows immediately from our remarks above that $AX=0$ has a non-trivial solution.

n x n identity matrix $I$. This is the n x n matrix defined by
$$ I_{ij} = \delta_{ij} = \begin{cases}\ 1,\quad if\ i = j \\\ 0,\quad if\ i \neq j.\end{cases} $$
This is the first of many occasions on which we shall use the Kronecker delta($\delta$).

**Theorem 7.** If A is an n x n matrix, then $A$ is row-equivalent to the n x n identity matrix\\
if and only if the linear system  $AX=0$ has only the trivial solution.

Proof : 

<!--
Elemination needs linearity.
+ superposition : f(x1 + x2) = f(x1) + f(x2).
+ homogeniety :     f(ax) = af(x).
-->
\\
[^1]: 추가 예정***END OF FILE***theorem 6. if A is an m x n matrix and m < a, then the homogenuous system AX = 0 has a non-trivial solution.
theorem 7. if A is an n x n matrix, then A is row-equivalent to the n x n indentity matrix if and only if the system AX = 0 has only the trivial solution.

homogenuous system always have trivial solution $x_1 = \cdots = x_n = 0$.

We form the Argumented matrix A' of the system AX = Y.
this is the m x (n+1) matrix whose first n column are the columns of A and whose last column is Y.
$$ A'_{ij}= A_{ij},\quad if\ j \le n\\ A'_{i(n+1)} = y_i. $$

Suppose we perform a sequence of elementary row operations on A, arriving at a row-reduced echelon matri R.
If we perfom this same equence of row opations on A',\\
we will arrive at a matrix R' whose first n column are the columns of R and whose last column contains certain scalars $z_1,\ \cdots,\ z_m$.
The scalar $z_i$ are the entries of the m x 1 matrix which result from applying the sequence of row operations to the matrix Y.

Gauss Elemination = Row reduction.
It is an algorithm solving a system of linear equations.
This method can also be used to find the rank of matrix, to calculate the determinant of a matrix, and to calculate the inverse of an invertible square matrix.
