# Sequential Bayesian Trading Strategy Simulator

## Overview
This project investigates how traders can evaluate and manage trading strategies with uncertain edge using Bayesian learning and sequential decision-making.

The simulation models:
- Bayesian belief updating
- Sequential stopping rules
- Edge detection thresholds
- Monte Carlo simulation of trading outcomes

## Progress

1. Analysis of Sharpe Heatmap of Fixed Sizing Strategy under Varying Parameters
2. Investigation of Detection Times and Rates of Fixed Sizing Strategy
3. Comparison of Sharpe under Fractional Kelly Sizing and Fixed Sizing Strategies

---

## Key Questions
- How quickly can we detect a profitable trading strategy?
- How does edge strength affect detection speed?
- What is the trade-off between early stopping and long-run profitability?

---

## Methodology
- Simulated coin-flip trading environment with unknown edge
- Bayesian updating over discrete probability hypotheses
- Sequential decision rules:
  - Stop if high probability of bad edge
  - Trade with variable size depending on confidence (Fixed vs Kelly)
- Parameter sweeps over stopping and detection thresholds

---

## Results

### 1. Weak edges require large sample sizes
Weak edges are difficult to distinguish from noise and require many trades before confidence emerges.

### 2. Stronger edges improve detection and Sharpe
Higher edge leads to faster detection and better risk-adjusted performance.

### 3. Trade-off between Type I and Type II errors
Stopping rules must balance:
- Exiting profitable strategies too early
- Staying too long in unprofitable ones

---

### 1. Sharpe Heatmap with Varying Threshold Parameters

### Sharpe Heatmap (true_p = 0.55)
![Sharpe heatmap](figures/sharpe_heatmap_p_0.55.png)

### Sharpe Heatmap (true_p = 0.60)
![Sharpe heatmap](figures/sharpe_heatmap_p_0.60.png)

### Sharpe Heatmap (true_p = 0.65)
![Sharpe heatmap](figures/sharpe_heatmap_p_0.65.png)

### 2. Investigation of Detection Times and Rates of Fixed Sizing Strategy

### Detection Time vs True Edge
![Detection time plot](figures/detection_time_vs_true_p.png)

### Detection Rate vs True Edge
![Detection rate plot](figures/detection_rate_vs_true_p.png)

### 3. Comparison of Sharpe under Fractional Kelly Sizing and Fixed Sizing Strategies

---



---

## Key Insight

---

## Tech Stack
- Python
- NumPy
- Pandas
- Matplotlib / Seaborn

---
