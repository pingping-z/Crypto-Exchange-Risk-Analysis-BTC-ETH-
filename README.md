# Crypto-Exchange-Risk-Analysis-BTC-ETH-
Overview
This project implements an exchange-style crypto risk analysis pipeline using recent market data to evaluate downside risk, tail behavior, and model performance under high-volatility regimes.
Using BTC and ETH daily data from a centralized exchange, the project focuses on rolling Value-at-Risk (VaR) backtesting, stress-window analysis, and portfolio drawdowns, aiming to assess whether traditional risk metrics systematically underestimate tail risk in crypto markets.


Data
Source: OKX public OHLCV API
Assets: BTC, ETH
Frequency: Daily
Sample Period: April 2025 – Present
The analysis intentionally focuses on recent market regimes, reflecting real-world exchange risk monitoring rather than long-horizon historical crises.

Methodology
1. Return & Volatility Analysis
Computed daily returns for BTC and ETH
Examined volatility clustering and fat-tailed return distributions
2. Risk Metrics
Historical VaR and CVaR (95%, 99%)
Parametric VaR (normal assumption) for comparison
3. Rolling VaR Backtesting
120-day rolling historical VaR
One-day-ahead VaR forecasts (no look-ahead bias)
Evaluated VaR breach frequency vs. theoretical expectations
4. Stress-Window Analysis
Identified recent extreme-loss days directly from the data
Analyzed worst-day loss, cumulative loss, and maximum drawdown within a stress window
5. Portfolio Risk
Constructed a BTC/ETH 60/40 portfolio
Evaluated drawdowns and VaR breaches under stress
Analyzed correlation-driven loss amplification

Key Findings
In a recent stress window (2026-01-25 to 2026-02-14), a BTC/ETH 60/40 portfolio experienced a worst-day loss of 8.94% and a maximum drawdown of 28.80%, highlighting severe downside concentration during market stress.
Rolling 95% historical VaR backtesting (120-day window) shows a breach rate of 8.43%, significantly higher than the theoretical 5%, indicating systematic tail-risk underestimation during high-volatility regimes.
During stress periods, BTC and ETH exhibit elevated downside correlation, reducing diversification benefits and amplifying portfolio drawdowns.


