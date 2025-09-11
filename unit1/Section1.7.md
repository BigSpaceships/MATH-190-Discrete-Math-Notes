# Introduction to Proofs
1. Consider the following statements
a) If $n$ is even, then $7n-5$ is odd
True, Not provable because we don't know definitions
b) Between any two distinct real numbers there is a rational number
True, Not provable because we don't have enough information (definitions)
c) If $x$ and $y$ are any real numbers, then $|x+y|\leq|x|+|y|$

d) if $f(x)=x^2$, then 
$lim_{x\to a}f(x)=a^2$
Don't have a definition of a limit

### 1.7.5 - Direct Proofs

> Direct Proof of $P\to Q$
> 
> Suppose $P$
> .
> .
> .
> Therefore $Q$
> Thus, $P\to Q$. $\qed$

2. Given an integer $n$
- $n$ is even if there exists an integer $k$ such that $n=2k$
- $n$ is odd if there exists an integer $k$ such that $n=2k+1$
Two integers have the same parity if they are both even or both odd; 
They have oppositve parity if one is even and the other is odd

- n is even $\equiv\exists k\in\mathbb{Z}[n=2k]$
- n is odd $\equiv\exists k\in\mathbb{Z}[n=2k+1]$

Every integer is either even or odd

1. [Prove that if $n$ is even, then $7n-5$ is odd]
> Suppose n is even
> Then $n=2k$ for some integer $k$ (Now show $7n-5$ is odd)
> Since $7n-5=7(2k)-5$
> $=14k-5$
> $=2*7k-6+2$
> $=2(7k-3)+1$,
> and $7k-3$ is an integer, then (Integers are closed under addition, subtraction, and multiplication)
> $7n-5$ is odd
> Thus, $n$ even implies $7n-5$ is odd

> [!Note] Guidelines for proofs
> Use complete sentences
> Incorporate expressions and or equations into sentences
> Use equal signs and inequality symbols only in equations
> Do not put a mathematical symbol directly following punctuation
> Do not use logical symbols as abbreviations for words
> Colons are vary rarely needed
> Display long formulas, as well as short ones that are important, on their own lines
> Use consistent notation throughout a proof

3. [Suppose that $n$ is an integer. Prove that $n^2$ is even implies $n$ is even]
> Suppose $n^2$ is an even (Show n is even)
> Then there exists an integer $k$ such that $n^2=2k$
> Then $n=\sqrt(2k)$

We don't know how to show 2k is a perfect square 

4. Let $m$ and $n$ be positive real numbers. Prove each 
a) if $m\geq n$, then $m^0\geq n^0$ (Those are raised to the zeros)
$m^0\geq n^0$ is always true (This is a trivial proof)

b) if $mn < 0$, then $m < 0$ or $n < 0$
$mn < 0$ is false (This is a vacuous proof)

5. the conditional $P\to Q$ is trivial if $Q$ is always true and vacuous if $P$ is always false

### 1.7.6 - Proof by contraposition

> Proof by Contraposition of $P\to Q$
> 
> Suppose $\neg Q$
> .
> .
> .
> Therefore $\neg P$
> Thus, $P\to Q$. $\qed$

3. Second Try
> [Suppose that $n$ is an integer. Prove that $n^2$ is even implies $n$ is even]
> By contraposition ($n$ odd implies $n^2$ odd)
> Suppose $n$ is odd (show $n^2$ is odd)
> There exists an integer $k$ such that $n=2k+1$.
> Then, $n^2=(2k+1)$
> $=4k^2+4k+1$
> $=2(2k^2+2k)+1$
> Since $2k^2+2k$ is an integer, then $n^2$ is odd
> Therefore, $n^2$ even implies $n$ is even $\qed$

### 1.7.7 - Proof by Contradition

6.
- A real number $x$ is ration if it can be written in the form $x=m/n$, where $m$ and $n$ are integers (with $n\neq 0$)
- A real number $x$ that is not rational is called irrational 

7. 
Let $p$ be a positive real number. The square root of $p$ is a positive real number $x$ such that $x^2=p$


