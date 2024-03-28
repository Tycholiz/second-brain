
Permutations are the number of ways to choose a sample of $r$ elements from a set of $n$ distinct objects where **order matters**
- another way to visualize the "order matters" requirement is to imagine a dinner seating arrangement where we are trying to figure out how many different ways people can be seated at a table. Since each seat is not interchangeable, we say that *order matters*.

- ex. the combination on a lock, since the order of digits matters.
- ex. in social networks, there are the concepts of "friends" and "following". When discussing one user following another, we are talking permutatins, since me following Elton John does not equate to Elton John following me. If one day he does decide to follow me, there will be 2 different entries in the database: Kyle-EltonJohn and EltonJohn-Kyle.

when $r$ === $n$, then the problem simply becomes $n!$.

mn: think "*P*ermutation ... *P*osition"

There are 2 types:
- with repetition (e.g. a combination lock can use $3$ multiple times)
- without repetition (e.g. in how many different ways can I order these 16 billiard balls?)

## Permutations with Repetition
ex. combination lock, password

Formula:
$$
n^r
$$
- $n$ - total number of possibilities for that position
    - ex. in combo lock, each position has 10 possibilities from 0-9
- $r$ - total number of positions
    - ex. combo locks typically have 3 or 4 positions

## Permutations without Repetition $P(n,r)$
### Formula:
$$
n!
\over
(n − r)!
$$

If we are creating our permutation by using every value in the set, then our formula becomes a simple [[factorial|math.arithmetic.factorial]].
- this is because in the above formula, if our permutation size is the same as the total set size, the result is $0!$, or $1$, against which we divide our number.
- it helps to think of there being 2 types of "permutation without repetition":
    1. where all possible values are used in the result set
        - in this case, $n === r$, and therefore the denominator resolve to $1$, and therefore only have to consider the numerator.
    2. where some values remain out of the result set
        - in this case, we concern ourselves with the denominator, since now we must get the factorial of the difference of $n$ and $r$.

- the denominator part of this formula works because it is cancelling out the parts of the numerator we don't care about. For instance, if we have 16 pool balls but only care about 3, then we keep the 16, 15 and 14, but cancel out the 13, 12, 11  (and so on) of the numerator. 

$$
{16 × 15 × 14 × 13 × 12 × ...
\over
13 × 12 × ...}
=
16 × 15 × 14
$$

- With this long-form, we can see that the how it can be reduced to $16 x 15 x 14$.

In this case, we have to reduce the number of available choices each time.
- ex. what order could 16 pool balls be in?
    - 20,922,789,888,000
- ex. what order could 3 pool balls be in, out of a total of 16 balls?
    - 3,360

Of course, because $0! = 1$, if we plan to use all available elements in the sequence, then our formula is a simple factorial, due to the nature of dividing by 1.
- in other words, we can ignore the denominator part of the equation.

### examples: 
- ex. anagram (assuming that every combination is an actual word)
- ex. An encyclopedia has eight volumes. In how many ways can the eight volumes be replaced on the shelf?
- ex. How many different seatings arrangements are there for 6 guests?
    - Let us fill the seats one by one, starting with the chair on Alice’s right. We can put here any of the 6 guests. Now look at the second chair. If Bob sits on the first chair, we can put here any of the remaining 5 guests; if Carl sits there, we again have 5 choices, etc. So the number of ways to fill the first two chairs is $5 + 5 + 5 + 5 + 5 + 5 = 6 · 5 = 30$. Similarly, no matter how we fill the first two chairs, we have 4 choices for the third chair, which gives $6 · 5 · 4$ ways to fill the first three chairs. Going on similarly, we find that the number of ways to seat the guests is $6 · 5 · 4 · 3 · 2 · 1 = 720$