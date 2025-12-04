# 9.3 - Representing Relations

## 9.3.2 - Representing Relations using matricies 

1. Let $\mathcal{R}$ be a relation from $A=\{a_1,a_2,...,a_m\}$ to $B=\{b_1,b_2,...,b_n\}$.
    The matrix representation of $\mathcal{R}$, denoted $M_{\mathcal{R}}$, is the $m\times n$ $M_{\mathcal{R}}=[m_ij]_{m\times n}$

$m_ij=\{1, if (a_i,b_j)\in\mathcal{R}, 0 if (a_i,b_j)\notin\mathcal{R}$

2. Let $A=\{x,y,z\}$. Let $\mathcal{R}$, $\mathcal{S}$ be relations on $A$ defined by
    $\mathcal{R}=\{(x,y),(y,y),(z,x)\}$ and $\mathcal{S}=\{(x,x), (x,y), (y,y), (y,z), (z,x), (z,z)\}$

a) $M_\mathcal{R} = \begin{bmatrix} 0 & 1 & 0 \\ 0 & 1 & 0 \\ 1 & 0 & 0 \end{bmatrix}$

b) $M_\mathcal{S} = \begin{bmatrix} 1 & 1 & 0 \\ 0 & 1 & 1 \\ 1 & 0 & 1 \end{bmatrix}$

c) $M_{\mathcal{R}^-1} = M_\mathcal{R}^T = \begin{bmatrix} 0 & 0 & 1 \\ 1 & 1 & 0 \\ 0 & 0 & 0 \end{bmatrix}$

d) $M_\mathcal{R}^C = 1 - M_\mathcal{R} = \begin{bmatrix} 1 & 0 & 1 \\ 1 & 0 & 1 \\ 0 & 1 & 1 \end{bmatrix}$

3. Given $A=[a_ij]_{m\times n}$ and $B=[b_ij]_{m\times n}$, $A$ precceds $B$, denoted $A\leq B$, 
    if all elements are in $A$ are less than or equal to their corresponding element in $B$

4. Let $\mathcal{R}$ and $\mathcal{S}$ be relations given by the matrix representations

$ M_\mathcal{R}=\begin{bmatrix} 1 & 1 & 1 \\ 0 & 1 & 1 \\ 0 & 0 & 1 \end{bmatrix}$
$ M_\mathcal{S}=\begin{bmatrix} 1 & 1 & 0 \\ 1 & 0 & 1 \\ 0 & 0 & 1 \end{bmatrix}$

a) 

i) $M_{\mathcal{R}\cup\mathcal{S}}=\begin{bmatrix} 1 & 1 & 1 \\ 1 & 1 & 1 \\ 0 & 0 & 1 \end{bmatrix}$
ii) $_{\mathcal{R}\cap\mathcal{S}}=\begin{bmatrix} 1 & 1 & 0 \\ 0 & 0 & 1 \\ 0 & 0 & 1 \end{bmatrix}$

b)
The Relation $\mathcal{R}$ is 
Reflexive? Yes
Symetric? No
Antisymetric? Yes
Transitive? Good question (TBD)

The Relation $\mathcal{S}$ is 
Reflexive? No
Symetric? No
Antisymetric? No
Transitive? Good question (TBD)

5. Let $\mathcal{R}$ and $\mathcal{S}$ be relations from $A$ to $B$. Then $M_{\mathcal{R}\cup\mathcal{S}}=M_\mathcal{R}\lor\mathcal{S}$
and $M_{\mathcal{R}\cap\mathcal{S}}=M_\mathcal{R}\land\mathcal{S}$

6. Let $A=\{0,1,2\}$, $B=\{x,y,z\}$, $C=\{\alpha,\beta,\gamma\}$. Let $\mathcal{R}$ be a relation 
from $A$ to $B$ and $\mathcal{S}$ be a relation from $B$ to $C$ defined by 
$\mathcal{R}=\{(0,x),(1,x),(1,y),(2,y),(2,z)\}$ and $\mathcal{S}=\{(x,\beta),(y,\alpha),(y,\beta),(z,\alpha),(z,\gamma)\}$

$ M_\mathcal{R} = \begin{bmatrix} 1 & 0 & 0 \\ 1 & 1 & 0 \\ 0 & 1 & 1 \end{bmatrix}$

$ M_\mathcal{S} = \begin{bmatrix} 0 & 1 & 0 \\ 1 & 1 & 0 \\ 1 & 0 & 1 \end{bmatrix}$

Determine $M_\mathcal{R} \odot\ M_\mathcal{S}$ (boolean product)

$M_\mathcal{R} \odot\ M_\mathcal{S} = \begin{bmatrix} 0 & 1 & 0 \\ 1 & 1 & 0 \\ 1 & 1 & 1 \end{bmatrix}$

corresponding relation: 
$\{(0,\beta),(1,\alpha),(1,\beta),(2,\alpha),(2,\beta),(2,\gamma)\}$

7. Let $\mathcal{R}$ be a relation from $A$ to $B$ and $\mathcal{S}$ is a relation from $B$ to $C$

Then $M_{\mathcal{R}\circ\mathcal{S}}=M_\mathcal{R} \odot\ M_\mathcal{S}$

8. Let $\mathcal{R}$ be a relation on $A$
i) $\mathcal{R}$ is reflexive if and only if $I\leq M_\mathcal{R}$
ii) $\mathcal{R}$ is symmetric if and only if $M_\mathcal{R}=(M_\mathcal{R}))^t$
iii) $\mathcal{R}$ is transitive if and only if $(M_\mathcal{R})^[2]\leq M_\mathcal{R}$

## 9.3.3 - Representing Relations using Digraphs

9. Draw a digraph representation fo the relation $\mathcal{R}$ on $A=\{1,2,3,4\}$
defined by $\mathcal{R}=\{(1,1),(2,2),(2,3),(3,2),(3,3),(3,4),(4,2)\}\subseteq A\times A$

uhhhh idk how to take notes on this you put all the points down and draw arrows for each connection in the relation

Reflexive: No, each node has to have an edge to itself
Symetric: No, each edge has to have arrows in both directions
Antisymetric: No, each edge can't be a double edge 
Transitive: No, 2->3, 3->4, but not 2->4
