# Markowitz Mean-Variance Optimization

### Overview

This project provides a robust framework for constructing optimal investment portfolios using Modern Portfolio Theory (MPT).

### Dataset

The project uses stock return data structured in CSV files with:

- stock_data2.csv	(Bank, Energy, Telecom stocks)
- stock_data3.csv	(Tech, Retail, Energy stocks)	
- stock_data_strong.csv	(Historically strong performers)	
- stock_data_weak.csv	(Historically volatile assets)	

### Dataset Limitations

1. Small Time Span:
- Some files cover only 2007-2008 (financial crisis period).
- Impact: Extreme volatility skews optimization.

2. Concentrated Sectors:
- stock_data2.csv is banking-heavy → Poor diversification.

3. Collinearity:
- Energy stocks (e.g., Chesapeake, GE) move together → Redundant in portfolios.

### Key Findings

Both the minimum volatility and maximum Sharpe ratio portfolios converged to nearly identical allocations, suggesting:

- Low return dispersion in the input data (assets behaved too similarly).
- Insufficient risk premiums (no asset offered significantly better risk-adjusted returns).

### Current and Future Use

1. Current Data Works For:
- Academic experiments with Markowitz theory.
- Testing basic diversification effects.

2. For Real-World Use:
- Expand to longer timeframes and more assets.
- Include uncorrelated asset classes (REITs, commodities).

### Source

[Stock Portfolio Optimization Dataset for Efficient from Kaggle](https://www.kaggle.com/datasets/chibss/stock-dataset-for-portfolio-optimization)
