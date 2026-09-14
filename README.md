# Academic-Asset-Pricing-Automated-Quantitative-Investing

A quantitative finance project that connects academic asset pricing models
with practical data analysis, systematic investment research, and automated
investment applications.

The project begins with a multi-frequency evaluation framework for classical
asset pricing models and will gradually expand toward portfolio construction,
backtesting, and automated quantitative investment strategies.

---

## Project 1: Real-Time Asset Pricing Monitor

The first project develops a framework for estimating and evaluating major
asset pricing models across different data frequencies.

### Models

The initial framework includes:

- Capital Asset Pricing Model (CAPM)
- Fama-French 3-Factor Model (FF3)
- Carhart 4-Factor Model (FF4)
- Fama-French 5-Factor Model (FF5)

The general factor model can be written as:

$$
R_{i,t} - R_{f,t}
=
\alpha_i
+
\boldsymbol{\beta}_i^{\prime}\mathbf{F}_t
+
\epsilon_{i,t}
$$

where:

- $R_{i,t}$: return of asset $i$
- $R_{f,t}$: risk-free rate
- $\mathbf{F}_t$: vector of systematic risk factors
- $\alpha_i$: abnormal return unexplained by the factor model
- $\boldsymbol{\beta}_i$: factor exposures

---

## Multi-Frequency Analysis

The long-run objective is to evaluate asset pricing models at multiple
investment horizons:

- Daily
- Hourly
- Minute
- Second

This allows the project to investigate how factor exposures and model
performance change as the investment horizon becomes shorter.

---

## Initial MVP

The first working version will focus on daily data.

### Phase 1

- [ ] Build market data collection pipeline
- [ ] Calculate asset returns
- [ ] Implement CAPM
- [ ] Implement Fama-French 3-Factor Model
- [ ] Implement Carhart 4-Factor Model
- [ ] Implement Fama-French 5-Factor Model
- [ ] Estimate rolling factor exposures
- [ ] Compare model performance

### Phase 2

Extend the framework to:

- [ ] Hourly data
- [ ] Minute-level data
- [ ] Second-level data
- [ ] Intraday factor construction
- [ ] Real-time model monitoring

---

## Model Evaluation

Models will be compared using measures such as:

- Alpha
- Alpha t-statistic
- Factor betas
- R-squared
- Adjusted R-squared
- RMSE
- MAE
- Rolling parameter stability

A major research question is:

> How does the explanatory power of traditional asset pricing models change
> across different investment horizons?

---

## Planned Repository Structure

```text
Academic-Asset-Pricing-Automated-Quantitative-Investing/

├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── capm/
│   ├── ff3/
│   ├── ff4/
│   └── ff5/
│
├── src/
│   ├── data/
│   ├── factors/
│   ├── models/
│   ├── evaluation/
│   └── visualization/
│
├── results/
│   ├── tables/
│   └── figures/
│
├── README.md
└── requirements.txt
