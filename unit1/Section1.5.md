# Nested Quantifiers 

1. Nexted Quantifiers occur when a propositional function of two or more variables has moe than one of its variables bound

2. What does the proposition $\forall x\exists y [x+y=0]$ mean? 
For every x, there exists a value y that $x + y = 0$

### 1.5.3 - The order of quantifiers

3. Let P(x,y) be a propositional function. 
Then $\forall x\forall y P(x,y)\equiv\forall y\forall x P(x,y)$
and $\exists x\exists y P(x,y)\equiv\exists y\exists xP(x,y)$

4. 
a) $\forall x\exists y [x+y=0]$ 
For every x, there exists a value y that $x + y = 0$

b) $\exists y\forall x [x + y = 0]$
For a value y, every value of exists such that $x + y = 0$ (False)

### 1.5.5 - Translating mathmatical statements into statements involing nested quantifiers

5. We say, for two functions, f and g, both defined from the
integers or the real numbers to the real numbers, f is Big-O of g if there are
constants C and k such that $|f (x)| <= C|g(x)|$ whenever x > k.

x, k, C

$ \forall x,\exists k,\exists C$

$[x>k\to|f(x)|<=C|g(x)]$

$ \exists k,\exists C,\forall x[x>k\to|f(x)|<=C|g(x)]$

the choice of k and C have to be chosen first so that you can say forall x

### 1.5.6 - Translating from nested quantifiers into enlgish

6.
a) $\forall x,\exists y[xy=1]$
F - when x = 0 this fails
b) $\forall x,\exists y[xy=1]\land x\neq 0$
F - Still false
c) $\forall x,\exists (x\neq 0)\to y[xy=1]$
T
d) $\forall x[x\neq 0\to\exists y(xy=1)]$
T - quantifiers can be inside they just have to be before the variables appear 

### 1.5.7 - Translating english sentences into logical expressions

7. Let V(x,y) be the statement "x has voted for y," where the domain for both variables consists of all citizens
of a country. Use tquantifiers to express each of the following statements

a) Everybody voted for Mr. Smith
$\forall x[V(x,'Mr Smith')]$

b) Everybody voted for at least one candidate
$\forall x,\exists y [V(x,y)]$

c) There are at least two people taht voted for Mr. Smith
$\exists x_1,\exists x_2[V(x_1,'Mr Smith')\land V(x_2, 'Mr Smith')\land(x_1\neq x_2)]$

d) There is exactly one person whom everyone has voted for
$\exists y_1,\forall x[V(x,y_1)\land\forall y_2(V(x,y_2)\to y_1=|y_2)]$
Shorthand $\exists!x$

$ \exists!y\forall x[V(x,y)]$

### 1.5.8 - Negating Nested Quantifiers
8. Express the negation of the proposition
$\forall x[(x\neq0)\to\exists y(xy=1)]$

$\neg\forall x[(x\neq0)\to\exists y(xy=1)]$
$\exists x\neg[(x\neq0)\to\exists y(xy=1)]$
$\exists x(x\neq 0)\land\neg\exists y(xy=1)$
$\exists x(x\neq 0)\land\forall y(\neg xy=1)$
$\exists x(x\neq 0)\land\forall y(xy\neq1)$

