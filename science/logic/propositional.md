@def title = "Propositional Logic"

# {{fill title}}
The Concren of the propositional logic is showing validness of deductive arguments
Arguments are the producing new knowledge from existing knowledges.

the representations of knowledge without ambiguations are called **Proposition**.\\
and the strings of symbols of propositional logic are called **Propositional Formula** ( formular in plural ).

\def{1. The Propositional Formula.}{The propositional formula is defined with followings recursively.\\
+   **Atomic formula**, that denotions of knowledges.
+   **Compound formula**, that connected with connectives and parenthesis.
 #### Definition 1-1. Connectives.\\
Connectives are only to in simply system ( this called functional complete set ). and this system can be various.\\
I use the system with negation and implication :\\
+   Negation represented in $\neg P$ or $\sim P$, and read as "not".\\
+   Implication, Necessatily represented in $P \implies Q$, and read as "implies" or "if P, then Q".}

The formulae interpereted as truth value that is always true or false.\\
Atomic formulae interpreted in true or false, what value assigned is due to mathematician.\\
Connectives determine value of compund formulae by following subformulae.\\

| $P$ | $Q$ | $\neg P$ | $P \implies Q$ |
|-----------|-----------|-----------|-----------|
| $F$ | $F$ | $T$ | $T$ |
| $F$ | $T$ | $T$ | $T$ |
| $T$ | $F$ | $F$ | $F$ |
| $T$ | $T$ | $F$ | $T$ |

#### Definition 2. If the formula $A$ is true in the truth-assignment $\bar{x}$, Called $A\ satisfied\ in\ \bar{x}$.
#### Definition. if the $\bar{x}$ stisfy the $A$w, call $\bar{x}$ models $A$, and denoted as $\bar{x} \models A$.
the sign $\models$ represent the satisfaction relation.\\
If exsists the satisfied truth-assignment of formula $A$, called $A$ is satisfiable. And if their doesn't exist, called $A$ is unsatisfiable or Contradiction.\\

\\conjunction read as and
disjunction read as or
biconditional read as iff or if and only if
contradiction $\bot$ read as bottom.

= is used for equivalence, comparative this two formula has same inperetation, use $\equiv$ and called **semantic equality**.
\\

### Definition 2. Equivalent.
Equivalent represents that the truth set is same in every truth-value assignment and it denoted with equality "$=$".
### Definition 2-1.  logicall valid formula, topology



명제논리는 결정가능(decidable)하다. 즉 임의의 명제 논리식이 타당한지 (혹은 두 명제 논리식 간에 논리적 도출 관계가 성립하는지) 여부는 기계적으로 판단할 수 있다.
We shall also look at the truth or falsity of the statements and the validity of arguments built up from them.
    문장 ϕ가 모든 해석 하에서 참일 경우 문장 ϕ는 타당하다.
    문장 ϕ와 문장집합 Γ에 대해, Γ의 모든 문장들을 참이게 하면서 ϕ를 거짓이게 하는 해석이 존재하지 않을 경우 ϕ는 Γ의 귀결이다.
    문장집합 Γ에 대해, Γ의 모든 문장들을 참이게 하는 해석이 하나라도 존재할 경우 Γ는 일관적이다.


[^1]: this
