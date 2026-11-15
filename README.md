# Quantitative Portfolio Risk & Performance Tracker

A Python-based financial data analysis tool that fetches historical market data, calculates key performance metrics (Cumulative Return, Volatility, Moving Averages), and evaluates multi-asset portfolio risk efficiency using the Sharpe Ratio and Covariance Matrices.

---

## Features

- Automated Data Pipeline: Downloads historical equity data directly from Yahoo Finance (`yfinance`).
- Trend Analysis: Calculates daily returns and tracks market trends using a 20-Day Simple Moving Average (SMA).
- Risk & Volatility Analysis: Computes annualized volatility and variance for single stocks and multi-asset portfolios.
- Sharpe Ratio Evaluation: Measures risk-adjusted returns to determine asset efficiency against market volatility.
- Portfolio Diversification: Constructs an annualized Covariance Matrix to model multi-stock interaction and compute portfolio-level return and risk.
- Data Visualization: Generates performance charts using `matplotlib`.

---

## Tech Stack & Libraries

- Language: Python 3.x
- Data Manipulation: `pandas`, `numpy`
- Data Ingestion: `yfinance`
- Visualization: `matplotlib`

---

## Financial Methodology & Formulas

### 1. Cumulative Return
$$\text{Cumulative Return} = \frac{P_{\text{final}} - P_{\text{initial}}}{P_{\text{initial}}} \times 100$$

### 2. Portfolio Annualized Volatility ($\sigma_p$)
$$\sigma_p = \sqrt{w^T \Sigma w}$$
*Where $w$ is the vector of asset weights and $\Sigma$ is the annualized covariance matrix.*

### 3. Annualized Sharpe Ratio
$$\text{Sharpe Ratio} = \frac{E(R_p) - R_f}{\sigma_p}$$
*(Assuming Risk-Free Rate $R_f = 0\%$ for baseline equity comparisons).*

---

## Getting Started

### Prerequisites
Ensure Python is installed along with the required libraries:

```bash
pip install yfinance pandas numpy matplotlib
