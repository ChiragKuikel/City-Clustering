# City-Clustering
## Overview
This project analyzes global cost of living indices to uncover key drivers influencing living expenses in different cities and countries.
Using correlation analysis, linear regression, and K-Means clustering, the project identifies patterns, relationships, and cost-based groupings of cities across the world.
A Power BI dashboard and visual maps provide an interactive summary of findings.

## Dataset
Source: https://www.kaggle.com/datasets/debdutta/cost-of-living-index-by-country
Description: The dataset includes indices such as:

Cost of Living Index

Rent Index

Groceries Index

Restaurant Price Index

Local Purchasing Power Index

## Project Woekflow
### 1. Exploratory Data Analysis (EDA)

Performed initial exploration of data (shape, missing values, distributions).

Identified key variables impacting cost of living.

### 2. Correlation and Regression Analysis

Conducted correlation analysis to find initial relationships between variables.

Performed linear regression to validate causation, since correlation alone does not guarantee it.

Finding:

Groceries Index strongly impacts Cost of Living Index.

Rent Index showed high correlation but negligible causal impact, which was a surprising insight.

### 3. Visualization of Relationships

Used pairplots to visualize correlations and feature distributions across cities.

Highlighted notable cities:

Mumbai – Low cost of living, high purchasing power.

Hamilton – High cost of living and expensive lifestyle.

Reykjavik (Iceland) – Expensive but lower income levels.

Kathmandu (Nepal) – Added for local relevance.

### 4. Data Normalization

Normalized all features using StandardScaler to prepare for clustering.

### 5. Optimal Clusters Determination

Used Inertia Plot (Elbow Method) and Silhouette Scores to determine the optimal number of clusters (found to be 3).

### 6. K-Means Clustering

Applied K-Means algorithm to group cities into 3 clusters based on cost-related indices.

Detected that Purchasing Power Index was inversely correlated, so it was inverted before final clustering for consistency.

### 7. Cluster Visualization

Created scatter plots to visualize clusters.

Plotted world maps to display geographical clustering results.

Designed an interactive Power BI dashboard summarizing the analysis and insights.

## Key Insights:
Groceries Index emerged as the strongest contributor to cost of living.

Rent Index, despite strong correlation, had little actual causal impact.

Cities with lower living costs don’t necessarily have low purchasing power.

Clustering provided meaningful segmentation of cities into affordable, mid-range, and expensive living groups.

## Tools and technologies
Languages: Python

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

Visualization: Power BI, matplotlib, seaborn

Clustering Algorithm: K-Means

Normalization: StandardScaler

## Skills Demonstrated
Exploratory Data Analysis (EDA)

Correlation vs. Causation interpretation

Feature engineering and normalization

K-Means clustering and evaluation

Visualization and storytelling using data

Power BI dashboard creation
