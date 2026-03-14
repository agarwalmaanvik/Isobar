# Isobar Weather Risk Backtest Results

This document summarizes the backtest results for the Isobar Weather Risk Engine across three primary risk categories: **Heatwave (Call Options)**, **Monsoon (Deficit Protection)**, and **Cold Snap (Put Options)**.

## 1. Heatwave Risk Backtest (Heat Index)
**Scenario**: Extreme summer heat across major Indian metros and arid regions.
**Contract**: 30-Day Limit, Payout INR 1000/tick (Degree Day), Cap INR 50k.

| City | Strike | Prob. of Payout | Insurer Price (CVaR) |
| :--- | :--- | :--- | :--- |
| **Delhi** | 45C | 25.8% | INR 23,838 |
| **Mumbai** | 45C | 22.9% | INR 17,331 |
| **Chennai** | 45C | 26.7% | INR 25,815 |
| **Bangalore** | 42C | 32.5% | INR 28,468 |
| **Ahmedabad**| 45C | 35.9% | INR 48,847 |
| **Nagpur** | 45C | 32.5% | INR 43,486 |
| **Jaisalmer**| 45C | 21.7% | INR 40,521 |
| **Churu** | 45C | 20.9% | INR 40,257 |

## 2. Monsoon Deficit Backtest (Rainfall)
**Scenario**: Rainfall deficit protection during peak monsoon months.
**Contract**: 30-Day Limit, Payout INR 500/mm Deficit, Cap INR 1 Lakh.

| City | Strike Rain | Prob. of Payout | Insurer Price (CVaR) |
| :--- | :--- | :--- | :--- |
| **Mumbai** | 200 mm | 35.5% | INR 51,885 |
| **Mumbai** | 300 mm | 82.0% | INR 97,497 |
| **Chennai** | (NE Mon) | *Calibrated* | *Simulated* |

## 3. Cold Snap Backtest (Winter Temp)
**Scenario**: Winter frost and cold wave protection for agriculture/energy.
**Contract**: 30-Day Limit, Payout INR 1000/tick (Degree Day), Cap INR 50k.

| City | Strike | Prob. of Payout | Insurer Price (CVaR) |
| :--- | :--- | :--- | :--- |
| **Delhi** | 6 C | 54.9% | INR 50,000 |
| **Delhi** | 4 C | 39.9% | INR 50,000 |
| **Amritsar** | (Winter) | *Calibrated* | *Simulated* |

---
*Note: Prices represent the Risk-Adjusted CVaR (Conditional Value at Risk) at the 95th percentile to ensure solvency during extreme tail sessions.*
