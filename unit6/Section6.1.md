# 6.1 - The basics of counting

## 6.1.1 - Introduction

1a. A college library has 200 textbooks in physcis and 350 in economics.
    How many ways can a student learn about one or the other of the subjects

550

1b. The drama club of a college is holding tryouts for a play.
    Eight men and five women are auditioning for the leading male and
    female roles. In how many ways can the director cast the leading couple?

## 6.1.2 - Basic counting principles

2. The Sum rule: If a first task can be performed in $m$ ways, while a second task can be performed in $n$ ways, 
    and the two tasks cannot be performed simultaneously, then performing either task can be
    accomplished in any one of $m + n$ ways.

3. The product rule: Suppose a procedure can be broken down
    into a sequence of two tasks. If there $m$ ways to do the first task and $n$
    ways to do the second task after the first task has been done, then there are
    $mn$ ways to do the procedure.

4. A coffee shop sells six kinds of soups, eight kinds of
    sandwiches, and five beverages (hot coffee, hot tea, iced tea, cola, and
    orange juice). Each day a student buys a lunch consisting of a soup and a
    cold beverage, or a sandwich and a hot beverage. In how many ways can
    the student buy lunch?

$6$ soups, $8$ sandwiches, $5$ beverages ($2$ hot, $3$ cold)

soup and cold = $6 * 3 = 18$
sandwhich and hot = $8 * 2 = 16$
(soup and cold) OR (sandwhich and hot) = $18 + 16 = 34$

## 6.1.3 - More complex counting problems

5. How many strings of four decimal digits can be formed
    a) no restrictions: $10*10*10*10=10^4=10,000$
    b) that do not contain the same digit twice: $10*9*8*7=5040$
    c) that have exactly three digits that are 7s: 4 places to put the not 7, with 9 other choices $7*9=63$
    d) includes at least one 5: 
        NOT 4 places to put the 5, 10 options for each of the other ones $4 * 10 * 10 * 10 = 4000$
            when you pick the 5 and then have two, it gets double counted
        could do ways to get one 5 + two 5s + three 5s + four 5s:
            $4 * 9 * 9 * 9 + 4 * 3 / 2 * 9 * 9 + 4 * 3 * 2 / 6 * 9 + 1 = 3439$
        could do total number - total that have no 5s: $10^4 - 9 * 9 * 9 * 9 = 10^4 - 9^4 = 3439$

6. (Counting Elements in Complements): Let $A$ be a set with $U$ the
universal set containing a finite number of elements, then
$|\conj{A}| = |U| - |A|$

7. How many bit strings of length nine either start with a 0 bit or end with the three bits 101


start with a 0 (control 1 bit)
$0 2 2 2 2 2 2 2 2$
$_ _ _ _ _ _ _ _ _$

$2^8$

End with 101 (control 3 bits)

$2^6$

Start with 0 and end with 101 (control 4 bits)

$2^5$

$ 2^8 + 2^6 - 2^5$

$288$

8.  (Counting Elements in Set Unions): Let $A$ and $B$ be finite sets.
The number of elements in the union is $|A \cup B| = |A| + |B| - |A \cap B|$
