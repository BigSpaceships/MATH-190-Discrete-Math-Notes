# 6.3 - Permutations and Combinations

## 6.3.2 - Permutations

1. In a class of 10 students, five are to be chosen and seated in a row for a picture. How many such linear arrangements are possible?

$10 * 9 * 8 * 7 * 6 = 30,240$

This is a permutation, order matters

2. A permutation of a set of distinct objects is an ordered arrangement of these objects

3. If $A=\{1,2,3\}$, then $(1,2,3)$ and $(2,3,1)$ are permutations of $A$. How many permutations of $A$ are there

$(1,2,3)$
$(1,3,2)$
$(2,1,3)$
$(2,3,1)$
$(3,1,2)$
$(3,2,1)$

or

$3 * 2 * 1 = 6$

4. An r-permutation of $n$ distinct objects is an arrangement using $r$ of the $n$ objects.

Let $P(n,r)$ denote the number of $r$-permutations of a set with $n$ elements.
A formula is 

$P(n,r)=n!/(n-r)!$

Note that $P(n,0)=1$ and $P(n,n)=n!$

## 6.3.4 - Combinations 

5. An $r$-conbination of $n$ distinct objects is an unordered Selection, or subset, of $r$ out of the $n$ objects

Let $C(n,r)$ denote the number of $r$-combinations of a set with $n$ elements. 
A formula is 
$C(n,r)=n!/(r!(n-r)!)$

$C(n,r)$ is also called the binomial coeffcient and is frequently denoted $\begin{pmatrix}n \\ r\end{pmatrix}$, pronounced n choose r
Note that $C(n,0)=1$ and $C(n,n)=1$

6. A combinatorial proof of an identity is either 
- a proof that uses counting arguments to prove that both sides of the
identity count the same objects but in different ways (called a double
counting proof) or
- a proof that is based on showing that there is a bijection between the sets
of objects counted by the two sides of the identity (called a bijective
proof).

Question: How many r-permutations of A are there?

Answer #1: $P(n,r)$
Answer #2: Use two steps
    Task 1. Take out $r$ elements from $A$ in $C(n,r)$ ways
    Task 2. Rearange these $r$ elements in all possible ways
        There are $P(r,r) ways to do this

So $P(n,r)=C(n,r)*P(r,r)$
$=> C(n,r)=P(n,r)/(P(r,r)$
$= n!/(r!*(n-r)!)$

7. Prove that $|\mathcal{P}(S)| = 2^{|S|}$ for any finite set $S$ 

(On mycourses)

8. A committee of 12 is selected from 10 men and 10 women. In how many ways can the selection be carried out if...

a) there are no restrictions? $C(20,12) = 20!/(12!8!) = 125,970$
b) there must be six men and six women? $C(10,6) * C(10,6) = 10!/(6!4!) * 10!/(6!4!) = 44,100$
c) there must be more women than men? 
$half of a - b = (C(20,12) - C(10,6) * C(10,6)) / 2 = 40,935$
$C(10,7)*C(10,5) + C(10,8)*C(10,4) + C(10,9)*C(10,3) + C(10,10)*C(10,2)$

9. Suppose that Heather shuffles a deck and draws 5 cards, all at once, without regard to order. In how many ways can this be done if

a) There are no restrictions? $C(52,5) = 2,598,960$
b) There are no clubs? $C(39,5) = 575,757$
c) There is exactly one club? $C(13,1) * C(39,4) = 1,069,263$
d) There is at least two clubs? $C(13,2)*C(39,3) + C(13,3)*C(39,2) + C(13,4)*C(39,1) + C(13,5) = 953,940$
or a - b - c
