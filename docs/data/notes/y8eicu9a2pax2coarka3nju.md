
The number of ways to choose a sample of $r$ elements from a set of $n$ distinct objects where order **does not matter**.
- therefore, given the same set of values, the amount of [[permutations|math.combinatorics.permutations]] will always outnumber the amount of combinations.
- ex. My fruit salad is a combination of apples, grapes and bananas
- ex. Lotteries, since the order of the numbers chosen does not matter.
- ex. in social networks, there are the concepts of "friends" and "following". When discussing friendships between 2 people, we are talking combinations, since a friendship is a handshake and once established, order no longer matters.

## Combinations without Repetition
In combinatorics we say "n choose r" (such as "16 choose 3") and is written $\binom{16}{3}$
- ex. creating a combination (ie. order doesn't matter) of 3 billiard balls out of a total of 16 (*16 choose 3*)
    - note that by simply changing the problem so that we no longer care about order, we go from 
- ex. choosing a committee of 5 people from a pool of 10

Formulaically speaking, we think of a combination as a "permutation where order doesn't matter". In other words, we approach a combination by figuring out the permutation first, then adjusting for the new fact that order doesn't matter. 
- Therefore, the formula for calculating a combination is identical to the formula for a [[permutation|math.combinatorics.permutations]], save for one detail: since given the same set, there will always be more permutations than combinations, we have to reduce the result by increasing the size of the denominator.
- in fact, we can derive the probability of combination by taking the probability of permutation and dividing it by $r!$
    - ex. permutations of 6 lotto balls numbered between 1-44 are 10,068,347,520, but number of combinations is $10,068,347,520 / 6! = 13,983,816$ 

### Formula

$$
n!
\over
r!(n−r)!
$$
- $n$ - total number of possibilities for that position
    - ex. in combo lock, each position has 10 possibilities from 0-9
- $r$ - total number of positions
    - ex. combo locks typically have 3 or 4 positions

### Examples
- ex. if we have a set of 16 billiard balls and are choosing all 16, we can see how there is only 1 possible combination. Plugging these numbers into the formula, we can see that the denominator becomes identical to the numerator, yielding $1$.
- ex. if we have 100 commodities and we want to know how many exchange rates there are, the problem can be restated as "how many combinations of 2 numbers are there out of a possible 100?"
$$
{100!
\over
2! • (100 - 2)!}
=
4,950
$$

### Combinations with Repetition
- ex. We have an icecream cone with 3 scoops where multiple scoops of the same flavor is allowed. How many combinations can we get?
    - Let us say there are five flavors of icecream: banana, chocolate, lemon, strawberry and vanilla, denoted `{b, c, l, s, v}`.
    - This problem gets framed a bit differently. Think in terms of each possible value as having come from a source (e.g. a single chocolate scoop came from box of chocolate ice cream)

![](/assets/images/2022-12-17-13-25-52.png)
- If we were programming a robot to scoop icecream for us, we'd give it directions like: 
    - move right, 
    - scoop, 
    - scoop, 
    - scoop, 
    - move right, 
    - move right, 
    - move right
- So instead of worrying about different flavors, we have a simpler question: "how many different ways can we arrange each step of the robot's process?"
    - put another way, how many different combination of each of the 7 steps above are there? (this is how the parenthesis part of the numerator is calculated)
    - This is like saying "we have 7 pool balls and want to choose 3 of them"

$$
(r + n − 1)!
\over
r!(n − 1)!
$$
$$
{(3 + 5 − 1)!
\over
3!(5 − 1)!}
=
35
$$