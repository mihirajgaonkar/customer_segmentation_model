# Online Retail Data Clustering

## Overview

This project aims to cluster online retail customer data to identify meaningful customer segments. By using clustering algorithms, the analysis provides insights into customer behavior patterns, which can be leveraged for targeted marketing strategies, personalized promotions, and improved customer retention. The dataset comprises transactions from an e-commerce retailer, making it an ideal case for customer segmentation.

## Table of Contents

- [Overview](#overview)
- [Technical Details](#technical-details)
- [Results & Conclusion](#results--conclusion)


## Technical Details

The project uses machine learning techniques for clustering, focusing on the following steps:

1. **Data Preprocessing:**
   - Cleaning data (handling missing values, removing duplicates).
   - Dealing with outliers using statistical methods.
   - Transforming data into a usable format.

2. **Feature Engineering:**
   - Creation of RFM (Recency, Frequency, Monetary) features to quantify customer interactions.
   - Scaling of data for effective clustering.

3. **Clustering:**
   - Implemented K-Means clustering to segment customers based on RFM values.
   - Evaluation of clusters using metrics like:
     - **Silhouette Score**
     - **Within-Cluster Sum of Squares (WCSS)**
     - Elbow Plot for optimal cluster selection.

4. **Visualization:**
   - Visualized the clusters and RFM distribution using Matplotlib and Seaborn.
   - Used PCA for dimensionality reduction to understand cluster separation.

The analysis is implemented in a Jupyter Notebook using Python libraries such as:
- **Pandas**: Data manipulation and analysis
- **Scikit-learn**: Clustering and evaluation
- **Matplotlib & Seaborn**: Data visualization

## Results & Conclusion

The clustering analysis identified multiple customer segments, providing clear insights into different types of buyers and their corresponding behaviors. Each cluster is defined based on RFM attributes, along with tailored strategies for effective engagement:

1. **Cluster 0 (Blue): "Retain"**
   - **Rationale:** This cluster represents high-value customers who purchase regularly, though not always very recently.
   - **Action:** Focus on retention efforts with loyalty programs, personalized offers, and regular engagement to maintain their loyalty and spending levels.

2. **Cluster 1 (Orange): "Re-Engage"**
   - **Rationale:** This group includes lower-value, infrequent buyers who haven’t purchased recently.
   - **Action:** Use targeted marketing campaigns, special discounts, or reminders to encourage them to return and purchase again.

3. **Cluster 2 (Green): "Nurture"**
   - **Rationale:** These are the least active and lowest-value customers but have made recent purchases.
   - **Action:** Focus on relationship building, excellent customer service, and offering incentives to increase their engagement and spending.

4. **Cluster 3 (Red): "Reward"**
   - **Rationale:** This cluster includes high-value, frequent buyers who are still actively purchasing.
   - **Action:** Implement a robust loyalty program, provide exclusive offers, and recognize their loyalty to maintain their engagement.

5. **Cluster -1 (Monetary Outliers): "Pamper"**
   - **Rationale:** High spenders with large but infrequent purchases.
   - **Action:** Focus on personalized offers or luxury services to maintain their loyalty and cater to their high spending capacity.

6. **Cluster -2 (Frequency Outliers): "Upsell"**
   - **Rationale:** Frequent buyers with lower spending per purchase.
   - **Action:** Implement loyalty programs or bundle deals to encourage higher spending per visit, leveraging their frequent engagement.

7. **Cluster -3 (Monetary & Frequency Outliers): "Delight"**
   - **Rationale:** The most valuable outliers with extreme spending and frequent purchases.
   - **Action:** Develop VIP programs or exclusive offers to maintain loyalty and encourage continued engagement.

### Summary of Cluster Names:

- **Cluster 0 (Blue): "Retain"**
- **Cluster 1 (Orange): "Re-Engage"**
- **Cluster 2 (Green): "Nurture"**
- **Cluster 3 (Red): "Reward"**
- **Cluster -1 (Monetary Outliers): "Pamper"**
- **Cluster -2 (Frequency Outliers): "Upsell"**
- **Cluster -3 (Monetary & Frequency Outliers): "Delight"**

The segmentation offers a comprehensive view of customer groups, allowing for tailored marketing strategies and focused engagement efforts.
