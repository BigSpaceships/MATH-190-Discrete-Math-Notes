# 2.3 - Functions

## 2.3.1 - Intro

1. Let $A$ and $B$ be sets. A funciton $f$ is a rule that assigns to each element $x\in A$ exactly one element $y\in B$, written $y=f(x)$
- A is called the domain of $f$ and $f$ is said to be defined on $A$
- B is called the codomain of $f$
- The range of f, denoted $ran(f)$, is $ran(f)=\{f(x)|x\in A\}$

Notes:
- We write as $f:A\to B$
- Mapping $\iff$ function
- One simple property of functions:
$\forall x,y\in A[x=y\to f(x)=f(y)]$

- A function $f:A\to B$ can be written
    $f=\{(x,f(x))|x\in A\}$
    which implies $f\subseteq A\times B$
    If  $(x,y)\in f$, then this means $f(x)=y$

- Arrow diagram

2. Determine the range of each function
a) let $f:\{1, 2, 3\}\to\{x,y,z\}$ be defined by $f=\{(1,x), (2,x), (3,y)\}$
    Range: $\{x, y\}$
b) let $sgn:\mathbb{R}\to\mathbb{R}$ be defined by
    $sgn=\{(x,y)|(x>0\to y=1)\ and\ (x=0\to y=0)\ and\ (x<0\to y=-1)\}$
    $ran(sig)=\{-1, 0, 1\}$
c) let $abs:\mathbb{R}\to\mathbb{R}$ be defined by $abs(x)=x*sgn(x)$
    $ran(abs)=\mathbb{R}^+\cup\{0\}=[0,\infty)$
d) let $floor,\ ceil:\mathbb{R}\to\mathbb{R}$ be defined by
    $floor=\{(x,n)|n\in\mathbb{Z}\ and\ (\exists c\in[0,1][x=n+c])\}$
    $ceil=\{(x,n)|n\in\mathbb{Z}\ and\ (\exists c\in[0,1][x=n-c])\}$

    $ran(floor)=\mathbb{Z}$
    $ran(ceil)=\mathbb{Z}$
e) let $X$ be a set with $S\subseteq X$. Define the function $f:\mathcal{P}(x)\to\mathcal{P}(X)\ by\ f(A)=A\cup S$
    $ran(f)=\{y\in\mathcal{P}(X)|y\supseteq S\}$

3. Let $f:A\to B$ with $S\subseteq A$. the image of $S$, denoted $f(S)$, is $F(S)=\{f(x)|x\in S\}$
$f(A)=ran(f)$
$F(\emptyset)=\emptyset$

4. Let $f:\mathbb{R}\to\mathbb{R}$ be defined by $f(x)=x^2$
a) $f([1,2])=[1,4]$
b) $f([-1,2])=[0,4]$
c) $\{x\in\mathbb{R}|f(x)\in[-1,2]\}=[-\sqrt{2},\sqrt{2}]$

5. For a function $f:A\to B$ with $T\subseteq B$, we define the preimage of $T$ through $f$, denoted $f^-1(T)$ as
$f^-1(T)=\{x\in A|f(x)\in T\}$

6. Let $f:A\to B$ with $S, T \subseteq A$, is $f(S)\cap f(T)=f(S\cap T)$? if yes, prove it. 
If no, can you say if one side is a subset of the other
False, but $f(S\cap T)\subseteq f(S)\cap f(T)$

Proposition: If $f:A\to B$ and $S,T\subseteq A$, then $f(S\cap T)\subseteq f(S)\cap f(T)$

> [Proof]: Suppose $f:A\to B$ and $S,T\subseteq A$
> Suppose $y\in f(S\cap T)$
> Then there exists $x\in S\cap T$ such that $y=f(x)$
> Since $x\in S\cap T$, then $x\in S$ and $x\in T$
> Since $x\in S$ and $x\in T$, then $f(x)\in f(S)$ and $f(x)\in f(T)$
> Then $f(x)\in f(S)\cap f(T)$
> Since $y=f(x)$, then $y\in f(S)\cap f(T)$.
> Thus $f(S\cap T)\subseteq f(s)\cap f(T)$

## 2.3.2 - One to One and Onto Functions

7. Let $f: A\to B$. We say that
    1) $f$ is one-to-one (or injective) if distinct elements in $A$ have distinct images in $B$
        - f is 1-1 $\iff \forall x_1,x_2\in A[f(x_1)=f(x_2)\to x_1=x_2]$
        - f is not 1-1 $\iff \exist x_1,x_2\in A[f(x_1)=f(x_2)\land x_1\neq x_2]$
    2) $f$ is onto (or subjective) if $B=f(A)$
        - f is onto $\iff \forall y\in B\exists x\in A[y=f(x)]$
        - f is not onto $\iff \exists y\in B\forall x\in A[y\neq f(x)]$
    3) $f$ is a bijection (or in one-to-one correspondence) if it is both one-to-one and onto

8. Determine if the following functions are one-to-one, onto, or both
a) let $p:\mathbb{Z}\to\mathbb{Z}$ be defined by
    1) $p(n)=n$ - Both
    2) $p(n)=n^2+4$ - Neither
    3) $p(n)=n^3-1$ - One-to-one (because defined on $\mathbb{Z}$)
b) let $f:\mathbb{N}\times\mathbb{N}\to\mathbb{Z}^+$ be defined by
    1) $f(m,n)=m+n+1$ - Onto
    2) $g(m,n)=2^m*3^n$ - One-to-one

