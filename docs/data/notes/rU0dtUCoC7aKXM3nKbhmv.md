
if you want to know what people typically pay for something, google the median, not the mean or average. The median cost of a wedding, for example, is $14k, but the average cost is $30k. Medians tell you what most people typically pay, averages are often skewed towards the higher end (and, more importantly, are not the data you're looking for).

### Geometric average (Gavg)
- Derived from multiplying all numbers together, then taking the *nth* root (ex. if 2 numbers, square root— if 3 numbers, cube root)
	- ex. `Gavg (2, 8) = 4`
    ![](/assets/images/2021-03-27-20-55-22.png)
- geometric mean is often used when comparing different items
	- the fact that each item has different properties and different numeric ranges renders the Gavg useful
	- ex. what if we want to compare 2 companies by 2 properties each: their environmental sustainability (rated from 0-5), and their financial viability (rated from 0-100). If we used the arithmetic average (Aavg) to compute result, it wouldn't be too meaningful. Financial viability would have higher weight by virtue of it's higher range. Instead, we use the Gavg, which causes an equal ∆% in either property to have the same impact. In other words, ↑20% of environmental sustainability (from 4 -> 4.8) would have the same impact as ↑20% of financial viability (from 60 -> 72).
- geometric mean applies only to positive numbers.
- often used for a set of numbers whose values are meant to be multiplied together or are exponential in nature
	- ex. population growth, interest rate of investment
- When looking at average growth rate, Gavg is better than Aavg
	- ex. if we start with $100, and that amount increases by 80% in year 1 (now $180) and 25% in year 2 (now $225), it is more appropriate to take a geometric average of that number, which would be 50%. In other words, the difference between our initial $100 and final $225 would be 50% per year (meaning the average growth rate is 50%).

#### When to use Gavg
**Proportional growth (inc. exponential)**

*P-Hacking* - misuse of data analysis to find patterns and correlations that would seem to imply a truth.
- ex. there is a correlation between the average length of winning spelling bee word and deaths by venomous snakes per year 

