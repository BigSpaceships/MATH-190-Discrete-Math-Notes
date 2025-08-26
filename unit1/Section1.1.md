# 1.1.2 Propositions

1. A proposiiton is a delcarative sentenece that is true or false, but not both 
2. The truth value of a proposition is either T or F, not 0 or 1

## Examples

| Statement  | Proposition? | TV |
| --- | --- | --- |
| $5 + 7 <= 19$ | Yes | T |
| Did shakespear wirte his plays in old, middle, or modern english | No |   |
| Near the end of the 1939 film the wizard of oz, the scarecrow cites the pythagorean therom | Yes | F |
| $x + 3 = 7$ | No | |
| If Mr. Smith is elected, then he will lower taxes on the middle class | Yes | ? |
| There will be an exam next week, but you won't know which day it will be unitl you come into class that day | No - Paradox | |
| Every even integer greater than 2 is the sum of two prime numbers. | No - Not proven | | 


## Operations 

| Name | Symbol | Latex | Pronounced | True when | False when | 
| --- | --- | --- | --- | --- | --- |
| Negation | $\neg P$ | `\neg` | not p | p is false | p is true |
| Conjuction | $P \land Q$ | `\land` | p and q | p and q are true | at least one of p or q are false | 
| Disjunction | $P \lor Q$ | `\lor` | p or q | at least of one of p or q are true | both p and q are false |
| Exclusive or | $P \oplus P$ | `\oplus` | p or q, but not both | one of p and q is true, and the other is false | p and q are the true | 
| Implication | $P \implies Q$ | `\implies` | P implies Q | | |


# 1.1.3 Conditional statements 

A statement of the form if... then... is an implication 

4. Suppose prof. makes the following statemnt:
"If you score 94% or higher on the final exam, then your course grade will be an A"

p: "you score 94% or higher" 
q: "your course grade is an A"

(is the satement true) 

| Case | if p then q |
| --- | --- |
| p and q are true | T |
| p is true and q is false | F |
| p is false and q is true | T | 
| p and q are false | T |


Implication is also a conditional statement 

5. Given the implicaiton $p \implies q$, then
 - $q \implies p$ = converse
 - $\neg q\implies \neg p$ = contrapositive
 - $\neg p\implies \neg q$ = inverse

5. Given the proposition "If it is raining, then the lawn is wet"
What is the truth value of the proposition

p = "it is raining"
q = "the lawn is wet"
prop: $p\implies q$ is T
converse: $q\implies p$ is F
contrapositive: $\neg q\implies\neg p$ is T
inverse: $\neg p\implies\neg q$ is F

# 1.1.4 Truth table

A truth table is a compact way to evaluate the truth values of a proposition
| p | q | $p\land q$ | $p\lor q$ | $p\oplus q$ | $p\implies q$ |
| - | - | - | - | - | - |
| T | T | T | T | F | T |
| T | F | F | T | T | F |
| F | T | F | T | T | T |
| F | F | F | F | F | T |

