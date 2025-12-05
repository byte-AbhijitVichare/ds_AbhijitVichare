Trader Behavior vs Market Sentiment Analysis  
Candidate: Abhijit Vichare  
Assignment: Web3 Trading Team – Data Science Internship  

This project analyzes the relationship between trader activity on Hyperliquid and overall crypto market sentiment using the Fear & Greed Index. It includes data cleaning, EDA, predictive modeling, and trader clustering.


Project Structure
ds_AbhijitVichare/
│
├── notebook_1.ipynb # Data Cleaning + EDA
├── notebook_2.ipynb # Modeling + Clustering
│
├── csv_files/
│ ├── historical_trader_data.csv
│ ├── fear_greed_index.csv
│ └── daily_trade_sentiment.csv # Processed dataset from Notebook 1
│
├── outputs/
│ └── notebook_1.output
│     └──├── daily_closedpnl.png
│        ├── pnl_by_sentiment.png
│        └── volume_by_sentiment.png
├── notebook_2.output
│     └──├── confusion_matrix.png
│        ├── roc_curve.png
│        ├── feature_importances.png
│        ├── cluster_counts.png
│        └── cluster_pca2d.png
│
├── ds_report_full.pdf # Final Report
└── README.md # Project Documentation


Google Colab Notebooks

| Notebook | Purpose | Link |
|---------|----------|------|
| Notebook 1 | Data loading, cleaning, preprocessing, merging, EDA | https://colab.research.google.com/drive/1i0caa4Vm55FaZ5kuYxVFzM3tLfarEVTp?usp=sharing|
| Notebook 2 | Feature engineering, sentiment modeling, clustering |https://colab.research.google.com/drive/1mKo0FpF2a87vClsEsN-gLnDvEbmux1ou?usp=sharing|


Project Overview

This assignment explores:

1. Market Sentiment (Fear, Greed, Neutral, Extreme values)
- Loaded from Fear & Greed Index dataset  
- Merged with trader activity by date

2. Trader Behavior
- Volume (USD)  
- Token size  
- Closed PnL  
- Fees  
- Trading frequency  
- Active days  

3. EDA Visualizations
- Daily PnL over time  
- PnL distribution by sentiment  
- Trading volume vs sentiment  
- Outlier detection  

4. Predictive Modeling
- Predict next-day sentiment using RandomForest  
- Lag features and volatility  
- Model evaluation with:
  - Confusion Matrix  
  - ROC Curve  
  - Feature importance  

5. Trader Segmentation (Clustering)
- KMeans clustering of accounts  
- PCA visualization  
- Interpretation of cluster behavior  


Key Insights

- Trader volume increases significantly during **Neutral** and **Greed** phases.
- Highest PnL spikes occur during **Fear**, contradicting typical expectations.
- RandomForest model struggled due to **dataset imbalance** and **limited predictive signal**.
- Clustering revealed distinct trader profiles, even with small samples.

How To Run

1. Open both notebooks in Google Colab.  
2. Upload the CSV files inside `/csv_files`.  
3. Run **notebook_1.ipynb** first to generate processed data.  
4. Run **notebook_2.ipynb** for modeling and clustering.  
5. Outputs will be saved automatically into the `/outputs` folder.

Final Report

The full detailed analysis is available in:

ds_report_full.pdf

