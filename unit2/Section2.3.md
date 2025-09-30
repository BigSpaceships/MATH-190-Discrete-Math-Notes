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
    $floor=\{(x,n)|n\in\mathbb{Z}\ and\ (\exists c\in[0,1)[x=n+c]\}$
    $ceil=\{(x,n)|n\in\mathbb{Z}\ and\ (\exists c\in[0,1)[x=n-c]\}$

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

