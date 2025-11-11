# 5.3 – Recursive Definitions and Structural Induction

1. A recursively defined function (or equence), with domain $\mathbb{N}$ 
  is defined int he following manner.
  Bases: sepcify the first (or first few) values of the function/sequence
  Recursive step: state a rule that defines the function/sequence as an integer from the function/sequence defined at smaller integers.

2. For each definitino rewrite using a recursive definintion

|Definition|Basis|Recursive|
|-|-|-|
|2.3-12 iterative powers| $f^0=I_A$ | $f^n=f*f^{n-1}$|
|2.3.18 factorial funciton| $0!=1$|$n!=n*(n-1)!$|
|2.6-6 Matric power| $A^0=I$ | $A^n=AA^{n-1}$|
|2.6.18 Iterative boolean matrix power| $A^{[0]}=I$|$ A^{[n]}=A\cirdot A^{[n-1]}$|

3. The fibonacci numbers $f_n$ with domain $\mathbb{N}$ are defiend as 
basis: $f_0=0,f_1=1$
recursive step: $f_n=f_{n-1}+f_{n-2}$

4. Prove that $f_n=1/\sqrt{5}*((1+\sqrt{5})/2)^n-1/\sqrt{5}*((1-\sqrt{5})/2)^n$ for all $n\in\mathbb{N}$

For each $n\in\mathbb{N}$, let $P(n)$ be the propsition 
$f_n=1/\sqrt{5}*((1+\sqrt{5})/2)^n-1/\sqrt{5}*((1-\sqrt{5})/2)^n$

Proof: [Use strong induction]
> Basis: [check that P(0) and P(1) are true
> Since $f_0=0$, and $1/\sqrt{5}*((1+\sqrt{5})/2)^0-1/\sqrt{5}*((1-\sqrt{5})/2)^0$
> $=1/\sqrt{5}-1/\sqrt{5}=0$, then $P(0)$ is true
> Since $f_1=1$, and $1/\sqrt{5}*((1+\sqrt{5})/2)^1-1/\sqrt{5}*((1-\sqrt{5})/2)^1$
> $=1/\sqrt{5}((1+\sqrt{5})/2-(1+\sqrt{5})/2$
> $=1/\sqrt{5}(\sqrt{5}/2+\sqrt{5}/2)=\sqrt{5}/\sqrt{5}=1$, then $P(1)$ is true

> Inductive step: Let $k\in\mathbb{N}$ with $k\geq 2$. Suppose $P(0),P(1),...,P(k)$
>   are true. [IH] [now show $P(k+1)$ is true]
>   Then $f_{k+1}=f_k+f_{k-1}$ (substitute in here, it's lots of algebra I don't want to write out
> use HW 7-9 to get to $f_{n+1}$
> So $P(k+1)$ is true.
> Overall $P(n)$ for all $n\in\mathbb{N}$

## 5.3.3 - Recursively Defined Sets and Structures
5. Let $A$ be a set defined recursively by
Basis: $1\in A$
Recursive step: if $m,n\in A$< them $m+n\in A$

$ a\in A\land 2\in A\to 1+2=3\in A$
$a\in A\land 2\in A\to 1+2=3\in A$

$A=\mathbb{Z}$

6. A recursive definition of a set $A$ consists of two parts:
Basis: $S\subseteq A$ ($S$ is the basis)
Recursive Step: If $x$ is determined from elements $y_1, y_2, ..., y_k\in A$, then $x\in A$

7. Given the recursive definition of $A$, there is associated the
sequence of disjoint sets $A_0,\ A_1,\ A_2,\ A_3, ...$ defined by
1) $A_0 = S$, and
2) for $k \in \mathbb{ Z}^+$, let $A_k$ consist of all new elements constructed from elements in
$A_0 \cup A_1 \cup ...\cup A_{k–1}$ using the rules in the Recursive Step

8. Let $A\subseteq\mathbb{N}\times\mathbb{N}$ be defined recursively as
Basis: $(0, 0)\in A$;
Recursive Step: If $(m, n)\in A$, then $(m + 1, n), (m + 1, n + 1),(m + 1, n + 2)\in A$.
a) Determine A0 through A3.
  $A_0=\{(0,0\}$
  $A_1=\{(1,0),(1,1),(1,2))\}$
  $A_2=\{(2,0),(2,1),(2,2),(2,3),(2,4)\}$
  $A_3=\{(3,0),(3,1),(3,2),(3,3),(3,4),(3,5),(3,6)\}$

(b) Draw the points in the plane
idk look somewhere

## 5.3.4 - Structural Induction

9. Structural induction: Let $A$ be deinfed recursively as in 6. (With basis $A_0$) and let $P$
be a propositional function on $A$. If
  Basis: $\forall x\in A_0[P(x)]$
  Inductive Step: $[(y_1,y_2,...,k_k)\in A\to x\in A)\land P(y_1)\land P(y_2)\land ...\land P(y_k))]\to P(x)$
Then $P(x)$ is true for all $x\in A$

10. Let $A$ be the set given in example 8. Prove that all ordered paris $(m,n)\in A$ satisfy $2m\geq n$
> Proof
> Let $P(m,n)$ be the proposition $2m\geq n$. Use structural induction.
> Basis: Since $(0,0)\in A$ and $0\geq 0$, 
>   Then $P(0,0)$ is true.
> Inducive step: Suppose $(m,n)\in A$ and $P(m,n)$ is true [The IH]
> 1) [Since $(m+1,n)\in A$; show $P(m+1,n)$ is true.]
>   Since $2m\geq n$, then $2m+2\geq n$ 
>   Which implies $2(m+1)\geq n$. Hence $P(m+1,n)$ is true
> 2) [Since $(m+1,n+1)\in A$; show $P(m+1,n+1)$ is true.]
>   Since $2m\geq n$, then $2m+1\geq n$
>   Adding 1 to both sides gets $2m+2\geq n+1$
>   Which implies $2(m+1)\geq n+1$, Hence $P(m+1,n+1)$ is true
> 3) [Since $(m+1, n+2)\in A$; show $P(m+1,n+2)$ is true.]
>   Take $2m\geq n$. Adding 2 to both sides gives $2m+2\geq n+2$
>   Which implies $2(m+1)\geq n+2$. Hence $P(m+1,n+2)$ is true
> Thus $P(m,n)$ is true for all $(m,n)\in A$. $\qed$

11. Let $\Sigma$ be a set of symbols and define $\Sigma^*$ be the set of strings defiend recursively by
  Basis: $\lambda\in\Sigma^*$ and $\Sigma\subseteq\Sigma^*$ (where $\lambda$ is the empy string containing no symbols)
  Recursive step: if $x\in\Sigma^*$ and $y\in\Sigma^*$, then $xy\in\Sigma^*$

12. Let $\Sigma=\{J,M,U\}$ and let $A\subseteq\Sigma^*$ be defined recursively as 
  Basis: $MJ\in\A$
  Recursive Step: Let $x,y\in\Sigma^*$.
    1) if $xJ\in A$, then $xJU\in A$
    2) if $Mx\in A$, them $Mxx\in A$
    3) if $xJJJy\in A$, then $xUy\in A$

a) Determine $A_0$ through $A_3$
  $A_0=\{\lambda, MJ\}$
  $A_1=\{MJU,MJJ\}$
  $A_2=\{MJJU,MJUJU,MJJJJ\}$
  $A_3=\{MJJJJU,MJJUJJU,MJUJUJUJU,MJJJJJJJJ,MUJ\}$

b) no.
Define $l(x)$ to be the number of J's in x
Conjecture: Prove that for any $x\in A-\{\lambda\}$, $3!| l(x)$
Use structural induction to prove that this is true

Proof: Let $P(x)$ be the proposition $3 !| l(x)$
Basis: Since $l(MJ)=1$,, then $1 !| l(MJ)$ and so $P(MJ)$ is true
Inductive step: Suppose $xJ\in A$ and $P(xJ)$ is true
  Then $3 !| l(xJ)$ and so $3 !| l(xJU)$
  Then $P(xJU)$ is true

See mycourses for the rest of the steps

This concludes the inductive step .
Hence $P(x)$ is true for all $x\in A-\{\lambda\}$

