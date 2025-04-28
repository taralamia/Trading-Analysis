# Trading-Analysis-Project
This project was completed as part of a technical interview assignment for NEXT Venture.
The goal was to analyze a trading dataset, evaluate trader profitability, build a predictive model to classify profitable traders, and perform trader segmentation through clustering techniques.
## Overview
This project analyzes a trading dataset related to gold trading (symbol: XAUUSD). It aims to explore data integrity, evaluate trader profitability, engineer predictive features, build a predictive model, and segment traders based on their performance.
The analysis focuses on:
- Profitability analysis of traders
- Key factors influencing profits
- Predictive modeling to classify profitable traders
- Clustering traders based on their performance
## Dataset Description
- Rows: 60,000 trading records
- Columns: 14 attributes including open_price, close_price, pips, volume, profit, etc.
## Key Analysis and Result
1. Profitability Analysis
   - Top Performers: Identified traders with highest cumulative profits.
   - Worst Performers: Identified traders with highest cumulative losses.
2. Key Factors Influencing Profitability
   - Strongest Positive Correlation: pips with profit.
   - Trade Type Insight: "Buy" trades are generally more profitable than "Sell" trades.
   - Symbol Contribution: Certain symbols (e.g., XAUUSD, EURUSD) contribute significantly to profits.  
3. Feature Engineering & Predictive Modeling:
- Engineered Features: profitability_flag, win_rate, avg_profit, avg_loss, extreme_loss_flag, trade_frequency, volume_weighted_profit.
- Predictive Model: Logistic Regression, 5-Fold Cross-Validation with accuracy 65.6%.
- Model Validation: 61.02% alignment accuracy between predicted flags and actual cumulative profits.
4. Clustering & Trader Segmentation:
- Method: K-Means Clustering (k=3)
- Clusters:
  - Cluster 0: Losers (Negative cumulative profits)
  - Cluster 1: Neutral Traders (Near-zero cumulative profits)
  - Cluster 2: Profitable Traders (High cumulative profits)
## Technologies Used
- Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- Machine Learning (Logistic Regression, K-Means Clustering)
- Data Visualization (Boxplots, Histograms, Heatmaps)
