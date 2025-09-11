# Rules of Inference

### 1.6.1 - Introduction 
1. 
- An arguement is a finite sequence of propositions (called the premises or hypotheses) intended to establish another proposition (called the conclusion)
- An argment is valid if the truth of all its premises imples that the conclusion is true
- An argment form is a sequence of compound propositions involing propositional variables

An argment of premises $p_1, p_2, p_3, ..., p_k$ and a conclusion q such that 
when all the ps are true, $p\to q$

### 1.6.2 - Valid arguements in propositional logic

2.
if it is raining, then the law is wet $R\to W$
it is raining $R$

---
Therefore, the lawn is wet $W$

### 1.6.3 - Rules of inference
They cannot be reversed 

list online maybe i'll type it out someday

### 1.6.4 - Using rules of inference to bulid argument

3. Show that the following arugment is valid using rules of inference and laws of equivalences

If the car is not empty, then it is not sunny $\neg F\to\neg S$
It is sunny or lunchtime $S\lor L$
It is not lunchtime $\neg L$

---
Therefore, the car is empty $\therefore F$

Proof:
|Step|Lines|Reason|
|-|-|-|
|$\neg F\to\neg S$| | Premise |
|$S\lor L$| | Premise |
|$\neg L$| | Premise |
|$S\to F$|1|Contrapositive (LE)|
|$L\lor S$|2|Communitive (LE)|
|$S$|2,5|Disjuctive syllogism (ROI)|
|$F$|4,6|Modus Ponens (ROI)|


4. A valid proof (formal proof) is an arguemtn from a sequence of propositions $p_1,p_2,p_3,...p_k$ where each $p_i$ is either
- A premise
- A logical equivalence
- A consequence using a rule of inference
and the last proposition in the proof is the conlcusion of the arguement 

5. Use a valid proof to take premises $(p\to q)\land r$, $\neg(q\land q)$ and $s\to p$, to conlcude $\neg s$

|#|Step|Lines|Reason|
|-|-|-|-|
|1|$(p\to q)\land r$| |Premise|
|2|$\neg(r\land q)$| | Premise|
|3|$s\to p$| | Premise |
|4|$\neg r \lor\neg q$| 2 | DeMorgan's Law|
|5|$p\to q$| 1 | Simplification (ROI)|
|6|$r\land(p\to q)$|1|Communitive (LE)|
|7|$r$|6| Simplification (ROI) |
|8|$\neg\neg r$|7|Double Negation (LE)|
|9|$\neg q$|4, 8| Disjunctive Syllogism (ROI)|
|10|

> [!TODO]
> finish this

### 1.6.6 - Fallacies

6. 
- The arguement $((p\to q)\land q)\to p$ is invalid is called the fallacy of affirming the conclusion
- The arugment $((p\to q)\land\neg p)\to\neg q$ is invalid and is called the fallacy of denying the hypothesis

### 1.6.7 - Rules of inference for Quantified Statements

7. Let P be a propositional function of one variable
- Universal instantiation takes $\forall xP(x)$ and concludes $P(c)$, where c is a member in the domain of $P$
- Universal generalization takes $P(c)$ for some arbitrary member $c$ in the domain of $P$ and conlcudes $\forall xP(x)$
- Existential instantiation takes $\exists xP(x)$ and conclludes $P(c)$ for some member c in the domain of $P$
- Existential generalization takes $P(c)$ for some arbitrary member $c$ in the domain of $P$ and conclludes $\exists xP(x)$

### 1.6.8 - Combining Rules of Inference for Propositions and Quantified Statements

8. 
Consider the domain to be the students in a college
$m$ is Mark Kelley
$j(x)$: $x$ is a junior
$s(x)$: $x$ is a senior
$p(x)$: $x$ is inrolled in a physical education class

Prove the Argument:
No junior or senior is enrolled in a physical education class.
Mary Kelley is enrolled in a physical education class.
Therefore, Mary Kelly is not a senior

$\forall x[(j(x)\lor s(x))\to\neg p(x)$
$p(m)$

$ \therefore\neg s(m)$

| |Step|Lines|Reason|
|-|-|-|-|
|1|$\forall x[(j(x))\lor s(x))\to\neg p(x)$| |Premise|
|2|$p(m)$| |Premise|
|3|$j(m)\lor(s(m)\to\neg p(m)$|1|Universal instantiation|
|4|$\neg\neg p(m)\to\neg(j(m)\lor g(m)$|3|Contrapositive|
|5|$p(m)\to\neg(j(m)\lor g(m)$|4|Double negation|
|6|$\neg(j(m)\lor s(m)$|2, 5|Motus Ponems|
|7|$\neg j(m)\land\neg s(m)$|6|DeMorgan's Law|
|8|$\neg s(m)\land\neg j(m)$|7|Communitive Law|
|9|$\neg s(m)$|8|Simplification|


