**Customer Segmentation with Clustering 🛍️**
📌 ***Project Objective***

The goal of this project is to apply unsupervised machine learning to segment mall customers into meaningful groups. By identifying distinct personas based on income, spending behavior, and other attributes, we can provide actionable insights for targeted marketing campaigns.

🔎 ***Dataset***

Source: Mall_Customers.csv 

Main Features:
  
  CustomerID (identifier, dropped)
  Gender
  Age
  Annual Income (k$)
  Spending Score (1-100)

🧪 ***Steps Performed***
1. Exploratory Data Analysis (EDA)

  Examined distributions of Age, Annual Income, and Spending Score.
  Compared Gender vs Spending Score:
    Female customers show slightly higher average spending scores.
    Distributions overlap, suggesting gender alone is not a strong predictor.

2. Feature Engineering

  Created a new feature:
  
    SpendIncomeRatio = Spending Score / Annual Income
    Purpose: normalize spending relative to income to better capture purchasing behavior.

3. Clustering

  Selected features for clustering: Annual Income, Spending Score, and SpendIncomeRatio.
  
  Applied StandardScaler to normalize data.
  
  Used the Elbow Method to determine the optimal number of clusters (k ≈ 4).
  
  Applied K-Means clustering and assigned cluster labels.

4. Cluster Visualization & Interpretation

  Visualized clusters using scatter plots (Income vs Spending, SpendIncomeRatio vs Spending).
  
  Profiles of discovered clusters:
  
  Cluster 0 – High income, low spending → wealthy but low engagement.
  
  Cluster 1 – Low income, high spending ratio → budget-conscious but strong buyers.
  
  Cluster 2 – Younger, mid income, high spending → trendy and responsive.
  
  Cluster 3 – Older, moderate income and spending → stable but less active.

📊 ***Insights***

Gender influences spending habits slightly, but not strongly enough for segmentation alone.

Engineered features such as SpendIncomeRatio reveal deeper insights that income or spending alone cannot capture.

Clustering helps identify target groups for personalized marketing strategies.

🚀 ***Key Learnings***

  Difference between supervised and unsupervised learning.
  Importance of feature engineering to uncover hidden patterns.
  Practical use of K-Means clustering and Elbow Method in customer segmentation.
