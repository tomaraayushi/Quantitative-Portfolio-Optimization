# Quantitative Portfolio Optimization

A comprehensive implementation of Modern Portfolio Theory using Python to optimize risk-adjusted returns for technology stock portfolios.

## 📊 Project Overview

This project demonstrates end-to-end portfolio optimization by analyzing 8 major technology stocks and finding the optimal allocation that maximizes the Sharpe ratio. The analysis combines statistical modeling, risk assessment, and mathematical optimization to create superior risk-adjusted portfolios.

## 🎯 Investment Objective

**Goal**: Maximize risk-adjusted returns (Sharpe ratio) for a technology-focused equity portfolio while maintaining reasonable diversification and risk controls.

**Universe**: Large-cap technology stocks (FAANG+ companies)
**Benchmark**: Equal-weighted portfolio
**Risk Controls**: Maximum 50% allocation per stock, long-only positions

## 🛠️ Technical Implementation

### **Phase 1: Data Collection & Preprocessing**
- Historical price data retrieval via Yahoo Finance API
- Data cleaning and return calculation
- Missing data handling and outlier detection

### **Phase 2: Risk-Return Analysis**
- **Statistical Metrics**: Mean returns, volatility
- **Performance Metrics**: Sharpe ratios
- **Distribution Analysis**: Return distribution characteristics

### **Phase 3: Portfolio Optimization**
- **Objective Function**: Maximize Sharpe ratio = (μₚ - rₑ) / σₚ
- **Constraints**: 
  - Weights sum to 1 (fully invested)
  - Maximum 50% allocation per asset
- **Method**: Sequential Least Squares Programming (SLSQP)
- **Risk Model**: Full covariance matrix with correlation effects

