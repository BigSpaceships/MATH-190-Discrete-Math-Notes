# 9.2 - N-ary relation and their applications

## 9.2.1 - Intro

1. Let $A_1,A_2,...,A_n$ be sets. an n-ary relation on those sets is a subset of $A_1\times A_2\times ...\times A_n$. 
    The sets $A_1\times A_2\times ...\times A_n$ are called the domains of the relation and $n$ is called it's degree

2. Let $\mathcal{R}$ be the relation on $\mathbb{Z}\times\mathbb{Z}\times\mathbb{Z}^+$ defined by
    $\mathcal{R}=\{(a,b,m)|a\equiv b(mod m)\}\subseteq\mathbb{Z}\times\mathbb{Z}\times\mathbb{Z}^+$

True or false?

a) $(8,2,3)\in\mathcal{R}$, T ($8\equiv 2 (mod 3)$, $3|8-2$)
b) $(7,2,3)\in\mathcal{R}$, F ($7\equiv 2 (mod 3)$, $3|7-2$)
c) $(-1,9,5)\in\mathcal{R}$, T ($-1\equiv 8 (mod 5)$, $5|-1-9$)
d) $(-2,-5,5)\in\mathcal{R}$, F ($-2\equiv -5 (mod 5)$, $5| -2-5$)
