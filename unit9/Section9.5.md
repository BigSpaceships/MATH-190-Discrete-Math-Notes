# 9.5 - Equivalence Relations

## 9.5.2 - Equivalence Relations

1. A relation on $\mathcal{R}$ on set $A$ is an equivalence relation if it is reflexive, symmetric, and transitive.

## 9.5.3 - Equivalence Classes

2. Let $\mathcal{R}$ be an equivalence relation on $A$. The equivalence class 
of an element $a\in A$, denoted $[a]_\mathcal{R}$, is 
    $[a]_\mathcal{R}=\{b\in A|(a,b)\in\mathcal{R}\}$

if $b\in[a]_\mathcal{R}$, theb b is called a representative of the equivalence class

3. Let $\mathcal{R}$ be the relation on $\mathbb{Z}$ defined by $\mathcal{R}=\{(a,b)|a\equiv b (mod 4)\}\subseteq\mathbb{Z}\times\mathbb{Z}$ is an equivalence relation.
What are the quivalence classes?

What is $[0]_\mathcal{R}$? 
$[0]_\mathcal{R}=\{b\in\mathbb{Z} | (0,b0\in\mathcal{R}\}$
$=\{b\in\mathbb{Z} | 0\equiv b (mod 4)$
$=\{b\in\mathbb{Z} | 4|0-b\}$
$=\{b\in\mathbb{Z} | 4|-b\}$
$=\{b\in\mathbb{Z} | 4|b\}=\{...,-8,-4,0,4,8,...\}$

$[4]_\mathcal{R}=\{...,-8,-4,0,4,8,...\}$

$ [1]_\mathcal{R}=\{b\in\mathbb{Z} | 1\equiv b (mod 4)\}$
$ =\{4k+1|k\in\mathbb{Z}\}$
$ =\{...,-7,-3,1,5,9,13,...\}$

$ [0]_\mathcal{R} \cup [1]_\mathcal{R} \cup [2]_\mathcal{R} \cup [3]_\mathcal{R} = \mathbb{Z}$
$ [0]_\mathcal{R} \cap [1]_\mathcal{R} = \emptyset$

## 9.5.4 - Equivialence classes and partitions 

5. A collection of sets is pairwise disjoint if every two distinct sets $A$ and $B$ in teh collection satisfies $A\cup B=\emptyset$

6. Let $S$ be a set. We say a collection of sets $\{ A_n | n\in I\}$ (where $I$ is an indexed set) is a a partition of $S$ if 
    i) $A_i \subseteq S$ for every $i\in I$
    ii) $\emptyset$ is not in the collection
    iii) the collection is pairwise disjoint
    iv) the union of all sets in the collection is exactly $S$

7. Which of the following are partitions of $S=\{1,2,3,4,5,6\}$

a) $\{1,2\}, \{2,3,4\}, \{4,5,6\}$ no - not pairwise disjoint
b) $\{1\}, \{2,3,6\}, \{4\}, \{5\}$ yes
c) $\{2,4,6\}, \{1,3,5\}$ yes
d) $\{1,4,5\}, \{2,6\}$ no - missing 3

8. 
a) Let $\mathcal{R}$ be an equivalence relation on a set $S$. The equivalence classes of $\mathcal{R}$ form a partitions of $S$
b) Given a partition $\{ A_i | i\in I\}$ of a set $S$, then there is an equivalence relation $\mathcal{R}$ whos equivalence classes are $\{ A_i | i\in I\}$


