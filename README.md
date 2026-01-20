# Trading-and-Volatility-Strategies
Individual coursework project on option-based trading strategies. I independently structured and analyzed 5 option trades using directional, volatility, protection and relative value approaches. Each trade includes rationale, pricing, Greeks, implied volatility, moneyness and mark-to-market analysis, following a professional Excel framework.

The result with explanation appear on the Excel Document attached.

You can find below the strategies choosen:

## APPLE Stocks - Strap Delta Hedged - Maturity : 11/09/2025

### Rationale
### High implied volatility scenario, with a directional bias to the upside
Main reason: Event-driven catalyst: Upcoming product launches or earnings (Apple’s earnings typically move the stock significantly).
-> Main event: 9 or 10 september 2025-> Expected launches: iPhone 17 with upgraded processor and camera, Apple Watch Series 11, Ultra 3, SE refresh, iPad Pro with M5 chip, and public release of iOS 19 (likely around September 15). 

1- High liquidity: AAPL has a deep options market with tight spreads — ideal for a straddle.
2- Market uncertainty: Mixed tech sector sentiment due to macro interest rate shifts and AI arms race.
3- Volatility divergence:  Implied volatility often underestimates realized volatility near earnings – straddles capitalize on that.
4- Clean chart structure: Technically coiled price range in past weeks – ripe for breakout in either direction.
5- Strategy Goal: Profit from significant price move in either direction, regardless of direction.

### Delta Hedging

14/04 : The net delta is –0.028, meaning the portfolio is nearly delta-neutral, with only a minimal exposure: it would lose $0.028 if Apple’s stock rises by $1. A new delta adjustement will be realised in june 2025.

## TESLA Stocks - Strangle - Maturity : 26/06/2025

### Rationale
### High implied volatility scenario,  benefit from large directional move (up or down), with a lower premium than straddle
Main reason: Elon Musk-driven volatility: TSLA often experiences sharp, unpredictable movements from tweets, product announcements, or regulatory news.
-> Main event: end of june 2025-> Tesla's most significant upcoming event is the launch of its robotaxi service in Austin, Texas.

1- Wide expected move: Strangle benefits from large moves, and TSLA is inherently volatile.
2- Option pricing asymmetry: OTM options may offer a cheaper vol exposure than ATM straddles.
3- Implied volatility skew opportunities: Slight differences in vol between calls and puts may improve cost efficiency.
4- Macro pressure on entreprise value sector: Interest rates + Chinese competition = potential downside shock.
5- Liquidity and gamma responsiveness: Tesla options are highly liquid, allowing for efficient entry, exit, and potential gamma scalping around the event. The high liquidity of TSLA options enables active management (e.g., adjusting delta hedges or monetizing gamma spikes), which is crucial in a volatile name ahead of a binary event like the robotaxi launch.

## Exxon Mobil Corp. Stocks - Bull Call Spread - Maturity : 24/07/2025

### Rationale
### Moderate bullish scenario with controlled risk, benefiting from a moderate rise in XOM’s stock price while limiting premium outlay compared to naked calls
Main reason: Oil price rebound and economic recovery potential driving demand for energy majors.
-> Main events: late July 2025 (Q2 earnings), OPEC+ supply decisions, and monthly EIA reports impacting crude prices.

1- Moderate expected upside: Bull Call Spread profits from a steady rise in XOM fueled by improving oil fundamentals.
2- Capital efficiency: Spread limits premium cost versus buying calls outright in an elevated implied volatility environment.
3- Risk management: Defined maximum loss and capped gains ideal for a moderately bullish view.
4- Macro factors: OPEC+ production cuts, geopolitical tensions, and demand resurgence support oil prices but pose risks for volatility.
5- Seasonal and historical patterns: Summer driving season historically supports oil demand and XOM performance, aligning well with a mid-2025 bullish thesis. U.S. gasoline consumption typically peaks in Q2–Q3, providing a seasonal tailwind for ExxonMobil’s refining and upstream margins, enhancing the probability of a moderate stock price rise within the spread’s strike range.

## Microsoft Corporation - Butterfly (with calls) - Maturity : 24/07/2025

### Rationale
### Neutral to slightly bullish scenario with limited risk, aiming to profit from MSFT’s price stability around a target level while minimizing premium outlay compared to buying calls outright
Main reason: Market expects consolidation after recent strong growth, with steady fundamentals supporting the stock.
-> Main events: late July 2025 (Q2 earnings), Microsoft Build conference (May-June), and ongoing innovation announcements in cloud and AI sectors.

1- Range-bound opportunity: The Long Butterfly capitalizes on MSFT’s price staying within a tight band, maximizing profit if the stock remains near the middle strike.
2- Cost-efficient construction: Selling 2 calls at the center strike helps finance the structure, resulting in a low net premium (~0.7% of spot), much cheaper than buying a call alone.
3- Neutral delta profile: The strategy’s delta is approximately flat (+1 Δ₍360₎ –2 Δ₍380₎ +1 Δ₍400₎ ≈ +0.01), minimizing unwanted directional exposure.
4- Balanced volatility: Implied volatility (~30% for 90-day options) is close to historical average, keeping option pricing fair and the structure cost-effective.
5- Cost-effective positioning: By selling calls at the center strike, this strategy lowers the overall premium paid compared to buying calls alone, making it more affordable in current volatility conditions.
6- Defined risk profile: Both maximum loss and potential gains are capped, providing clear risk parameters suitable for traders expecting limited directional moves.
7- Sector stability with catalysts: While the tech sector shows steady growth, upcoming product launches and earnings announcements could trigger short-term volatility that the butterfly can navigate effectively.

## AUD/JPY - Call Spread (with carry and directional strategy) - Maturity : 25/07/2025

### Rationale
### Moderately bullish on AUD/JPY, driven by diverging monetary policy and risk sentiment recovery in Asia-Pacific. The goal is to benefit from a gradual appreciation of the AUD against the JPY while keeping downside risk defined and premium low
Main reason: The Bank of Japan maintains ultra-loose monetary policy, while the Reserve Bank of Australia remains relatively hawkish due to sticky inflation and resilient economic data.
-> Main events: late July 2025 (Q2 earnings), BoJ Policy Meeting – June 14, 2025: potential continuation of dovish stance, RBA Meeting – June 4, 2025: possible tightening due to inflation, Chinese data releases – June–July 2025: trade-linked AUD impact, global risk appetite shifts: AUD benefits from improved sentiment.  The most accurate maturity for this AUD/JPY long call spread strategy is July 25, 2025, as it captures key upcoming events like the RBA meeting (June 4), BoJ policy decision (June 14), and relevant Chinese economic data through June–July, allowing enough time for the trade thesis to play out before expiry.

1- Monetary policy divergence: RBA’s higher rates vs BoJ’s yield curve control favors AUD strength.
2- Carry advantage: Long AUD/JPY benefits from positive carry due to rate differentials (+3% to +4% annualized).
3- Directional upside potential: JPY remains weak on structural grounds, and AUD could rise toward key resistance zones.
4- Defined risk-reward: The long call spread caps both potential loss and gain, suitable for a controlled bullish view.
5- Low volatility cost structure: Implied vol (~9–10%) is relatively low for this FX pair, making spreads attractive.
6- Event alignment: Major central bank meetings and macro releases within maturity window may trigger movement into profit zone.


# Coding analysis

## First Event - Apple Strap Hedging
Python code used to analyse Apple stock by computing daily log returns, realised volatility (daily, period and annualised) and total return over a defined time window. The analysis provides a quantitative measure of risk and performance, useful for comparing realised volatility with option-implied volatility and assessing directional versus volatility-driven strategies.

[*********************100%***********************]  1 of 1 completedDaily volatility (σ):            2.1466%
Volatility over period:          10.7328%
Annualised volatility (σ·√252):  34.0755%
Total return over the period:    2.28%

<img width="1863" height="1254" alt="image" src="https://github.com/user-attachments/assets/d4542714-80be-425c-8ab2-94dacda44751" />

<img width="968" height="650" alt="image" src="https://github.com/user-attachments/assets/bf839cd0-c8a2-403a-8d8f-5bfc425970c2" />
<img width="912" height="648" alt="image" src="https://github.com/user-attachments/assets/f9b201fb-e5cc-46b6-a1a6-6e3ee01dc3e1" />

Estimated number of option contracts:  1.48
Total delta exposure from options:     20.76 shares
To delta hedge, you should short:      21 shares of the stock

## FX analysis - AUD/JPY Call Spread (with carry and directional strategy)
Python code used to analyse the AUD/JPY exchange rate by computing daily log returns, realised volatility (daily, period and annualised) and total return over a defined horizon. This analysis quantifies FX risk and performance, enabling comparison with option-implied volatility and supporting directional, carry or volatility-based FX option strategies.

[*********************100%***********************]  1 of 1 completedDaily volatility (σ):            0.6575%
Volatility over period:          3.2212%
Annualised volatility (σ·√252):  10.4379%
Total return over the period:    3.37%

Secondly, the AUD/JPY exchange rate analysis by computing daily log returns and a 10-day rolling annualised volatility. The exchange rate and realised volatility are plotted together to visualise the relationship between price movements and changing FX risk over time, supporting volatility-based and option trading analysis.

<img width="1847" height="897" alt="image" src="https://github.com/user-attachments/assets/3405b2c1-c103-404d-87b1-ca0c9bff892c" />

## Phenix analysis - Global view on 21/05/2025
Analysis providing a clear overview of risk and performance across multiple equities (AAPL, TSLA, MSFT, XOM) by estimating daily log returns, realised volatility at different horizons, and total returns over the same period. This allows direct comparison of market behaviour across stocks and supports relative value and option strategy assessment.

[*********************100%***********************]  1 of 1 completed
[*********************100%***********************]  1 of 1 completed
[*********************100%***********************]  1 of 1 completed
[*********************100%***********************]  1 of 1 completed--- AAPL ---
Daily volatility (σ):            2.1466%
Volatility over period:          10.7328%
Annualised volatility (σ·√252):  34.0755%
Total return over the period:    2.28%

--- TSLA ---
Daily volatility (σ):            3.6823%
Volatility over period:          18.4117%
Annualised volatility (σ·√252):  58.4553%
Total return over the period:    36.25%

--- MSFT ---
Daily volatility (σ):            2.0438%
Volatility over period:          10.2192%
Annualised volatility (σ·√252):  32.4449%
Total return over the period:    18.36%

--- XOM ---
Daily volatility (σ):            1.4288%
Volatility over period:          7.1438%
Annualised volatility (σ·√252):  22.6810%
Total return over the period:    2.44%

Overview comparing four equities (AAPL, TSLA, MSFT, XOM) over the same time window by plotting both their closing prices and their 10-day rolling annualised realised volatility was done. This dual-axis visual highlights how price trends and risk evolve together across stocks, enabling quick cross-name comparison for relative value and option/volatility strategy selection.

****<img width="1646" height="823" alt="image" src="https://github.com/user-attachments/assets/77f44de0-361b-448e-812a-acd4244961e7" />

