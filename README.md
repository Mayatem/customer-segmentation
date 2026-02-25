# Customer Segmentation Using PCA and K-Means

## 📊 Project Overview

This project analyzes customer credit card transaction data to identify distinct customer segments based on spending and payment behavior.

To reduce dimensionality and improve clustering performance, Principal Component Analysis (PCA) was applied before performing K-Means clustering. The goal was to uncover meaningful behavioral groups while preserving most of the dataset’s variance.

## 🎯 Business Objective

Financial institutions and marketing teams can use customer segmentation to:
 -  Identify high-value customers
 -  Detect low-engagement users
 -  Personalize marketing strategies
 
  Optimize credit and retention strategies
This project demonstrates how dimensionality reduction and clustering techniques can simplify large financial datasets and reveal actionable customer insights.

## 📁 Dataset

Dataset: Customer Credit Card Data (public dataset)
Features include:
- Balance
- Credit Limit
- Purchases
- Payments
- One-Off Purchases
- Purchases_TRX
The dataset was cleaned by removing missing values and zero-value records before analysis.

## ⚙️ Methodology

1️⃣ Data Preprocessing
  - Removed missing and zero-value entries
 -  Selected key financial features
  - Performed exploratory data analysis (pair plots, correlations)

2️⃣ Dimensionality Reduction (PCA)
  - Applied Principal Component Analysis
 - First four components explained ~93% of total variance
  - Reduced dataset complexity while preserving key information
  - Generated Scree Plot and cumulative variance summary

3️⃣ Clustering (K-Means)
  - Used PCA-transformed dataset
  - Evaluated optimal cluster size using:
    - Elbow Method
    - Silhouette Score
 -  Selected k = 3 for better business interpretability

4️⃣ Cluster Interpretation
Generated:
  - PCA scatter plot with centroids
  - Cluster summary tables
 -  Heatmap of average feature values
  - Final pair plot visualization

## 📈 Key Results

Three distinct customer segments were identified:
🔵 Cluster 0 – Moderate Activity Customers
 -  Moderate balances
 -  Controlled spending behavior
 -  Regular but manageable purchases

🟠 Cluster 1 – Low Activity Customers
  - Low balances
  - Low purchase activity
  - Limited credit usage

🟢 Cluster 2 – High-Value Customers
 - High balances
  - High credit limits
- Large purchase and payment amounts
  - Active, high-spending segment
    
PCA successfully reduced complexity while preserving meaningful behavioral patterns for clustering.

## 🛠 Tools & Technologies
  - PowerBI
  - Python
  - Pandas
 -  NumPy
  - Scikit-learn
  - Seaborn
 -  Matplotlib
  - PCA
  - K-Means Clustering

## 📊 Visualizations
- Pair Plot
- PCA Scree Plot
- K-Means Clustering on PCA Space
- Elbow & Silhouette Analysis
- Cluster Heatmap

🚀 Key Takeaways
- PCA can significantly reduce dataset dimensionality while preserving over 90% of variance.
- Combining PCA with K-Means improves clustering clarity.
- Cluster interpretability is critical for business applications.
- Statistical optimality (k=2) may differ from business practicality (k=3).
