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

