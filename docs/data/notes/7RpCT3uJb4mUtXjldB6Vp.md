
Probability and relative frequency are two sides of the same coin.

### Denominator neglect
Low probability events are taken more seriously (ie. Given more weight) when described in terms of relative frequency (e.g. How many times out of 100 it will occur), than when described in abstract terms of probability
- ex. "There is a .001% chance you child will get cancer and die" vs. "1 / 100,000 children will get cancer and die".
	- The second example is more vivid, leading us to imagine it, and produce cognitive ease. This makes a better story, and makes its likelihood seem higher

### How to determine probability
first access with a base rate is if I am asking what are the odds that Jim is a teacher that I have to find out how many teachers in the population are. For instance if .1% of the population are teachers, with such limited information I must conclude that there is a .1% chance that Jim is a teacher. this is the base rate probability and we should always start here first. from there we can adjust the probability up or down depending on what extra information we have.

### Bayes' Theorem
Bayes’ theorem is a probabilistic approach towards incorporating new information into the model as it becomes available, and updating the probability as a result.
- The act of adjusting our assessment of the probability is called `Bayesian inference`

Describe the probability of an event occurring based on prior knowledge that may relate to the event.
- ex. if the risk of developing health problems is known to increase with age, Bayes’s theorem allows us to assess the risk more accurately, by including the age in the model. Otherwise, we are just assuming that the individual is typical of the population as a whole.

### Zipf's law
Zipf's law states: "given a large sample of words used, the frequency of any word is inversely proportional to its rank in the frequency table." 
- So *n*th word has a frequency proportional to 1/n.
- this means that the second most common word (*of*) will appear 1/2 as often as the most common (*the*), and the third most common (*and*) word will appear 1/3 as often as the most common (*the*)
- this also means that only about 135 words are needed to account for half the sample of words in a large sample. This holds true for most languages, though the reason is not well understood.

Zipf's law applies to:
- the population ranks of cities in various countries, 
- corporation sizes, 
- income rankings, 
- etc. 

# Echo Chamber Danger
- If all people in one group are coming to similar conclusions, it could be a sign of an echo chamber. Conversely if very different people are saying the same thing, they're probably right.
    - The likelihood of people using different data (ie. a different source of information) and different perspectives and still arriving at the same conclusion is low.

improbable things happen all the time because "improbability" is an illusion based on our preconceptions. Often it has nothing to do with statistical truth. The trouble is that we can't grasp the difference between (a) "This particular improbable pattern of lottery numbers came up on this particular day in this particular lottery" and (b) "Some improbable pattern of lottery numbers came up sometime in the last five years somewhere in the world." In short: "improbability" does not imply "impossibility".

### The Same Birthday
Consider a party attended by thirty people: what are the chances that two of them have the same birthday? One in twelve, or, roughly 8% (30/365)? After all, it's a 1 in 365 chance someone will share your birthday, and by the lottery analogy above, there's 30 shots at winning.

No, the odds are significantly better than that. In fact, there is a 70% probability.

This is known as the "birthday problem". The apparently miraculous breaking of odds is attributed to the fact that the question is "what is the chance that any two people have the same birthday?", whereas most people following common sense tend to translate the question as "what is the chance that someone has the same birthday as mine?". So while you get 30 shots at this 1 in 365 lottery, so does everyone else. More specifically, every possible pairings of two individuals in the group of 30 has a shot at this 1 in 365 chance. Regardless, the answer is very non-intuitive and is a good display of how people don't do well at guessing probabilities. Once the problem is known, however, calculating the real odds is just a simple case of exploiting the correct mathematics.

# Probability of at least one being selected
Say we have 6 face-down cards, and 2 are known to be aces. What many people will assume from intuition is the chance of choosing at least one ace when flipping two cards over is 2 in 6 (~33%). This is only true of drawing an ace on the first attempt, however. The actual chance of picking up at least one ace is much better than that.

* * *

### Range of probabilities
Consider all possible parallel paths of outside effects : janitor who won the lottery would have had 999,999 lives with unsuccessful lottery tickets, and one possible life winning. Whereas a dentist who followed the dental-school and self-practice path has a smaller range of possibilities : ranging only from a dentist practice for poor people versus a dentist practice for rich people.

### Reference Point Argument
def - do not compute odds from the vantage point of the winning gambler, but from the bird's eye view of all those who started in the cohort.

# Normal Distribution
### Small/Large hospital example
in a town, there are 2 hospitals: 1 large and 1 small. one day, 60% of the births of one hospital were male. which hospital was it?
- intuition tells us that it was the large hospital, but statistics shows us that with larger sample sizes, we get closer to a mean (50%). therefore, it must be the smaller hospital

* * *

### Prior Probability
ex. 1% of women have breast cancer. 80% of those women received a positive mammogram. Also, 9.6% of women without breast cancer tested positive. What is the probability that any random person that tests positive will actually have breast cancer?
- most doctors when asked this question will vastly overestimate the probability, placing it at ~80%.
	- The most common mistake is to ignore the original fraction of women with breast cancer (only 1%), and the fraction of women without breast cancer who receive false positives (9.6%), and focus only on the fraction of women with breast cancer who get positive results (80% of the 1%)
		- It seems intuitive that if 80% of people with breast cancer tested positive, then the probability of a woman with a positive test actually having breast cancer is 80%.
- “The probability that a woman with a positive mammogram has breast cancer” is not at all the same thing as “the probability that a woman with breast cancer has a positive mammogram”

The Priors
- **Prior probability** - The original proportion of patients with breast cancer (1%)
- **Conditional probabilities** - probability that a patient with breast cancer gets a positive mammogram (80% of the 1%), and the chance that a patient without breast cancer gets a positive mammogram (9.6%)
- see **Round-trip Fallacy**

* * *

### Chaotic system
- Imagine we had a pseudo-random coin flipper that worked by simply reading the digits of pi. If the number was even, then it is tails. If it was odd, then it is heads. To those who don't know how the heads/tails are derived, it seems random. However in reality it is not really random at all. This is the distinction between a random system and a chaotic system.
	- the fundamental truth of a chaotic system is that if we know the inputs, we can determine the outputs. Put another way, it is completely deterministic
	- ex. physically flipping a coin is not random, but chaotic, because if we knew the initial linear and angular momentum of the coin, and amount of wind resistance, we could predict every time what the result would be.
- when you get a bunch of chaotic motions all working together, they end up producing a predictable result
	- What this implies is that the more chaotic a system is, the more predictable it is.
	- ex. consider a distribution curve metal ball tool. When we turn it upside-down and let all the balls drop, it results in an almost perfect distribution curve. The balls do not "know" where to go, but they end up that way.

# Quotes
- "any event can have an infinite amount of possible causes" - Pierre Daniel Huet

# Related
- [[Combinatorics|math.combinatorics]]