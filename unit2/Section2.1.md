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
d) $|\{\emptyset\}|$ = $1$ - the set containing $\emptyset$ not the empty set
e) $|\{\emptyset, {\emptyset}\}|$ = $2$ - $\emptyset$ and the set containing $\emptyset$ - this didn't format right it shoudl be {0 ,{0}}

## 2.1.5 - Power sets

15. The set of all subsets of a set $S$ is called the power set of $S$ and is written $\mathcal{P}(S)$.

$X\in\mathcal{P}(A)\iff X\subseteq A$

16.
a) Determine the power set of each set
i) $S=\{x\}$
$S=\{\emptyset, {x}\}$

ii) $S=\{x, y\}$
$S={\emptyset, {x}, {y}, {x, y}\}$

iii) $S=\{x, y, z\}$
$S=\{\emptyset, {x}, {y}, {z}, {x, y}, {x, z}, {y, z}, {x, y, z}\}$

iv) $S=\mathbb{N}$
$s=\{\emptyset, {0}, {1}, ..., {0, 1}, {0, 2}, ..., {1, 2}, {1, 3}, ..., \mathbb{N}\}$

b) if $S$ is finite, determine $|\mathcal{P}(S)|$
if $|S|=n\in\mathbb{N}$, then 
$|\mathcal{P}(S)|=2^n=2^{|S|}$

17. Let $A$ and $B$ be sets. Prove if  $A\in B$, then $\mathcal{P}(A)\in\mathcal{P}(B)$
> [Proof]
> Suppose $X\in\mathcal{P}(A)$ \[show $X\in\mathcal{P}(B)$\]
> Then $X\subseteq A$
> Since $X\subseteq A$ and $A\subset B$, then $X\subseteq B$ (By ex. 10)
> Since $X\subseteq B$, then $X\in\mathcal{P}(B)$. Thus $A\subseteq B$ implies $\mathcal{P}(A)\subseteq\mathcal{P}(B)$

Alternatively the first two lines could be 
> Suppose $A\subseteq B$ and $X\in\mathcal{P}(A)$ \[Now show $X\in\mathcal{P}(B)$\]

## 2.1.6 - Cartesian Products

18.
- the ordered pair $(a,b)$ is the ordered collection that has $a$ as its first element and $b$ as its second element
- the ordered n-tuple $(a_1, a_2, ..., a_n)$ is the ordered collection of $n$ elements that has $a_1$ as its first element, 
$a_2$ as its second element, ..., and $a_n$ as its last ellement

19.
- The cartesian product of the sets $A$ and $B$, denoted $A \times B$, is $A\times B=\{(a,b)|a\in A\ and\ b\in B\}$
- The cartesian product of the sets $A_1, A_2,..., A_n$ denoted $A_1\times A_2\times ...\times A_n$ is
$A_1\times A_2\times ...\times A=\{(a_1, a_2, ..., a_n)|a_1\in A_i\ for\ i=1,2,...,n\}$

20. Determine the Cartesian product of $A=\{1,2,3\}$ and $B=\{y, z\}$
$A\times B=\{(1,y),(1,z),(2,y),(2,z),(3,y),(3,z)\}$

If $A$ and $B$ are finite sets, what is $|A\times B|$

$ |A\times B| = |A| |B|$

Notation: Use $A^2=A\times A$. So $\mathbb{R}^2=\{(x,y)|x,y\in\mathbb{R}\}$

