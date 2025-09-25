# 2.2 - Set Opperations

## 2.2.1 - Introduction

1. Set opperations: Let $A$ and $B$ be sets with $U$ the universal set.
- Union: $A\cup B=\{x|x\in A\ or\ x\in B\}$
- Intersection: $A\cap B=\{x|x\in A\ and\ x\in B\}$
- Difference(or complement of $A$ with respect to $B$): $A-B=\{x|x\in A\ and\ x\notin B\}$
- Complement: $\overline{A}=U-A=\{x|x\notin A\}$

2. Two sets are disjoint if thier intesertion is empty $A\cap B=\emptyset$

3. Let $A=\{1, 2, 3\}$ and $B=\{3, 4, 5, 6\}$
a) $A\cup B=\{1, 2, 3, 4, 5, 6\}$
b) $A\cap B=\{3\}$
c) $A-B=\{1, 2\}$
d) $B-A=\{4, 5, 6\}$
e) $A\cap(A\cup B)=\{1, 2, 3\}=A$
f) $|A|+|B|-|A\cap B|=6=|A\cup B|$

4. Let $A=(1,3]$ and $(B=[3, 5)$ Determine the following.
a) $A\cup B=(1,5)$
b) $A\cap B=\{3\}$
c) $A-B=(1,3)$

5) Let $A=\{n\in\mathbb{Z}^+|n\ is\ even\}$ and $B=\{n\in\mathbb{Z}^+|n\ is\ prime\}$ with $U=\mathbb{Z}^+$ is the universal set
a) $\overline{A}=\{n\in\mathbb{Z}^+|n\ is\ odd\}=\mathbb{Z}^+-A$
b) $\overline{\overline{A}}=A$
c) $\overline{A\cap B}=\mathbb{Z}^+-\{2\}$
d) $\overline{A}\cup\overline{B}=\mathbb{Z}^+-\{2\}$

## 2.2.2 - Set Identities

Table in notes

7. Let $A$, $B$, and $C$ be esets. Prove if $A\subseteq B$, then $A\cap C\subseteq B\cap C$
> Suppose $A\subseteq B$ and $x\in A\cap C$ \[ now show $x\in B\cap C$
> Since $x\in A\cap C$, then $x\in A$ and $x\in C$.
> Since $x\in A$ and $A\subseteq B$, then $x\in B$.
> Since $x\in B$ and $x\in C$, then $x\in B\cap C$
> Thus $A\subseteq B$ implies $A\cap C\subseteq B\cap C$

## 2.2.3 - Generalized Unions and Intersections

8. Let $A_1, A_2, ..., A_n$ be a collection of sets 
- the union $A_1, A_2,...,A_n$, denoted $\bigcup^n_{i=1}A_i$, is the set that contains elements that are memebrs of at least one of the sets in the collection
- the intersection $A_1, A_2,...,A_n$, denoted $\bigcap^n_{i=1}A_i$, is the set that contains elements that are memebrs all of the sets in the collection

9. For each $i\in\mathbb{Z}^+$, define $A_i=\{0, 1, 2, ..., i\}$ Determine each of the following 
a) $\bigcup^{30}_{i=1}A_i=A_30$
b) $\bigcap^{30}_{i=1}A_i=\{1\}$

