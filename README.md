# Crypto Clustering

## Overview

This project applies unsupervised machine learning techniques to analyze cryptocurrency market behavior. Using historical market data, we cluster cryptocurrencies based on their 24-hour and 7-day price change percentages to identify similar movement patterns.

---

## Key Steps

- Scaled the data using `StandardScaler`
- Used the **elbow method** to find the optimal number of clusters (k = 4)
- Applied **K-means clustering** on the scaled data
- Visualized clusters using scatter plots with `hvPlot`
- Reduced dimensions using **PCA** (3 components, ~89.5% explained variance)
- Re-ran K-means clustering on the PCA-reduced data
- Compared elbow curves and cluster results between original and PCA data

---

## Files

- `Crypto_Clustering.ipynb`: Main notebook with full analysis
- `Resources/crypto_market_data.csv`: Input data file

---

## Conclusion

Both the original and PCA-reduced data produced consistent clustering results (k = 4). PCA simplified the data while retaining ~89.5% of the variance, demonstrating its usefulness for dimensionality reduction without major performance loss.
