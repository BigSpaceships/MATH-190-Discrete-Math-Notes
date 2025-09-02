# Propositional Equvilance

## Definitions
a Tautology is a compound proposition that is always true
a contradiction is a compound proposition that is always false
a contingency is a compound proposition that is sometimes true and sometimes false

2. Determine the truth values of $p\iff p$ and $\neg(p\lor q)\iff\neg p \land\neg q$

a)
|a|$p\iff p$|
|-|-|
|T|T|
|F|T|


b)
|p|q|$\neg(p\lor q)\iff\neg p \land\neg q$|
|-|-|-|
|T|T|F T T F F F|
|T|F|F T T F F T|
|F|T|F T T T F F|
|F|F|T F T T T T|


3. Let P and Q be compound propsitions. if $p\leftrightarrow q$ is a tautology, than p and q are logically equivalent, written $p\equiv q$
This can also be written $p\iff q$

Notes:
- if P and Q are logically dquivalent, then P and Q have the exact same truth values
- $p\equiv q$ is not a propsition

$\mathbb{T}$ and $\mathbb{F}$ represent tautology and contraditions

4. $p\implies q$ is logically equivalent to its contrapositive ($\neg q\implies\neg p$)
$p\implies q\equiv\neg q\implies\neg p$

|p|q|$p\implies q\leftrightarrow\neg q\implies\neg p$|
|-|-|-|
|T|T|T T F T F|
|T|F|F T T F F|
|F|T|T T F T T|
|F|F|T T T T T|

Since $p\implies q\leftrightarrow\neg q\implies\neg p$, then $p\implies q\equiv\neg q\implies\neg p$

5. simplify $[a\land(a\to b)]\to\neg b$
$\equiv[a\land(a\to b)]\to\neg b$
$\equiv[a\land(\neg a\lor b)]\to\neg b$  [Law #1]
$\equiv[(a\land\neg a)\lor(a\land b)]\to\neg b$ [Distributive Law]
$\equiv[\mathbb{F}\lor(a\land b)]\to\neg b$ [Negation Law]
$\equiv[(a\land b)\lor\mathbb{F}]\to\neg b$ [Communative Law]
$\equiv a\land b\to\neg b$ [Identity Law]
$\equiv\neg(a\land b)\lor\neg b$ [Law #1]
$\equiv(\neg a\lor\neg b)\lor\neg b$ [Demorgan's Law]
$\equiv\neg a\lor(\neg b\lor\neg b$ [Associative Law]
$\equiv\neg a\lor\neg b$ [Idempotent Law]

6. Simplify $[\neg p\land(\neg p\to(q\to r))]\to\neg(q\to r)$
let $a\equiv\neg p$ and $b\equiv q\to r$
using example 5., our expression is equivalant to $\neg a\lor\neg b$
$\equiv\neg\neg p\lor\neg (q\to r)$
$\equiv p\lor\neg (q\to r)$ [Double negation law]

