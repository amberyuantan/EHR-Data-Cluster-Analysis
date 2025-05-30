# EHR-Data-Cluster-Analysis
# Cluster Analysis of Electronic Health Records (EHR)

## Overview

This project uses unsupervised learning to analyze ICU patient data from Electronic Health Records (EHR). By applying **PCA** for dimensionality reduction and **K-Means clustering**, the goal is to identify patient subgroups with different levels of mortality risk.

## Methods

- **Data Cleaning**: Removed invalid or missing entries, encoded categorical variables.
- **Feature Scaling**: Standardized numeric features with Z-score normalization.
- **PCA**: Reduced to 2 components (PC1 + PC2 explain 27.2% variance).
- **K-Means**: Optimal number of clusters determined as **3** using Elbow and Silhouette methods.
- **Evaluation**:
  - Silhouette Score: **0.611**
  - Chi-square p-value: **0.01752**

## Results

| Cluster | Patients | Mortality Rate |
|---------|----------|----------------|
| 1       | 157      | 1.91%          |
| 2       | 660      | 3.64%          |
| 3       | 565      | 6.37%          |

- Cluster 1: Low-risk  
- Cluster 2: Intermediate-risk  
- Cluster 3: High-risk  
