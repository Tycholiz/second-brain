
# Overview
Options derive their value from the fact that no one knows where the stock price is going to be in X amount of days. All we know is that it won’t be where it currently is. This is of the option however the resulting prices of these options is considered the aggregate beliefs on where a stock will be in any amount of given time

An option is a [[finance.securities.derivative]] because its price is intrinsically linked to the price of something else

options premiums are a function of two main ingredients:
1. value of the option (profit gained by executing option)
2. time value

↑option value as ↑interest rate
- And when you sell an option, profit is capped at the price of the premium, but the downside potential is unlimited.

With options, a strategy can be employed to profit off literally any type of market condition (bear, bull, sideways)

As an option buyer, your objective should be to purchase options with the longest possible expiration, in order to give your trade time to work out
- And when you are writing options, go for the shortest possible expiration in order to limit your liability.

The main draw of options is one of leverage
- ex. given a simple situation where an investor has $1000 to burn and is bullish on a stock; a simple 14% upward movement in the price of a stock could result in a CALL return of 150% (Just to demonstrate how far apart these percentages are)
	- It's true that buying a CALL and buying a stock both have capped downsides, but if in both situations we are spending $1000, the option route is more like "the downside is 100%", whereas just buying a stock, it's unlikely the stock goes to 0.
	- In reality, since you don't have to own an option until expiry, you can sell before losing all your money

Typically, an options contract loses approximately one-third of its time value during the first half of its life.
- Time value decreases at an accelerating pace and eventually reaches zero as the option's expiration date draws near.
A common mistake option investors make is allowing a profitable trade to sit long enough that theta reduces the profits substantially.
- For example, a trader may buy an option for $1, and see it increase to $5. Of the $5 premium, only $4 is intrinsic value. If the stock price doesn't move any further, the premium of the option will slowly degrade to $4 at expiry

# Terminology
### Open Interest (OI)
Gives a sense of the liquidity of an option
- is not simply a count of all the available buy and sell contracts
- instead, intended to provide a more accurate picture of trading activity surrounding options, and the ∆money flow in and out of options

When a buyer and seller make a contract, the contract is considered "open" and, will only close upon execution, expiration, or manual closing out of the option.
- If there were low open interest, it would be more difficult to get option orders filled at a good price
- one must also examine whether the open interest is in calls or puts and whether the contracts are being bought or sold.
- "Volume" refers to the number of contracts traded in a given period, and is distinct from OI

#### Interpretations
- ↑Prices & ↑Trend & ↑OI - can mean that new money is coming into the market (reflecting new positions; a bullish sign)
- ↑OI ↓StrikePrice - a sign of a downward trend of the underlying stock.
	- might suggest that new money is coming into the market on the short side
- ↓Prices & ↓Trend & ↑OI - This scenario is consistent with a continuing downtrend and is bearish.
- ↓Prices & ↓Trend & ↓OI - could indicate that holders are being forced to liquidate their positions (bearish).
	- could mean that a selling climax could be on the near-term horizon.
- ↑OI & ↓Prices (sharply decreasing) - could be a bearish signal if holders who bought near the top are now losing money;
	- this also could potentially cause an environment of panic selling.

### Implied Volatility (IV)
- volatility increases the premium of an option.
	- This makes sense, since options have limits (floors/ceilings). a CALL holder is not going to care if he is on the wrong end of high volatility any more than if he is at the wrong end of low volatility (since he only loses the premium). However, if he is on the right side of the volatility, then high/low matters, since there is no limit on the upside.
	- This is why options become expensive before earnings reports
- as people gain interest and expecatations for an option, the implied volatility rises
	- therefore, volatility is directly influenced by supply and demand
- the longer the remaining time period, the more IV will matter
	- Options with strike prices that are near the money are most sensitive to implied volatility changes, while options that are further in the money or out of the money will be less sensitive to implied volatility changes
- IV is not the same as historical volatility
- Implied volatility usually increases in bearish markets and decreases when the market is bullish

### Intrinsic value
- the difference between the stock price, and the strike price
	- in other words, it's what you would get when factoring in the price you can excercise at, and the price of the option itself
	- therefore, intrinsic value=0 unless the stock price moves beyond the strike price
- to calculate how much of an option's premium is due to intrinsic value, an investor would subtract the strike price from the current stock price.
	- if the option premium is primarily made up intrinsic value, the option's value and profitability are more dependent on movements in the underlying stock price.
- time value is the portion of the premium above the intrinsic value that an option buyer pays for the privilege of owning the contract for a certain period.
	- therefore, time value is often referred to as extrinsic value.

### Delta
- a measure of an option's sensitivity to the underlying stock
	- ex. Delta=0.6 means a $1 increase in the stock price will result in a $0.60 increase in the option price
- The delta for puts is represented as a negative number, which demonstrates the inverse relationship of the put compared to the stock movement.
	- ex. A put with a delta of -0.4 should increase by 40 cents in value if the stock drops $1 per share.
- An in-the-money option has higher delta

### Buy to open
- the act a open a new option
- if you were bullish on a stock, you would buy to open a call
- if you were bearing on a stock, you would buy to open a put

### Sell to close
- the act a holder takes to exit his position in the option
- if you were no longer bullish on a stock, you would sell to close a call
- if you were no longer bearish on a stock, you would sell to close a put

# Being a Writer (seller of options)
- writers are obligated to buy/sell if the option expires in the money
- Your odds of profit are higher (than if you were a buyer), even though the risk is technically unlimited

# Being a Holder (buyer of options)
- When you buy an option, loss is capped at the price of the premium, but the upside potential is unlimited.
option price decays over time
"time value of money always settles at zero"
when buying a call, you should always ask, how will this option overcome the decay inherent in aging options?

# Call
the right to buy stock at a given price
- As ↑StockPrice, ↑OptionPrice
	- Though as time goes on, the stock price must rise enough to offset time decay
- ↑premium, as:
	1. stock price rises more and more above strike price
	2. time to expiration is longer
	3. volatility is higher
- The more volatile a stock, the more valuable the call option, since losses are already minimized and gains have no limit.
- Think of a call option as a down-payment for a future purchase. You could also see it as a deposit, in the sense that you can walk away from it and just be limited to losing your deposit.
	- ex. A potential homeowner sees a new development going up. That person may want the right to purchase a home in the future, but will only want to exercise that right once certain developments around the area are built.
		- In the real estate world, this would be known as a deposit (`premium` in options). In the stock world it is a `call`

## Buying
- Buying call options are total-loss investments, because unless the strike price is reached, the loss will be 100%
- Can be a strategy for hedging a short position

## Selling
- Selling a naked (ie. uncovered) call gives you a potential short position in the underlying stock.

# Put
the right to sell the stock at a given price
- ↑premium, as:
	1. stock price falls more and more below strike price
	2. time to expiration is longer
	3. volatility is higher

## Buying
- Gives you a potential (and less risky) short position in the underlying stock.
- Can be a strategy for hedging a long position

## Selling
- Selling a naked, or unmarried, put gives you a potential long position in the underlying stock
- if slightly bullish, you can write near-term puts to capture premium income

# Relationships
- The more likely something is to occur, the more expensive an option would be that profits from that event
	- ex. as a stock price rises further, the more expensive that CALL will cost.
- The less time there is until expiry, the less value an option will have
	- This is because as we get closer and closer to expiry, the probability that the stock will move drastically in price get smaller and smaller (ie. it is a *wasting asset*)
	- ex. if you bought a 1-month option that is out-of-the-money and the stock is stagnant, the option devalues each passing day, because the odds that it eventually becomes in-the-money decreases with each passing day.
	- This shows that you can think of an option in terms of "as long as this event (strike price) occurs within my time period, I'm good"
	- If the stock is worth exactly the same the next day, the option will still be worse less, because of time decay.
- volatility of the stock increases price of an option, since volatility increases the odds of a certain outcome

# Strategies
- use options to hedge against a declining market to limit downside losses
	- think of a put option as an insurance policy. If you wanted something akin to insurance on a stock that you bought, you could buy a PUT option
	- ex. I buy a stock at $100, and am unwilling to lose more than 10%. I buy a PUT with strike price of $90, allowing me sell that stock at $90 anytime within the next 2 years. Now if in 6 months the market drops 20%, I have effectively gained a 10% return, as I can sell a stock with a prevailing price of $80 at $90
		- a short seller would buy CALL options to limit their exposure
- can be used for speculative purposes such as wagering on the direction of a stock.
	- buying a call option on the stock
	- buying a call option instead of just buying the stock may be attractive, since options provide leverage

### Spread
- buying more than 1 contract at different strike prices
	- ie. buying an option(s) to sell another option(s)
	- all options should have same expiry
- spreading will offset the premium paid
	- ie. the premium *earned* from selling an option will offset the premium *paid*
- potential profit/loss are capped
- can be employed to capitalize on any price movement
- like regular options, you can be a buyer or seller of a spread strategy

#### Bull Call Spread
- buy 1+ call at one strike price, while simultaneously selling same number of calls at higher strike price
- often used when you are bullish on the underlying stock, and expect a moderate rise in its price.
	- If you are expecting a large gain, then you'd be limiting your upside which would be a bad idea.
- This strategy limits upside gain, while reducing premium you have to spend
![](/assets/images/2021-03-30-22-50-46.png)

#### Bear Put Spread
- buy 1+ PUT at one strike price, while simultaneously selling same number of PUTs at lower strike price.
- used in opposite way of the bull call spread— you are moderately bearish on the stock, and want to limit your gain/loss
![](/assets/images/2021-03-30-22-51-03.png)

### Protective Put
- buy a put with a strike price below the current price, and simultaneously own the stock.
- purpose is to hedge (ie. insure) a long-term investment (ie. create a floor of loss)
- if ↓investment, put can be exercized to recover some of the loss
- Therefore, this strategy is good on a long-term play, where you might be anticipating some loss (think `PRPL` stock)
- If however the investment is a success, then your profit must factor in the cost of that PUT.
- The only disadvantage of this strategy is that if the stock does not fall in value, the investor loses the amount of the premium paid for the put option.
- known as *Married Put* when the coverage from the put is equal to the amount of long stock
- P&L graph looks similar to a long call’s P&L graph
![](/assets/images/2021-03-30-22-51-17.png)

### Covered Call
- buy a stock, while simultanously selling a call
	- therefore, a type of **buy-write** transaction
	- The investor will sell the same amount of options as shares that he owns, so that when/if the holder of the call comes knocking, the investor will already own the stock that he needs to sell to the holder of the call.
- the "cover" is the stock that investor owns, since they can use it to cover the cost of having to provide the owner of the call with the stock, should they choose to execute the option.
	- Whereas if the writer of the call didn't actually own the stock, they would have to go on the open market and buy the stock, then sell it to the holder of the call for the strike price. Since the situation of them exercising the option would occur when the strike price is below the current price, this investor would lose a potentially unlimited amount of money. In a Covered Call situation, since we own the stock, we don't need to worry about this. We just have to be ready to sell our stock for the price that we agree we'd sell it at to them (strike)
- purpose is to limit both losses and gains, while giving a higher probability of *some* gain.
- losses are limited at the price of the stock, minus the income earned from the sale of the call.
- gains are capped at the strike price
- ideal for an investor who believes the underlying price will not move much over the near-term, while simultaneously believing in the long-term worth of the stock.
	- ex. perhaps banking stocks following Covid— since their prices dropped significantly, but the long-term integrity of the banks is not really hindered.
- alternatively, you might use this strategy when you have a short-term position in the stock and a neutral opinion on its direction
![](/assets/images/2021-03-30-22-51-33.png)

### Straddle
- buy a CALL and buy a PUT at same strike price and same expiration date
- profit happens when the stock price rises/falls *in excess* of both option premiums paid
	- ex. if stock is at $100 and we buy a CALL and PUT at strike=$80, and both options cost a total of $10, then we will realize profit when the stock price is either below $70 or above $90
- an investor will employ this strategy when they are expecting movement out of a specific range, but aren't sure on direction of movement.
	- Therefore, there are 2 breakeven points
	- In this sense, the aim is the inverse of a **covered call**
- loss is limited at the price of the premiums
![](/assets/images/2021-03-30-22-51-46.png)

### Strangle
- similar to a Straddle, except the CALL and PUT have different strike prices
- on long strangles, the (out-of-the-money) call's strike price will be higher than the stock price, and the put's strike price will be lower than the stock price
- riskier than a straddle, since the stock will have to make a bigger movement to make profit
	- reflected by the the lower price compared to a straddle
![](/assets/images/2021-03-30-22-51-56.png)

### Protective Collar
- buy an out-of-the-money PUT (the floor) and simultaneously write an out-of-the-money CALL (the ceiling) (same expiration)
- strategy is employed after an investor has experienced substantial gains from a long position and wants to have downside protection.
- the trade-off is that they may be obligated to sell shares at a higher price, thereby forgoing the possibility for further profits.
- ex. bought SHOP at $1000, and it rose to $1500. The investor decides he is happy with those gains, so buys a $1600 PUT and sells a $1400 CALL.
- vs. Stop Loss
	- pro
		- stop loss is triggered when price hits $1500, whereas the collar just becomes in-the-money, so there is no obligation to sell
		- protects against the risk of slippage
	- con: limits upside

# Misc
- On most U.S. exchanges, a stock option contract is the option to buy or sell 100 shares; that's why you must multiply the contract premium by 100 to get the total amount you’ll have to spend to buy the call.
- The majority of the time, holders choose to take their profits by trading out (closing out) their position. This means that option holders sell their options in the market, and writers buy their positions back to close. Only about 10% of options are exercised, 60% are traded (closed) out, and 30% expire worthlessly.
