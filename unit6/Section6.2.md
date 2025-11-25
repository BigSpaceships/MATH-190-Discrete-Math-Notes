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

