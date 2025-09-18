# 1.8 Proof methods and Strategy

### 1.8.2 - Exhaustive proof and proof by cases

1. Suppose $n$ is an odd integer. Show that there exists and integer $k$ such that $n^2=8k+1$
> [Proof]
> Suppose $n$ is odd.
> By definition, there exists an integer $j$ such that $n=2j+1$.
> Squaring both sides gives $n^2=(2j+1)^2=4j^2+4j+1$
> Every integer is either odd or even. 
> [Case #1]
> Suppose $j$ is even.
> Then $j=2j_1$ for some integer $j_1$
> Then $n^2=4j^2+4j+1=4(2j_1)^2+4(2j_1)+1=16j_1^2+8j_1+1=8(2j_1^2+j_1)+1$
> Take $k=2j_1^2+j_1$ This implies $n^2=8k+1$
> [Case #2]
> Suppose $j$ is odd.
> Then $j=2j_2$ for some integer $j_2$
> then $n^2=4j^2+4j+1=4(2j_2+1)^2+4(2j_2+1)+1$
> $=4(4j_2^2+4j_2+1+8j_2+4+1=16j_2^2+16j_2+4+8j_2+4+1$
> $=16j_2^2+24j_2+8+1=9(2j_2^2+3j_2+1)+1$
> Take $k=2j_2^2+3j_2+1$ and so $n^2=8k+1$
> Since the statement holds for both cases, then we are done. $\qed$

### 1.8.3 - Existence Proofs

2. Prove that there exists an integer that can be expressed as the sum of two perfect cubes in two different ways.
> $1729$ - Taxicab number
> $7829=1^3+12^3=9^3+10^3$

3. Prove each of the following:
a) there eixists an irrational number $x$ and a rational number $y$ such that $x^y$ is rational
> $x=\sqrt{2}$, $y=2$
> $x^y=2$
b) there exists irrational numbers $x$ and $y$ such that $x^y$ is rational
> $x=\sqrt{2}$, $y=\sqrt{2}$ if $\sqrt{2}^\sqrt{2}$ is rational, then we wouold be done if $\sqrt{2}^\sqrt{2}$ is irrational, then consider $\sqrt{2}^\sqrt{2}^\sqrt{2}$
$=\sqrt{2}^(\sqrt{2}*\sqrt{2})$
$=\sqrt{2}^2=2$

### 1.8.5 - Proof Stratigies
5. Prove directly that if $x$ and $y$ are any real numbers, then $|x+y|\leq|x|+|y|$

Preliminary (not the proof)
$|x+y|\leq|x|+|y|$
$(x+y)^2\leq(|x|+|y|)^2$
$x^2+2xy+y^2\leq|x|^2+2|x||y|+|y|^2$
$x^2+2xy+y^2\leq x^2+2|xy|+y^2$
$2xy\leq 2|xy|$
$xy\leq|xy|$

> [Proof]
> Let $x$ and $y$ be real numbers.
> Since $|a|\geq a$ for any real number, we apply it to $xy$
> to get $|xy|\geq xy$
> Multiplying both sides of the previous inequlity by $2$ gives $2|xy|\geq 2xy$
> We add $x^2$ and $y^2$ to each side gives $x^2+2|xy|+y^2\geq x^2+2xy+y^2$ (eqn. *)
> The right hand side of (*) is a perfect square. 
> and can be simplified to $x^2+2xy+y^2=(x+y)^2$
> Consider the expression $x^2+2|xy|+y^2$ on the left hand side of (*)
> We rewrite $x^2$ and $y^2$ as $|x|^2$ and $|y|^2$, respectively
> We rewrite the middle term of the left hand size of (*) as $2|xy|=2|x||y|$
> Thus, the left hand side of (*) is $x^2+2|xy|+y^2=|x|^2+2|x||y|+|y|^2$
> $=(|x|+|y|)^2$
> Substituting back in both expressions into * gives
> $(|x|+|y|)^2\geq(x+y)^2$
> We take the square roots to get
> $|x|+|y|\geq|x+y|$


