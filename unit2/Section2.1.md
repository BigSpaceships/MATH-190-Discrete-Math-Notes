# 2.1 - Set

## 2.1.1 - Intro
1. A set is an unordered collection of objects. These objects are called elements or members

2. $A=\{2,3,5,7\}=\{3,7,5,2\}=\{2,2,3,5,7,7,7\}$

$5\in A$

$ 4\notin A$

$ 2\in A\land 3\in A$ written as $2,3\in A$

3. Sets of numbers
a) Natrual numbers: $\mathbb{N}=\{0, 1, 2, 3, 4, ...\}$
b) Integers: $\mathbb{Z}=\{...,-2,-1,0,1,2,...\}$
c) Positive Integers: $\mathbb{Z}^+=\{1, 2, 3, 4, ...\}$
d) Rational numbers: $\mathbb{Q}=\{m/n\in\mathbb{Z}, n\neq0\}$
e) Real numbers: $\mathbb{R}$

others: $\mathbb{Q}^+$,$\mathbb{R}^-$, ...

Set Builder Notation: Characterize all elements in a set by stating the property or properties they must have to be members in the set.
{$x$ in a set | $x$ satisfies property $P$}

4. Reperesent the following sets using set buildernotation

$n,m,i,k$: integers
$x,y,z$: real numebrs
a) $\mathbb{N}$
$ \mathbb{N}=\{n\in\mathbb{Z}|n\geq 0\}$

b) $\{1,3,5,7,...\}$
$ \{n\in\mathbb{Z}^+|there\ exists\ k\in\mathbb{Z}\ such\ that\ n=2k+1\}$

c) $\{1,2,3,4,...,100\}$
$ \{n\in\mathbb{Z}^+|n\leq 100\}$

5. More sets of numbers
a) Complex numbers: $\mathbb{C}=\{x+iy|x,y\in\mathbb{R},i^2=-1\}$
b) Integers modulo n: for $n\in\mathbb{Z}^1,\mathbb{Z}_n=\{0,1,2,...,n-1\}$
c) Bounded intevals: let $a,b\in\mathbb{R}\ with\ a<b$
$[a,b]=\{x\in\mathbb{R}|a\leq x\leq b \}$
$[a,b)=\{x\in\mathbb{R}|a\leq x<b\}$ this doesn't work 
$(a,b)=\{x\in\mathbb{R}|a<x<b\}$
$(a,b]=\{x\in\mathbb{R}|a<x\leq b\}$

d) Unbounded intervals: let $a\in\mathbb{R}$
$[a,\infty)=\{x\in\mathbb{R}|x\geq a\}$
$(a,\infty)=\{x\in\mathbb{R}|x>a\}$
$(-\infty,b]=\{x\in\mathbb{R}|x\leq b\}$
$(-\infty,b)=\{x\in\mathbb{R}|x<b\}$

6. $A$ and $B$ are equal, written $A = B$, if they have exactly the same elements. In terms of quantifiers.
$A=B\equiv\forall x(x\in A \leftrightarrow x\in B)$

7. List all elements of $\{x\in\mathbb{R}|2^x+q=0\}$
There all no elements in the set

8. The unique set having no elements is the empyt set and is denoted $\emptyset$ or $\{ \}$

## 2.1.3 - Subsets 

9. Let $A$ and $B$ be sets. $A$ is a subset of $B$, written $A\subseteq B$, if $x=in A\ implies\ x\in B$
AKA $A\subseteq B\equiv\forall x(x\in A\to x\in B)$

> [Prove] Use a direct proof to prove $A\subseteq B$:
> Suppose $x\in A$
> ...
> Thus $x\in B$
> Therefore $A\subseteq B\qed$

10. Let $A$, $B$, and $C$ be sets. Prove if $A\subseteq B$ and $B\subseteq C$, then $A\subseteq C$
> [Proof]
> Suppose $A\subseteq B$ and $B\subseteq C$ \[now show $A\subseteq C$\]
> Suppose $x\in A$. \[Now show $x\in C$\]
> Since $x\in A$ and $A\subseteq B$, then $x\in B$.
> Since $x\in B$ and $B\subseteq C$, then $x\in C$.
> Hence, $A\subseteq B$ and $B\subseteq C$ implies $A\subseteq C$

11. Let $S$ be a set. Prove that (i) $\emptyset\subseteq S$ and (ii) $S\subseteq S$

> (i) [Proof] - Suppose $x\in\emptyset$, which is false
> The statement is vacously true
> Thus $\emptyset\subseteq S$

> (ii) [Proof] - Suppose $x\in S$ \[Prove $x\in S$\]
> We are done.
> Thus $S\subseteq S$

12. Let $A$ and $B$ be sets. We say $A$ is a proper subset of B, written $A\subset B$, if $A\subseteq B$ and $A\neq B$

## 2.1.4 - The size of the set

13. If there are exactly $n$ distint elements in a set $S$, then $S$ is called a ***finite set***
- The order (or cardinality) of a finite set $S$, denoted $|S|$, is $n$. 
- The set that is not finite called infinite

14. Determine each of the following.
a) $|\{-2,-1,0,1,2\}|$ = $5$
b) $|\emptyset|$ = $0$
c) $|\{\mathbb{R}\}|$ = $1$ - the set containing $\mathbb{R}$ NOT the set $\mathbb{R}$
d) $|\{\emptyset|\}|$ = $1$ = the set containing $\emptyset$ not the empty set
