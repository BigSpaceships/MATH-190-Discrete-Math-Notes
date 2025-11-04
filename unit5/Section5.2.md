# 5.2 - Strong Induction and Weak Ordering

## 5.2.2 - Strong Induction

1 Let $P(n)^\infty_{n=0}$ be a sequence of propositions and let $m>0$
if basis step: P(0),P(1),...P(m) are all true and 
for any integer $k>m$ P(0),P(1),...P(k) are all true imply P(k+1) is true.

Then all popositions are true

The starting integer is arbitrary

The IH is the assumption $P(0)\land P(1)\land P(2)\land\cdots\land P(k)$ is true

In logical symnols
$\forall k[\forall j(j<k\to P(j))\to P(k+1)]\to\forall nP(n)$

## 5.2.3 - Examples of proofs using strong induction

2. Every positive integer greater than 1 can be written as the product of prime numbers.

Outline: 

> For $n\in\mathbb{Z}^+$ with $n>1$, let $P(n)$ be the proposition that n can be written 
>     as the product of primes
> Prove $P(n)$ is true for all $n\geq 2$
> Basis step: for $n=2$, this is a prime, so $P(2)$ is true
> Inductive step 
> Supose for some $k\in\mathbb{N}$ with $k\geq 2$, that $P(2),P(3),P(4),...,P(k)$ are all true [show $P(k+1)$ is true]
> That is, $k+1$ can be written as the product of prime numbers.
> If $k+1$ is prime, then $P(k+1)$ is true.
> If $k+1$ is composite, then there exists $a,b\in\mathbb{Z}^+$ such that $k+1=a*b$ where $a,b\geq 2$.
> $P(a)$ and $P(b)$ are true by the IH.
> Since $a$ and $b$ can be written as products of prime numbers, $k+1$ can be written as products of prime numbers, and $P(k+1)$ is true.
> Therefore the Inductive stem is true and $P(n)$ is true for any $n\in\mathbb{Z}^+$ and $n>1$

## 5.2.5 - Proofs using the well ordering principle

3. (the Well-Ordering Principle- WOP): Every nonempty set of nonnegative integers has a least elemtn

4. Mathematical induction is a valid proof technique.

Outline: By Contradiction

Suppose that $P(0)$ is true and $P(k)\to P(k+1)$ for any $n\in\mathbb{N}$ but at least one of them is false.

Let $S=\{n\in\mathbb{N}|P(n)\ is\ false\}\neq\emptyset$ because it contains at least one element.
Let $q$ be the least element in $S$ (by the WOP)
So $P(0),P(1),...,P(q-1)$ are all true. 
Thus $P(q)$ is true, which is a contradiction and $P(n)$ is true for any $n\in\mathbb{N}$

5. Prove that every nonnegative integer can be described using no more than fourteen english words.

Proof by condtradictino
Consider the set $A$ of nonnegative integers that can only be described in fifteen or more english words
This set $A$ is a subset of $\mathbb{N}$
By the well ordering principle (WOP) $A$ has a smallest element, say $m$.
This nonnegative integer is "The smallest nonnegatie integer that can be described using fifteen or more english words"
Which was done with fourteen words.
This is a contradiction that $M\in A$
Threfore, $A=\emptyset$ and every nonnegative integer can be described using no more than fourteen english words

(You have to define the set $A$ more preciesly; this proof is invalid) 

6. (division algorithm). Let $a,b\in\mathbb{Z}$ with $b\neq 0$. Then there are are unique integers $q,r\in\mathbb{Z}$ such that $a=qb+r$ and $0\leq r<|b|$
> Proof online

