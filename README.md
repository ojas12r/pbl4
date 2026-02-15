# pbl4
Market Regime Detection using Hidden Markov Models
Overview

Financial markets are non-stationary and alternate between different regimes such as:

 Bull Markets

 Bear Markets

 High Volatility Periods

 Low Volatility Periods

Traditional trading strategies assume constant market behavior, which leads to poor performance during regime shifts.

This project uses a 3-State Gaussian Hidden Markov Model (HMM) to detect hidden market regimes and enhance a Simple Moving Average (SMA) trading strategy using regime-based filtering.

Objective

Detect hidden market regimes using probabilistic modeling

Validate volatility clustering hypothesis

Improve SMA crossover strategy

Reduce drawdowns and false signals

Perform out-of-sample validation

Returns=log(Pt​/Pt−1​)


Model Configuration

3-State Gaussian HMM

Full Covariance Matrix

Maximum Likelihood Estimation

n_iter = 1000

StandardScaler normalization

Hidden States → Market Regimes
Observations → Returns + Volatility

Trading Strategy
Base Strategy — SMA Crossover

10-day SMA > 30-day SMA → BUY

10-day SMA < 30-day SMA → EXIT

Weakness:

Whipsaws during volatile regimes

High drawdowns
References

QuantStart — Market Regime Detection using HMM in QSTrader

hmmlearn Documentation

Statistical Learning Theory
Author

Ojas Raghav
Project-Based Learning (PBL)
2026
