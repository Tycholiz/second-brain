
Combinatorics is closely related to [[probability|statistics.probability]] in cases where each combination is equally likely.
- if each combination/permutation is equally likely, then the odds of landing upon any particular set is equal to the total possible number of sets.

When determining the result of a combinatorics question, you must ask:
1. does order of the result set matter?
    - if yes, it's a [[permutation|math.combinatorics.permutations]]
    - if no, it's a [[combination|math.combinatorics.combinations]]
2. can the same value be used multiple times?
    - if yes, it's a (permutation/combination) with repetition
    - if no, it's a (permutation/combination) without repetition

Each combination of the 4 possibilities will yield a different formula.

## The Basic Counting Principle
When there are $m$ ways to do one thing, and $n$ ways to do another, then there are $m×n$ ways of doing both.

- ex. there are 3 girls and 4 boys, meaning there can be 12 possible pairs.
- ex. you have 3 shirts and 4 pants, meaning $3×4=12$ different outfits.
- ex. a password consists of 2 letters followed by 3 numbers ([[a permutation with repetition|math.combinatorics.permutations#permutations-with-repetition]]). To get the number of total possible passwords, we have to get the # of possibilities of the letter part and multiply it by the # of possibilities for the number part. (answer: 676,000)
- ex. I want to buy a car. It can be any combination of:
    - type: sedan, hatchback
    - color: red, blue, green
    - trim: standard, sports, luxury
    - Therefore, $2 \times 3 \times 3 = 18$ possible combinations
- this formula only works when **choices are independent** of each other (such as when we have the logic "black hatchbacks are not possible")

## Handshake problem
If there are 7 people at a party and each of them shake hands, how many handshakes were there?

$$
handshakes = n*{(n - 1)\over2}
$$

This is because each of the n people can shake hands with n - 1 people (they would not shake their own hand, which is why we divide by 2), and the handshake between two people is not counted twice.

## Chess board combinations
If there are 6 players and 3 chess boards, how many different combinations of players can there be?
- 2 players at the same chess board switching places (ie. black/white) counts as 1 combination
- it does not matter which board the same pair of players sits at.

$$
combinations = (n - 1) \times r
$$
$$
combinations = 5 \times 3 = 15
$$

Or:
$$
n! \over 2^r \times n
$$
$$
{6! \over 2^3 \times 6} = 15
$$
