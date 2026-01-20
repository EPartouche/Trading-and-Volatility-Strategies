# Trading-and-Volatility-Strategies
Individual coursework project on option-based trading strategies. I independently structured and analyzed 5 option trades using directional, volatility, protection and relative value approaches. Each trade includes rationale, pricing, Greeks, implied volatility, moneyness and mark-to-market analysis, following a professional Excel framework.

You can find below the strategies choosen:

## APPLE Stocks - Strap Delta Hedged 

# Rationale
# High implied volatility scenario, with a directional bias to the upside
Main reason: Event-driven catalyst: Upcoming product launches or earnings (Apple’s earnings typically move the stock significantly).
-> Main event: 9 or 10 september 2025-> Expected launches: iPhone 17 with upgraded processor and camera, Apple Watch Series 11, Ultra 3, SE refresh, iPad Pro with M5 chip, and public release of iOS 19 (likely around September 15). 

1- High liquidity: AAPL has a deep options market with tight spreads — ideal for a straddle.
2- Market uncertainty: Mixed tech sector sentiment due to macro interest rate shifts and AI arms race.
3- Volatility divergence:  Implied volatility often underestimates realized volatility near earnings – straddles capitalize on that.
4- Clean chart structure: Technically coiled price range in past weeks – ripe for breakout in either direction.
5- Strategy Goal: Profit from significant price move in either direction, regardless of direction.

# Delta Hedging

14/04 : The net delta is –0.028, meaning the portfolio is nearly delta-neutral, with only a minimal exposure: it would lose $0.028 if Apple’s stock rises by $1. A new delta adjustement will be realised in june 2025.

Strategy1	APPLE Stocks	Strap Delta Hedged	.AAPL	14/04/2025	Spot	202,585	Strap Delta Hedged	30000	11/09/2025	-	ATM				205,86		14,02%	34,83%	10,73%	29,44%											
Leg1	AAPL	Long European Call	.AAPL	14/04/2025	Spot	202,585	Long	20000	11/09/2025	Call	100%	9,556%	7,114%	-1911,18	205,86	488,3780958	56,88%	34,83%	10,73%	29,44%	"High implied volatility scenario, with a directional bias to the upside
Main reason: Event-driven catalyst: Upcoming product launches or earnings (Apple’s earnings typically move the stock significantly).
-> Main event: 9 or 10 september 2025-> Expected launches: iPhone 17 with upgraded processor and camera, Apple Watch Series 11, Ultra 3, SE refresh, iPad Pro with M5 chip, and public release of iOS 19 (likely around September 15). 

1- High liquidity: AAPL has a deep options market with tight spreads — ideal for a straddle.
2- Market uncertainty: Mixed tech sector sentiment due to macro interest rate shifts and AI arms race.
3- Volatility divergence:  Implied volatility often underestimates realized volatility near earnings – straddles capitalize on that.
4- Clean chart structure: Technically coiled price range in past weeks – ripe for breakout in either direction.
5- Strategy Goal: Profit from significant price move in either direction, regardless of direction."										
Leg2	AAPL	Long European Put	.AAPL	14/04/2025	Spot	202,585	Long	10000	11/09/2025	Put	100%	8,11%	5,912%	-811,15	205,86	219,95	-42,86%	34,83%	10,73%	29,44%											
Delta Hedging	APPLE Stocks	Delta Hedging	.AAPL	14/04/2025	Spot	202,585	Short	4254,285	avr-25	Cash	-	-	1,62%	-	205,86	-68,775	-0,03	-	-	-	"DELTA HEDGING
14/04 : The net delta is –0.028, meaning the portfolio is nearly delta-neutral, with only a minimal exposure: it would lose $0.028 if Apple’s stock rises by $1. A new delta adjustement will be realised in june 2025."										
Leg1	AAPL	Cash	.AAPL	14/04/2025	Spot	202,585	Short	4254,285	avr-25	Cash	100%	0	1,62%	 4 254,29 	205,86	-68,775	-3%	-	-	-											
Total P&L	APPLE Stocks	Strap Delta Hedged	.AAPL	14/04/2025	-	202,585	Strap Delta Hedged		sept-25	-	-	-	-	 1 531,96   	205,86	639,5530958	-0,03	34,83%	10,73%	29,44%											
<img width="32766" height="500" alt="image" src="https://github.com/user-attachments/assets/8dd24674-c484-43fa-8a70-d02c2a01bb46" />
