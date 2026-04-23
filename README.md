
# Fashion Retail Analytics: Data-Driven Decision Support for SMEs

This project shows how small and medium-sized European fashion retailers can leverage existing multi-table transactional data to generate actionable business insights without relying on complex AI or large historical datasets. Using real e-commerce data spanning sales, customers, products, campaigns, and inventory, the analysis delivers practical tools for customer retention, inventory planning, and marketing optimization through interpretable machine learning.

## Approach & Methodology

The solution integrates seven relational tables into task-specific analytical views. Core techniques include RFM (Recency, Frequency, Monetary) analysis, K-Means clustering, and classical supervised learning (Logistic Regression, Linear Regression). All models priorities easiness of use and operational utility over algorithmic complexity, to ensure non-technical teams can understand and act on results. Feature engineering transforms raw transactions into behavioral signals for forecasting and segmentation.

## Dataset Overview

The dataset comprises seven relational tables representing a realistic European fashion e-commerce operation over three months (April–June 2025). It includes over 1,000 rows per table across sales, customers, products, campaigns, channels, stock, and sales items. It Covers transactional, demographic, product, promotional, and inventory dynamics with no missing values or duplicates.

## Key Insights

- **Customer Segmentation**: Identified high-value “Champion” customers (Cluster 2) using RFM + K-Means (silhouette score = 0.44), to enable targeted retention.
- **Churn Risk**: Detected 57 at-risk customers (9.8% of base), concentrated in Germany and France, many with high past spend.
- **Campaign Impact**: Marketing efforts showed **30% lower daily revenue** during campaigns (*p* = 0.978), suggesting unsegmented discounts attract low-value buyers and erode margins.
- **Inventory Gaps**: Flagged 7 best-selling SKUs (e.g., Elegant Cotton Dress) as critically understocked (<5 units despite >23 sales)—urgent restock priorities.
- **Forecasting**: Simple linear models outperform complex alternatives in interpretability while delivering operationally useful MAE (<€97 for sale value, <3 units for demand).

## Future Work

Future improvements include expanding the data horizon beyond three months to improve CLV and churn model reliability. It will incorporate unstructured feedback (reviews, returns) to capture sentiment-driven volatility, and testing SMOTE or cost-sensitive learning to boost recall on rare high-value churn events. A weekly automated dashboard will provide restock alerts, churn flags, and campaign anomaly detection.
