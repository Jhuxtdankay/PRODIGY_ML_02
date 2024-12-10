# Customer Segmentation Using K-Means Clustering

## Project Overview

This project applies the **K-Means Clustering Algorithm** to segment customers of a retail store based on their purchasing behavior. The goal is to identify customer groups with similar spending patterns and provide actionable insights for targeted marketing strategies.

---

## Table of Contents
1. [Dataset](#dataset)
2. [Objective](#objective)
3. [Methodology](#methodology)
4. [Implementation Details](#implementation-details)
5. [Results](#results)

---

## Dataset
- **Source**: [Kaggle: Mall Customer Segmentation Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python).
- **Features**:
  - `Age`: Age of the customer.
  - `Annual Income (k$)`: Annual income of the customer in thousands.
  - `Spending Score (1-100)`: A score assigned based on spending patterns.
  - `Gender`: Gender of the customer.

---

## Objective
- Segment customers into distinct groups using **unsupervised learning**.
- Provide actionable insights to optimize marketing campaigns.

---

## Methodology

1. **Data Understanding and EDA**:
   - Examined data distribution and identified trends.
   - Checked for missing values and visualized correlations.

2. **Data Preparation**:
   - Handled missing values and detected outliers.
   - Scaled numerical features using **MinMaxScaler**.

3. **Model Building**:
   - Determined the optimal number of clusters using:
     - Elbow Method.
     - Silhouette Score.
   - Implemented the **K-Means algorithm** with `k-means++` initialization.

4. **Model Optimization**:
   - Compared K-Means with PCA-optimized clustering.
   - Experimented with alternate methods (e.g., K-Medoids).

5. **Post-Processing and Interpretation**:
   - Visualized clusters using scatter plots and heatmaps.
   - Analyzed and summarized the characteristics of each cluster.

---

## Implementation Details

### Libraries Used:
- **Data Analysis and Preprocessing**: `pandas`, `numpy`, `scikit-learn`
- **Visualization**: `matplotlib`, `seaborn`

### Key Functions:
- **Optimal Cluster Detection**: Combined Elbow Method and Silhouette Analysis.
- **K-Means Clustering**: `KMeans` from `scikit-learn`.
- **PCA for Dimensionality Reduction**: `PCA` from `scikit-learn`.

---

## Results

- **Optimal Clusters**: The analysis determined 6 clusters as optimal.
- **Performance Metrics**:
  - Silhouette Score (K-Means): **0.429**
  - Cluster Inertia: **8.406**
- **Cluster Insights**:
  - Grouped customers based on **age**, **income**, and **spending patterns**.
  - Identified potential target groups for high-spending customers.

---
