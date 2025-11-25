# 9.6 - Partial Orderings

## 9.6.1 - Introduction

equivalence rllations: $\equiv, \~ $
partial orderd sets 
$\leq, \preccurlyeq, \subseteq, |$

$ (\mathbb{R}, \leq)$ is the partial order on $\mathbb{R}$ for the normal less than relation

Let the relation $\mathcal{R}$ be defined on a set $S$, a poset (partial ordered set) is written as $(S,\preccurlyeq)$

1. A relation $\mathcal{R}$ on a set $A$ is a partial ordering if it is reflexive, anti-symmetric, and transitive

2. A partial ordering is complete if for every $x,y\in A$, we have either $x \preccurlyeq y$ or $y \preccurlyeq x$. Such an ordering is called a total

3. The following are partially ordered sets, are they total

a) $(\mathbb{R},\leq)$ yes, total because every element is less than another 
b) $(\mathbb{Z}^+,|)$ no, $5!| 7$ and $7!| 5$
c) $(\mathcal{P}(A),\subseteq)$, where $A$ is a set, $\{1\}$ and $\{3\}$ are not subsets of each ther

## 9.6.3 - Hasse Diagram

4. Given the partially ordered set $(A,|)$ where $A=\{1,3,5,6,9,10,12,15\}$

a) draw a digraph representation of $(A,|)$
    every element is connected to itself (it's reflexive)
    one is directed to everything
    three is directed to 6,9,12,15
    five divides 10, 15
    six divides 12

b) draw digraph representation of $(A,|)$ but with reflexive and transitive edges removed
    1 | 3 
    1 | 5
    3 | 6
    3 | 9
    3 | 15
    5 | 10
    5 | 15
    6 | 12

5. The Hasse diagram of a partially ordered set $(A,\precurlyeq)$ is the undirected graph representation 
    with reflexive and transitive edges removed so that arrows would all be directed upward

6. Draw the hasse diagram of $(A,|)$

   12
   |
9  6  15  10
 \ /.--'\ / 
  3      5
   '-. /
      1

