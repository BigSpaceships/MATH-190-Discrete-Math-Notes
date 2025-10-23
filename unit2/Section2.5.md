# 2.5 - Cardinality of Sets

## 2.5.1 - Intro

1. Two sets $A$ and $B$ have the same cardinality, written as $|A|=|B|$. if there is a bijection between two sets

$A=\{1,2,3\}$
$B=\{x,y,z\}$
$f=\{(1,x),(2,y),(3,z)\}$

Thus, $|A|=|B|$

2. Let $A$ and $B$ be sets. We say $A$ has less than or the same cardianlity than $B$, written $|A|\leq|B|$ 
if there exists a 1-1 function $f:A\to B$

## 2.5.2 - Countable sets

3. Let A be a set.
- A is countable if it is finite if $|A|=|\matbb{Z}^+|$
- A is countabley infinite if $|A|=|\matbb{Z}^+|$
- A is uncountable if it is not countable

4. Hilbert Hotel. This hotel has infinitely many rooms labled $r_1, r_2, r_3, r_4,...$

a) a guest arrives in the middle of the night at the hotel to find no vacency. How can the night clerk accomodate the guest?

Everyone moves one more room over 

b) the bus contains an infinite number of people. How can they be accomodated

Move from room $n$ to $2n$

c) infinite number of busses with infinite numbers of people

Room $n$ to $5^n$
$g_ij$ go to $2^i*3^j$

5. Show that the set of positive even integers $\mathbb{E}^+=\{2,4,6,8,...\}$ is countable (countably infinite)
Show: $|\mathbb{E}^+|=|\mathbb{Z}^+|$
Find a bijcetion $f:\mathbb{E}^+\to\mathbb{Z}^+$

Define $f:\mathbb{E}^+\to\mathbb{Z}^+$ by $f(n)=n/2$
Show $f$ is 1-1 and onto 
1-1: Suppose $m,n\in\mathbb{E}^+$ with $f(m)=f(n)$
Then $m/2=n/2$. Solving gives $m=n$. 
Hence $f$ is 1-1

Show $f$ is onto.
Suppose $q\in\mathbb{Z}^+$
Since $2q\in\mathbb{E}^+$ and $f(2q)=2q/2=q$
Thus, $f$ is onto

6. Is $\mathbb{Z}$ countable? Yes.

Find a bijection $f:\mathbb{Z}^+\to\mathbb{Z}$

defined as:

$ f(n)=\{n/2\ if\ n\ is\ even,\ (-n+1)/2\ if\ n\ is\ odd\}$

Show $f$ is 1-1 and onto

7. Is $Q$ countable

Yes

## 2.5.3 An uncountable set

8. Is the interval (0,1) countable?
No

9. All real numbers have at most two decimal representations

10. The number $x=0.a_1a_2a_3...$ where each $a_n\in\{0,1,2,...,9\}$ for $n\in\mathbb{Z}^+$, is said to be in normalized form 
    if there does not exist $N\in\mathbb{Z}$ such that $a_n=9$ for all $n>N$

Prove 8.
Proof by contradition
> Suppose (0,1) is countable
> Then $(0,1)=\{r_1,r_2,r_3...\}$
> In decimal form,
> $r_1=0.d_11d_12d_13...$
> $r_2=0.d_21d_22d_23...$
> $r_3=0.d_31d_32d_33...$
> ...
> $r_n=0.d_{n1}d_{n2}d_{n3}...d_{n}_{n}...$
> ...
>
> Construct a number $c=0c_1c_2c_3c_4...$
> That is not in the previous list
let $c_i=\{d_{ii}+1\ if\ d_{ii}<0,\ 0\ if\ d_ii=9\}$
>
> So c is not any of the numbers in the list

11. [Schroder-Bernstein]: Let $A$ and $B$ be sets. If $|A|\leq|B|$ and $|B|\leq|A|$, then $|A|=|B|$

Redo 7 with Schroder-Bernstein
We show $|\mathbb{Q}^+|=|\mathbb{Z}^+|$
When $x\in\mathbb{Q}$, we write $x=p\q$ and we presume that they have no common factors
Proof. Let $f:\mathbb{Q}^+\to\mathbb{Z}^+$ and $g:\mathbb{Z}^+\to\mathbb{Q}^+$
$f:(p/q)=2^p*3^q$
$g:(n)=n/1$
Both are 1-1. By the SB-theorem $|\mathbb{Q}^+|=|\mathbb{Z}^+|$

12.
Q1) the set of all finite strings over a finite alphabet is infinite, countable
Q2) the set of programs for a programming language is infinite, countable
Q3) the set of functions with domain and codomain $\mathbb{Z}^+$ is infinite, uncountable

13. The cardinality of real numbers is denoted $c$

14. Cantor's Theorem: for every set $A$, $|A|<|\mathcal{P}(A)|$

