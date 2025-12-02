# 6.2 - Pigeonhole Principle 

## 6.2.1 - Introduction

1. Let $A$ be a sset of 19 distinct integers chosen from the following collection of 34 integers:
    $1,4,7,10,13,...,97,100$

    Prove taht there must be two distinct integers in $A$ whose summ is 104

2. (Main idea): if $n+1$ objects are placed into $n$ boxes, then some box contains at least two objects

2. (The Pigeonhole Principle): if $n+1$ or more pigeons fly into $n$ pigeonholes, then at least one pigeonhole has two or more pigeons roosting in it

A basic outline of a using the pigoenhole priciple is as follows:
    1) explain how pigeonholes are labeled (include the number of pigeonholes being used)
    2) explain how objects are placed into the pigeonholes (include the number of objects we are using
    3) use the pigeonhole priciple to complete the proof

Solution to 1. 
    Label each pigeonhole with the following: 
        $\{1\}, \{4,100\}, \{7,97\}, ..., \{49,55\}, \{52\}$
    There are a total of 18 pigeonholes
    Place each element in $A$ into the corresponding pigeonhole,
    Then by the pigeonhole principle, there must be at least one pigeonhole with two numbers in it
    Those two sum to 104. $\qed$

2. (The Pigeonhole Principle -> functional version): If $A$ and $B$ are finites sets with $|A|>|B|$ and $f:A\to B$, then there exists $x,y\in A$ such that
    $x \neq y$ and $f(x)=f(y)$

3. Prove that among any five points in a square of side length 2, two of the points must be at most $\sqrt{2}$ units away from each other

## 6.2.2 - Generalized Pigeonhole Principle

4. Prove that in a theater with 1000 people, at least 3 share the same birthday.

$n=1000$, $k=366$, by the generalized pigeonhole principle, then the $\lceil n/k\rceil=\lceil 1000/366\rceil=3$ people with the same birthday

5. (The Generalized Pigeonhole Principle): If $n$ pigeons occupy $k$ pigeonholes, then at least one pigeonhole has $\lceil n / k\rceil$ pigeons roosting in it

## 6.2.3 - Some Elegant Applications of the Pigeonhole Principle

6. Assume that in a group of six people, each pair of idividuals consists of two friends or two enemies. Show that there are either three mutual friends or three mutual enemies in the group

7. The Ramsey Number $R(m,n)$, with $m,n\in\mathbb{Z}^+-\{1\}$, denotes the minimum number of people at a party such that there are either $m$ mutual friends or $n$ mutal enemies, 
    assuming that every pair of people at the party are friends or enemies

