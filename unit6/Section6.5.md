# 6.5 - Generalized Perutations and Combinations

Given $n$ identical objects and $k$ distinguishable boxes, how many ways can we place the objects in those boxes

1. Three indistinguishable marbles are to be put into three containers labeled 
“Box 1”, “Box 2” and “Box 3”. In how many ways can this be done?

| Number | Box 1 | Box 2 | Box 3 | String |
| ------ | ----- | ----- | ----- | ------ |
| 1      | I I I |       |       | `***ll` | 
| 2      | I I   | I     |       | `**l*l` |
| 3      | I I   |       | I     | `**ll*` |
| 4      | I     | I I   |       | `*l**l` |
| 5      | I     |       | I I   | `*ll**` |
| 6      | I     | I     |       | `*l*l*` |
| 7      |       | I I I |       | `l***l` |
| 8      |       | I I   | I     | `l**l*` |
| 9      |       | I     | I I   | `l*l**` |
| 10     |       |       | I I I | `ll***` |


Strings with three `*` and two `|`

"how many ways to place three `*` in a sequence of length 5?"

5 choose 3 = 10

2. (Counting ways to place objects in boxes): There are $n+k-1 choose n$ = $n+k-1 choose k-1$ ways to place $n$ identical objects in $k$ boxes

3. Given some indistingishable marbles and 3 numbered bags. In how many ways can we place into the bags...

a) 10 marbles? $10+3-1 choose 10 = 12 choose 10 = 66$

b) 10 barbles with at least one in each bag?
Put one marble in each bag, distribue the rest.
$7+3-1 choose 7 = 9 choose 7 = 36$

c) 10 marbles such that there is one bag that contains at least 6 marbles 
Place 6 marbles in any bag, 3 ways
Distribute remaining 4 marbles in bags, $4+3-1 choose 4 = 6 choose 4 = 15$

$3 * 15 = 45$

d) 10 marbles such that there is one bag that contains at least 4 bags?
There would always be 4 marbles in at least one, (pidgeonhole principle) so the same as a, $66$

e) 14 marbles such that there are no more than 6 marbles in each bag? 

f) 14 marbles such that there are no more than 11 marbles in each bag?

How many ways can you select $n$ objects from $k$ groups of identical objects?

$n+k-1 choose n$ 

4. How many different strings can be made by reordering the letters of the word EVERGREEN?

9 total letters, 4 Es, 2 Rs

$9! / 4! / 2!$

5. The number of different permutations of $n$ objects, where there are $n_i$ indistinguishable objects of type 1, $n_2$ indisitinguishable objects of type 2,..., 
and $n_k$ indistingishable objects of type $k$ is 

$n!/(n_1! n_2! \cdots\ n_k!)$
