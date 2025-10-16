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

Counter Examples:
a - 2): $p(n)=n^2+4$ is not 1-1 because $-1,1\in\mathbb{Z}$(the domain) and $p(-1)=p(1)=5$
b - 1): $f(m,n)=m+n+1$ is not 11 because $(0,1),(1,0)\in\mathbb{N}\times\mathbb{N}$
        and $f(0,1)=f(1,0)=2$

a - 2): $p(n)=n^2+4$ is not onto because $2\in\mathbb{Z}$(the codomain), but there is no $n\in\mathbb{Z}$(the domain) 
        such that $p(n)=2$
a - 3): $p(n)=n^3-1$ is not onto because $9\in\mathbb{Z}$(the codomain), but there is no $n\in\mathbb{Z}$(the domain)
        such that $p(n)=8$
b - 2): $g(m,n)=2^m*2^n$ is not onto because $5\in\mathbb{Z}^+$(the codomain), but there is no $(m,n)\in\mathbb{N}\times\mathbb{N}$
        such that $g(m,n)=5$

Proofs:

1-1:

a - 1): 
Proposition: the function $p:\mathbb{Z}\to\mathbb{Z}$ defined by $p(n)=n$ is one-to-one
> [Proof] Suppose $p(m)=p(n)$ for $m,n\in\mathbb{Z}$.
> Then $m=n$. Thus $p$ is 1-1 $\qed$

a - 3):
Proposition: the function $p:\mathbb{Z}\to\mathbb{Z}$ defined by $p(n)=n^3-1$ is one-to-one
> [Proof] Suppose $p(m)=p(n)$ for $m,n\in\mathbb{Z}$(domain)
> Then, $m^3-1=n^3-1$. We simplify as $m^3=n^3$.
> Taking the cube root gives $m=n$
> Thus, $p$ is 1-1 $\qed$

Onto:

a - 1):
Proposition: the function $p:\mathbb{Z}\to\mathbb{Z}$ defined by $p(n)=n$ is onto
> [Proof] Suppose $n\in\mathbb{Z}$(codomain)
> Since $p(n)=n$ and $n\in\mathbb{Z}$(domain), $p$ is onto. $\qed$


b - 1):
Proposition: the function $f:\mathbb{N}\times\mathbb{N}\to\mathbb{Z}^+$ defined by $f(m,n)=n+m+1$ is onto
> [Proof] Suppose $k\in\mathbb{Z}$
> Since $k-1\in\mathbb{N}$, $0\in\mathbb{N}$ and $f(k-1,0)=(k-1)+0+1=k$ 
> Thus, $f$ is onto

b - 2):
Proposition: the function $g:\mathbb{N}\times\mathbb{N}\to\mathbb{Z}^+$ defined by $g(m,n)=2^m*3^n$ is one-to-one
> [Proof]: [Show $g$ is 1-1]
> Suppose $g(m,n)=g(p,q)$ [now show $(m,n)=(p,q)$, that is $m=n$ and $p=q$]
> Then $2^m*3^n=2^p=3^q$
> Divide both sides by $2^p*3^n$ to get $2^n/2^p=3^q/3^m$ 
> Simplify to $2^(m-p)=3^(q-n)$
> Since all powers of $3$ are odd (or have reciprocals that are odd) and the 
>     only powers of 2 that are odd are when the expondnet is $0$
> So $2^(m-p)=3(q-n)=1$ and implies $m-p=0$ and $q-n=0$.
> Thus, $m=p$ and $q=n$ and $(m,n)=(p,q$, so $g$ is 1-1

9. Let $A$ be a set. the identity map of $A$, denoted $l_A$ is the function $l_A:A\to A$ defined by $l_A(x)=x$ for all $x\in A$

10. Given functions $f:A\to B$ and $g:B\to C$, the composition $g\circ f:A\to C$ is defiend as $(g\circ f)(x)=g(f(x))$

11. For $A=\{1,2,3\},B=\{x,y,z\},\ and\ C=\{\alpha,\beta,\gamma\}$ 
    let $f:A\to B$ be defined as $f=\{(1,x),(2,y),(3,x)\}$
    let $g:B\to C$ be defiend as $g=\{(x,\gamma),(y,\alpha),(z,\beta)\}$
    What are $g\circ f$ and $f\circ g$

$ g\circ f:A\to C$
$ g\circ f=\{(1,\gamma),(2,\alpha),(3,\gamma)\}$

$f\circ g=$NOT DEFINED


12. Let $A$ be a set, $f:A\to A$ a function, and $n\in N$. the n-th iterative power of $f$, denoted $f^n$, is a function $f^n:A\to A$
defined as $f^0=l_A$ and for $n\in\mathbb{Z}^+$

$ f^n=f\circ f\circ f\circ ...\circ f$

13. For $A=\{1,2,3,4\}$, defined $g:A\to A$ as $g=\{(1,2),(2,2),(3,1),(4,3)\}$
find a) $g^0$, b) $g^1$, c) $g^2$, d) $g^3$, e) $g^4$

a) $g^0=l_A=\{(1,1),(2,2),(3,3),(4,4)\}$
b) $g^1=g$
c) $g^2=\{(1, 2), (2, 2), (3, 2), (4, 1)\}$
d) $g^3=\{(1, 2), (2, 2), (3, 2), (4, 2)\}$
e) $g^4=\{(1, 2), (2, 2), (3, 2), (4, 2)\}$

14. Let $f: A\to B$ be a bijection. The inverse of $f$ is the unique function $g:B\to A$ such that $g\circ f=l_A$
and $f\circ g=l_A$ The inverse of $f$ is traditionally written as $f^-1$. A function that has an inverse is said to be invertible

15. Let $f:[0,\infty)\to\mathbb{R}$ be defined by $f(x)=x^{1/2}$, is $f$ invertible? If yes, what is the inverse functino
Not onto, so not invertible 

16. Let $f:A\to B$. Then $f$ is a bijection if and only if f is invertible 

## 2.3.4 - The graph of functions 

17. Let $f:A\to B$. The graph of $f$, denoted $graph(f)$, is the set $graph(f)=\{(x,y)\in A\times B|f(x)=y\}$

## 2.3.5 - Other important functions 

18. The factorial function has the domain $\mathbb{N}$ and codomain $\mathbb{Z}^+$, denoted $n!$, and defined $0! =q$ and for $n\in\mathbb{Z}^+$

$n! = 1*2*3*4*...n$

