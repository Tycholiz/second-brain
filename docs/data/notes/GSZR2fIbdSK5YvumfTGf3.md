
The idea is that if you take some set of number data and chop off all numbers after the first one, you will have a predictable distribution of numbers
- ex. take a large list of airline prices over the course of a year.

![](/assets/images/2021-04-11-20-47-22.png)

What this curve shows is that ~30% of the numbers will start with a `1`, ~17% with a `2`, and so on.

#### Use in discovery of Enron fraud
In an analysis of Enron, it was found that the numbers they reported did not follow the expected curve.

#### Social Media Bots
If you analyze friend count among users, you will see a distribution that follows Benford's Law
- ex. I have 233 friends (2), you have 125 (1), and so on... the observations will follow Benford's Law distribution.

This fact has been used to uncover bots who do not have natural friend counts.

#### Elections
Interestingly, an election where people vote their conscience results in a curve that follows the distribution pattern. However, elections add a degree of complexity, in that humans will vote for someone who is not their first choice if they think that candidate will lose. This disturbs the resulting curve, and as a result will be a curve that is a skewed version of a expected curve.
