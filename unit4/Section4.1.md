$ 4 - Divisibility and Modular Arithmetic
1) Let $m,n\in\mathbb{Z}$ we say that m divides n, written $m|n$, if there exists a (unique) integer $k$ such that $n=km$
- if $m|n$, then
  - m is called a factor or divisor of n
  - n is called a multiple of m
- write $m\not| n$
2.
a) $2|14$ T
b) 6 is a factor of 12
c) 8 is a multiple of 4
d) $5\not\divides 9$
e) $0|n$ false, $n|0$ true, $0|0$ false

3. Let $m,n,r,s\in\mathbb{Z}$
i) $m|n$ and $n|r$ implies $m|r$
ii) $m|n$ and $r|s$ implies $mr|ns$
iii) $m|n$ and $m|r$ implies $m|(an+br)$ for any integers $a$ and $b$

Proof if (iii):
> Suppose $m|n$ and $m|r$ and let $a,b\in\mathbb{Z}$ (show $m|(an+br)$)
> Since $m|n$, then there exists a $j\in\mathbb{Z}$ such that $mj=n$
> Since $m|r$, then there exists a $k\in\mathbb{Z}$ such that $mk=r$
> Since $an+br=a(mj)+b(mk)=m(aj+bk)$ and $aj+bk$ is an integer.
> So the defintion applies and $m|(an+br)$  $\qed$

## 4.1.2  The Division Algorithm 
4. The division algorithm: Let $a\in\mathbb{Z}$ and $d$ a positive iteger. then there are unique integers $q$ and $r$
    such that $a=qd+r$ and $0\leq r<d$

5. In the division algorithm, $d$ is the divisor, $q$ is the quotient, and $r$ is the remainder
- We write the quotient and remainder asociated to $a$ and $d$ as, respectively, $a\ div\ d$ and $a\ mod\ d$

TLDR:
Given $a$ and $d$,
$q=a\ div\ d=floor(a/d)$
$r=q\ mod\ d$
$a=qd+r$ -> $r=a-qd=a-floor(a/d)d$

6. What are the remainders and quotient when 
a) 83 is divided by 7
    $a=83$, $d=7$
    $q=floor(83/7)=11$
    $r=6$

b) -83 divided by 7
    $a=-83$, $d=7$
    $q=floor(-83/7)=-12$
    $r=-83-(-12*7)=1$

## 4.1.4 - Modular Arithmetic
7. Let $a,b\in\mathbb{Z}$ and let $m$ be a positive integer. We say that $a$ is congruent to $b$ modulo $m$, denoted $a\equiv b(mod\ m)$, if $m|(a-b)$
  - write $a\nequiv b(mod\ m)$ if $m\ndivides (a-b)$

8. determine if they are true or false
a) $3\equiv 3\ mod\ 8$ = $8|3-3$ T
b) $3\equiv 27\ mod\ 3$ = $8|(3-27)$ T
c) $27\equiv 3\ mod\ 8$ = $8|(27-3)$ T
d) $n\equiv n-1\ mod\ 8$ = $8|n-(n-1)$ = $8|1$ F
e) if $n$ is odd, then $n^2\equiv 1\ mod\ 8$ T, see Section 1.8 Ex. 1

## 4.1.5 - Arithmetic Modulo M
10. On $\mathbb{Z}_m$, we define the opperations of addition modulo m denoted $+_m$ and multiplication modulo m, denoted$*_m$.
        (do normal opperation, then mod m)

11. Let $m=6$
$+_m$

| |0|1|2|3|4|5|
|-|-|-|-|-|-|-|
|0|0|1|2|3|4|5|
|1|1|2|3|4|5|0|
|2|2|3|4|5|0|1|
|3|3|4|5|0|1|2|
|4|4|5|0|1|2|3|
|5|5|0|1|2|3|4|

$*_m$
| |0|1|2|3|4|5|
|-|-|-|-|-|-|-|
|0|0|0|0|0|0|0|
|1|0|1|2|3|4|5|
|2|0|2|4|0|2|4|
|3|0|3|0|3|0|3|
|4|0|4|2|0|4|2|
|5|0|5|4|3|2|1|

Properties of $\mathbb{Z}_m$ 
Closer:
Associtivity: $(a+b)+c=a+(b+c)$
Communitiveity: $a+b=b+a$, $ab=ba$
Idenentity elements: $0$ or $1$
Additive interses: let $a\in\mathbb{Z}_m$
Distributivity: AGH FILL THIS OUT I couldn't take notes fast enough
