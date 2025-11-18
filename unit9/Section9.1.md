# 9.1 - Relations and Their Properties

1. Let $A$ and $B$ be sets. 
  - A relation from $A$ to $B$ is a subset of $A\times B$
  - A relation on $A$ is a subset of $A\times A$
Denote the relation as $\mathcal{R}$

2. Let $A=\{1,2,3\}$ and $B=\{y,z\}$ The following are relations from $A$ to $B$
a) $\mathcal{R}_1=\emptyset$
b) $\mathcal{R}_2=\{(1,y),(2,y),(2,z)\}$
c) $\mathcal{R}_3=\{(1,2),(2,y),(3,z)\}$
d) $\mathcal{R}_4=A\times B$

2^6 possible relations, that is $|\mathcal{P}(A\times B)|$

3. Properties of relations. Let $\mathcal{R}$ be a relation on $A$, then $\mathcal{R}$ is 
i) reflexive $\equiv\forall a\in A[(a,b)\in\mathcal{R}]$
ii) symmetric $\equiv\forall a,b\in A[(a,b)\in\mathcal{R}\to(b,a)\in\mathcal{R}]$
iii) anti-symmetric $\equiv\forall a,b\in A[(a,b),(b,a)\in\mathcal{R}\to(a=b)]$
iv) transitiive $\equiv\forall a,b\in A[(a,b),(b,c)\in\mathcal{R}\to(a,c)\in\mathcal{R}]$

4. Which of the properties does the relation $\mathcal{R}$ on $A=\{1,2,3,4\}$ defined by 
    $\mathcal{R}=\{(1,1),(2,2),(2,3),(3,2),(3,3),(3,4),(4,2)\}\subseteq A\times A$

i) reflexive?
    No. $(4,4)\notin\mathcal{R}$

ii) symmetric?
    No. $(3,4)\in\mathcal{R}$ but $(4,3)\notin\mathcal{R}$

iii) anti-symmetric?
    No. $(2,3)\in\mathcal{R}$ and $(3,2)\in\mathcal{R}$ but $2\neq 3$

iv) transitive?
    No. $(2,3)\in\mathcal{R}$ and $(3,4)\in\mathcal{R}$ but $(2,4)\notin\mathcal{R}$

5. Which of the properties does the relation $\mathcal{R}$ on $\mathbb{Z}$ define dy
    $\mathcal{R}=\{(m,n):m|n\}\subseteq\mathbb{Z}\times\mathbb{Z}$

i) reflexive?
    No. $0!|0$, $(0,0)\notin\mathcal{R}$

ii) symmetric?
    No. $2|4$ but $4!|2$ 

iii) anti-symmetric?
    No. $-2|2$ and $2|-2$ but $-2\neq 2$

iv) transitive? 
    Yes.

Using $\mathbb{Z}^+$ instead of $\mathbb{Z}$

Reflexive, symmetric, and transitive but not anti-symmetric

6. Let $n\in\mathbb{Z}^+$. Which of the properies does the relation $\mathcal{R}$ on $\mathbb{Z}$ defined by
    $\mathcal{R}=\{(a,b)|a\equiv(mod n)\}\subseteq Z\times Z$

i) reflexive? 
    Yes.

ii) symmetric?
    Yes.

iii) anti-symmetric?
    No. take $n=2$, then $(2,4),(4,2)\in\mathcal{R}$ but $2\neq 4$

iv) transitive?
    $n|a-b$ and $n|b-c$ does $n|a-c$?
    Yes.

Can a relation be both symmetric and anti-symmetric?
    Yes. 

## 9.1.5 - Combining Relations

7. Let $\mathcal{R}$ nd $\mathcal{S}$ be relations from $A$ to $B$. Using normal set operations,
    $\mathcal{R}\cup\mathcal{S}$, $\mathcal{R}\cap\mathcal{S}$, $\mathcal{R}-\mathcal{S}$, and $\mathcal{R}^c$ are all relations from $A$ to $B$

    (it just makes sense)

8. Let $\mathcal{R}$ be a relation from $A$ to $B$ and $\mathcal{S}$ from $B$ to $C$.
    The composition of $\mathcal{R}$ and $\mathcal{S}$, denoted $\mathcal{S} \circ\mathcal{R}$ is 
    (a normal composition)
    $\mathcal{R} \circ \mathcal{S}=\{(x,z)|\forall y\in B[(x,y)\in\mathcal{R}\ and\ (y,z)\in\mathcal{S}]\}\subseteq A\times C$

9. Let $A=\{0,1,2\}$, $B=\{x,y,z\}$ and $C=\{\alpha,\beta,\gamma\}$. Let $\mathcal{R}$ be a relation from $A$ to $B$ and 
    $\mathcal{S}$ be a relation from $B$ to $C$ defined by $\mathcal{R}=\{(0,x),(1,x),(1,y),(2,y),(2,z)$
    and $\mathcal{S}=\{(x,\beta),(y,\alpha),(y,\beta),(z,\alpha),(z,\gamma)\}$

$ \mathcal{S} \circ \mathcal{R}=\{(0,\beta),(1,\beta),(1,\alpha),(2,\beta),(2,\alpha),(2,\gamma)\}$

It's what you'd think of it's a little confusing because it's not a function but you have to follow all the paths

10. Let $A$ be a set. The identity relation on $A$ is 
$\Delta_A=\{(x,x)|x\in A\}\subseteq A\times A$

11. Iterative Powers exist 
Basis: $\mathcal{R}^0=\Delta_A$
Recursive Step: for $k\in\mathbb{Z}^+\mathcal{R}\circ\mathcal{R}^{k-1}$

12. Let $\mathcal{R}$ be a relation from $A$ to $B$. The inverse relation of $\mathcal{R}$ denoted $\mathcal{R}^-1$

13. Let $\mathcal{R}$ be a relation on $A$
i) $\mathcal{R}$ is reflexive if and only if $\Detla_A\subseteq\mathcal{R}$
ii) $\mathcal{R}$ is symmetric if and only if $\mathcal{R}=\mathcal{R}^-1$
iii) $\mathcal{R}$ is transitive if and only if $\mathcal{R}^2\subseteq\mathcal{R}$

proof of iii online 
