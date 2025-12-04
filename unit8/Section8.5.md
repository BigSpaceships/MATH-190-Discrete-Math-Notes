# 8.5 – Inclusion - Exclusion

1. (Counting Elements in Set Unions): Let $A$, $B$, and $C$ be finite sets. The number of elements in the union is 
$|A \cup\ B \cup\ C| = |A| + |B| + |C| - |A \cap\ B| - |A \cap\ C| - |B \cap\ C| + |A \cap\ B \cap\ C|$

8. (The generalized inclusion-Exclusion Principle): Let $A_1, A_2, A_3, \dots, A_n$ be sets with $X=\{1,2,3,\dots, n\}$ then
$|\bigcup_{k\in\{1,2,3,\dots,n\}}A_k| = \sum_{I\in\mathcal{P}(X)}(-1)^{|I|+1}|\bigcup_{k\in I}A_k|$

where $\mathcal{P}(X)$ is the power set of $X$
