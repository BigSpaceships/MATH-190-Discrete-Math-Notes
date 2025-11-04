# 5.3 – RECURSIVE D EFINITIONS AND S TRUCTURAL I NDUCTION

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
