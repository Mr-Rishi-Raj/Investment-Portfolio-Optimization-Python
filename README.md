# Investment Portfolio Optimization Using Python

## Project Overview

A Python-based investment management and portfolio optimization project designed to analyze stock performance, portfolio risk and return, diversification, and optimal asset allocation.

The project uses 5 years of historical market data for five Indian stocks and applies portfolio management techniques to identify portfolios with different risk return objectives.

## Portfolio

The analysis covers:

* ITC
* L&T
* Adani Ports
* Wipro
* Indian Oil

##  Project Objectives

* Analyze historical stock performance
* Calculate CAGR and annualized volatility
* Measure risk adjusted performance using Sharpe Ratio
* Analyze correlation and covariance
* Construct diversified portfolios
* Simulate 10,000 random portfolios using Monte Carlo simulation
* Optimize portfolio weights for maximum Sharpe Ratio
* Construct a minimum-volatility portfolio
* Analyze the Efficient Frontier
* Measure individual stock risk contribution
* Perform portfolio stress testing

## 🔧 Tools & Technologies

**Python | Pandas | NumPy | Matplotlib | Seaborn | SciPy | yfinance | Jupyter Notebook**

## 📊 Methodology

### 1. Market Data

Historical stock prices were retrieved using `yfinance`.

### 2. Performance Analysis

Calculated:

* Daily returns
* Cumulative returns
* CAGR
* Annualized volatility
* Sharpe Ratio

### 3. Risk & Diversification

Used:

* Correlation matrix
* Covariance matrix
* Portfolio variance
* Portfolio volatility
* Risk contribution

### 4. Portfolio Construction

Compared four portfolio strategies:

* Equal Weight
* Monte Carlo Max Sharpe
* Optimized Max Sharpe
* Minimum Volatility

### 5. Portfolio Optimization

The Maximum Sharpe portfolio was optimized using **SLSQP**, subject to portfolio weight constraints.

### 6. Efficient Frontier

Simulated portfolios were plotted to analyze the relationship between expected return and portfolio risk.

### 7. Stress Testing

The optimized portfolio was tested under hypothetical market shocks to evaluate potential downside sensitivity.

## Key Results

| Portfolio                | Expected Return | Volatility | Sharpe Ratio |
| ------------------------ | --------------: | ---------: | -----------: |
| Equal Weight             |          14.54% |     18.22% |         0.47 |
| Monte Carlo Max Sharpe   |          21.13% |     20.40% |         0.74 |
| **Optimized Max Sharpe** |      **21.09%** | **20.24%** |     **0.75** |
| Minimum Volatility       |          10.97% | **15.81%** |         0.31 |

### Optimized Portfolio Allocation

| Stock       | Weight |
| ----------- | -----: |
| ITC         |  9.33% |
| L&T         | 45.92% |
| Adani Ports | 10.02% |
| Wipro       |  0.00% |
| Indian Oil  | 34.72% |

The optimized portfolio achieved the highest Sharpe Ratio among the strategies tested, indicating the strongest historical risk adjusted performance within the model.

## Key Visualizations

The project includes:

* Efficient Frontier
* Portfolio Allocation Comparison
* Risk Contribution Analysis
* Sharpe Ratio Comparison
* Portfolio Stress Testing
* Portfolio Performance Comparison

## Key Takeaways

The analysis demonstrates that portfolio construction is not only about selecting high-return stocks. Correlation, covariance, volatility, portfolio weights, and risk contribution can significantly influence the overall risk-return profile.

The optimized portfolio allocated a larger proportion to L&T and Indian Oil while assigning zero weight to Wipro under the optimization constraints.

## Disclaimer

This project is for educational and analytical purposes only. The analysis uses historical market data and hypothetical assumptions. Historical performance and optimized portfolio weights do not guarantee future returns.

