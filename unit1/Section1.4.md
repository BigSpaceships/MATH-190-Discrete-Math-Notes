# Predicates and Quantifieres

### 1.4.2 - Predicates

1. For x a real number, let $p(x)$ be the proposition $x+3=7$. 
Then, $p(3)$, $p(4)$, and $p(\pi)$ are all propositions because they are either true or false

- $p(x)$ is call a proposiitonal function
- $x+3=7$ is called the predicate
- the set of values that x can possibliy be in the porpoositional function is called the universe of discourse or the domain

2. Let $R(x,y)$ be the propositional function $R(x,y): x+y=4$ where x and y are integers.
$R(1,2)$ is false but $R(1,3)$ is true

(Propositional functions can have multiple variables)

3. (Goldbach's conjecture): Let q(n) be the proposition q(n): "n can be written as the sum of two prime numbers" where the domain is the positive even integers.

$ q(4) \land q(6)\land q(8) \land q(10)\land q(12) \land ...$

### 1.4.3 - Quantifiers

4. Let $p(x)$ be a propositional function

The universal quantification of $p(x)$ is $\forall xp(x)$
 - meaning for all value of x, $p(x)$ is true

The existential quantification of $p(x)$ is $\exists xp(x)$
 - $p(x)$ is true for at least one value x


5. $p(x): "x+3=7"$ is a proposition when a specific number is substituted for x. 

Which quantifier makes $p(x)$ a proposition?

Both, both $\forall xp(x)$ and $\exists xp(x)$ because it is always a proposition

6. Given the propositional function $F(n): "2^{2^n} + 1"$ is a prime number

Conjecture: $\forall nF(n)$

|n|$2^{2^n}+1$|
|-|-|
|0|3|
|1|5|
|2|17|
|3|257|
|4|65537|
|5|4296297 - False 641 * 67006417 |


### 1.4.5 - Quantifiers with Restricted Domains
7. Let $p(x): "x>=0 \to |x|=x"$ and $q(x): "x>=0\land |x|=x"$ where the domain of discourse is the real numbers
is $\forall x p(x) \equiv \forall x q(x)$

No, $p(-1)\equiv T$ but $q(-1)\equiv F$

### 1.4.6 - Precidence of Quantifiers

What does $\forallx P(x)\to Q(x)$ mean

$(\forall xP(x))\to Q(x)$ or $\forall x(P(x)\to Q(x))$
The first one (USE PARANTHESIS)

### 1.4.7 - Binding Variables

9. When a variable is given a quantifier, the variable is called bound. Otherwise, it is free
- The part of logical expression to which a quantifier is applied is called the scope of this quantifier.

### 1.4.8 - Logical equivalences involving quantifiers

10. Prove or disprove the following

a) $\forall(P(x)\land Q(x))\equiv\forall P(x)\lor\forall Q(x)$

Proof:
$q\equiv q$ iff $q\iff q$ is a tautology
$p\to q \land q\to p$

do left side and right

Proof: suppose $\forall x(P(x)\land Q(x))$

That is, if a is in the domain, then the $P(a) \land Q(a)$ is true

Since $P(a)$ is true for every a in the domain,
then $\forall xP(x)$ is true

Since $Q(x)$ is true for every a in the domain,
then $\forall xQ(x)$ is true

Hence $\forall xP(x)\land\forall xQ(x)$ is true
Overall, $\forall x(P(x)\land Q(x))\to\forall xP(x)\land\forall xQ(x)$


b) $\forall(P(x)\to Q(x))\equiv\forall P(x)\to\forall Q(x)$

attempt 1
$p(x): "x>=0 \to |x|=x"$ and $q(x): "x>=0\land |x|=x"$

$\forall xP(x)\equiv T$ and  $\forall xQ(x)\equiv F$ but $T\to F\equiv F$

$\forall x(P(x)\to Q(x))\equiv F$

attempt 2

$p(x):$ "x is prime" and $q(x): "x^2 + 1 <0"$
When X is an integer

$\forall xP(x)\equiv F$ and  $\forall xQ(x)\equiv F$ but $F\to F\equiv T$

$x=2$
$P(2)\equiv T$ $Q(2)\equiv F$

$\forall x(P(x)\to Q(x))\equiv F$

### 1.4.9 - Negating Quantified Expressions

(back to 6) 
Given the propositional function $F(n): "2^{2^n} + 1"$ is a prime number

Conjecture: $\forall nF(n)$

$\forall nF(n)\equiv F$
$\neg\forall nF(n)\equiv T$
$\exists n\neg F(x)\equiv T$
11. 
$\neg\forall xp(x)\equiv\exists x\neg p(x)$

and 

$\neg\exists xP(x)\equiv\forall x\neg p(x)$

12. 
Suppose that the domain is the students ath the university. 
Let F(x): "x is a freshman" and C(x): "x is a computer science major".

Translate each of the following into symbolic propositions.
a) Some freshmen are computer science majors
$\exists x[F(x)\land C(x)]$

b) Every computer science major is a freshman
$\forall x[C(x)\to F(x)]$

c) No computer science major is a freshman
$\forall x[C(x)\to\neg F(x)]$



3. Cont.

let g(n) be the number of ways to write n as the sum of two prime numbers. 
The function g is called the Goldbach partial function

The plot of g from n = 0 to 1000

> TODO
> Figure out images

The plot of g from n = 0 to 1000000


