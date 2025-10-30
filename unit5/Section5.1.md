# 5.1 - Mathematical Induction

1. 
Show (i) $2|37^{5000}-37^{1000}$
Show (ii) $5|37^{5000}-37^{1000}$

$37^{5000}-37^{1000}$
$=(37^{1000})^5-37^{1000}$

Look!!!

|n|$n^5-n$|
|-|-|
|0|0-0=0|
|1|1-1=0|
|2|32-2=30|
|3|243-3=240|
|4|1024-4=1020|


## 5.1.2 - Mathmatical Induction

2. Theorem (The first principle of mathematical induction): 
Let: $(P(n))^\infty_{n=0}=(P(0),P(1),P(2)...)$ be a sequence of propositions
If: 
(base step) $P(0)$ is true and
(inductive step) for any $k\in\mathbb{N},P(k)$ implies $P(k+1)$ is true

Then $P(n)$ is true for all $n\in\mathbb{N}$

Notes: 
- Called weak induction because you only assume the previous case
- Say induction is being used
- In the inductive step, the premise of the implication is called the inductivce hypthoesis (DON'T SKIP) 
- $k$ is a dummy variable 
- The starting integer is arbitrary
- Be careful not to assume the conclusion
- Using logical expressions
  $P(0)\land[\forall k(P(k)\to P(k+1))]\to\forall nP(n)$

## 5.1.7 - Examples of proofs by mathematical induction

3. Prove that $0+1+2+3+\dots + n=1/2*n*(n+1)$

> [Proof]: By induction
> For each $n\in\mathbb{N}$, let $P(n)$ be the propositional function that
> $0+1+2+3+\dots + n=1/2*n*n_1)$
> Basis step: [Show $P(n)$ is true, plug in the left and right hand side]
> For $n=0$, the LHS of $P(0)$ is $0$, 
> the RHS of $P(0$ is $1/2*0*1=0$. Hence $P(0)$ is true
> Inductive step: Suppose $P(k)$ is true for some $k\in\mathbb{N}$ - The inductive hypothesis
> [That is $0+1+2+\dots+k=1/2*k*(k+1)$. Now show $P(k+1)$ is true. 
> That is, $0+1+2+\dots+k+1=1/2*(k+1)*(k+2)$]
> Then $0+1+2+\dots+(k+1)=(0+1+2+\dots+k)+(k+1)=1/2*k*(k+1)+(k+1)$
> $=(k+1)(1/2*k+1)$(factor out $k+1$)
> $=(k+1)(1/2k+2/2)=1/2(k+1)(k+2)$. Hence $P(k+1)$ is true
> Overall, for all $n\in\mathbb{N}$, $P(n).\qed$

4. Proof [by induction] $5|(n^5-n)$ for all $n\in\mathbb{N}$
> For each $n\in\mathbb{N}$ let $P(n)$ be the propositional function $5|n^5-n$
> Basis step: [Show P(0) is true]
> For $n=0$, $n^5-n=0$ and $5|0$. Hence, $P(0)$ is true
> Induction step: Suppose $P(k)$ is true for some $k\in\mathbb{N}$
> [That is, $5|k^5-k$; this is the IHs]
> Show $P(k+1)$, that is show $5|(k+1)^5-(k+1)$
> Then $(k+1)^5-(k+1)$
> $=k^5+5k^4+10k^3+10k^2+5k+1-k-1$
> $=k^5-k+5k^4+10k^3+10k^2+5k$
> $=(k^5-k)+5(k^4+2k^3+2k^2+k)$
> We know $5|k^5-k$ by the IH. Since $5|5$,
> Then, by theorem 4.1-3, $5|(k^5-k)+5(k^4+2k^3+2k^2+k)$.
> Equivilently, $5|(k+1)^5-(k+1)$. Hence $P(k+1)$ is true
> Overall, $P(n)$ for any $n\in\mathbb{N}.\qed$

5. Prove that $2^n<n!$ for all integers $n\geq 4$
> Proof by induction
> For each $n\in\mathbb{N}$ and $n\geq 4$, let $P(n)$ be the propositional function $2^n<n!$
> Basis step: [Show P(4) in true]
> For $n=4$, the LHS of $P(4)$ is $2^4=16$. 
> The RHS of $P(4)$ is $4! =24$ so $P(4)$ is true
> Inductive step: Suppose $P(k)$ is treu for some $k\geq 4$
> [That is, $2^k<k!$; this is the IH]
> Show $P(k+1)$, that is, show $2^{k+1}<(k+1)!$
> $2^{k+1}=2*2^k<2*k!$ [by the IH]
> $<(k+1)*k!$ This is true since $2<k+1$ for all $k\geq 4$
> $=(k+1)!$
> Hence $P(k+1)$ is true

