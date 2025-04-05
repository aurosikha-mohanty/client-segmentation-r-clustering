# Client Segmentation & Strategic Insights for Company XYZ
Client segmentation and strategic insights using K-Means clustering for a wholesale distributor in Portugal.

## Project Overview
Company XYZ, a wholesale distributor based in Portugal, aims to optimize its inventory management and tailor its marketing strategies by understanding spending behavior across its 440 business clients. This project applies clustering techniques to identify distinct client segments and extract actionable insights for improving demand forecasting and client retention.

## Objectives
- Identify spending patterns across six product categories: Fresh, Milk, Grocery, Frozen, Detergents_Paper, and Delicatessen.
- Segment clients into meaningful groups using K-Means clustering and silhouette analysis.
- Provide strategic recommendations tailored to each segment’s behavior and needs.

##  Methodology
1. **Data Preprocessing**
   - Handled missing values (none found).
   - Detected and removed outliers using IQR-based logic.
   - Standardized features for clustering using Z-score scaling.

2. **Outlier Strategy**
   - Outliers were grouped into a separate cluster named **"Elite Spenders"** to preserve main client structure.

3. **Clustering Approach**
   - Performed K-Means clustering with `k=2` and `k=3` for comparison.
   - Evaluated cluster validity using **silhouette coefficients**.
   - Conducted **hierarchical clustering** for cross-validation.

4. **Segmentation Result**
   - Final segmentation includes **4 clusters**, integrating 3 main K-Means clusters and the outlier group.

##  Cluster Profiles
1. **Elite Spenders**
   - High-value clients with consistent large orders in Fresh, Milk, Frozen, and Grocery.
   - Found primarily among Horeca in Oporto and Retailers in other regions.

2. **Perishable Heavy**
   - Strong demand for Fresh and Frozen products.
   - Horeca in Lisbon and hotels show peak interest in perishable goods.

3. **Essential Stockers**
   - Retailers focusing on bulk orders of Milk, Grocery, and Detergents.
   - Higher demand in Lisbon and Oporto regions.

4. **Value Seekers**
   - Low to mid-level spenders, often boutique or small-scale clients.
   - Price-sensitive and responsive to value bundles.

##  Strategic Recommendations
| Cluster            | Strategy Highlights |
|--------------------|---------------------|
| **Elite Spenders** | Premium bundles, loyalty programs, volume discounts, flexible delivery. |
| **Perishable Heavy** | Subscription models, margin increase on perishables, targeted offerings. |
| **Essential Stockers** | Cross-sell Fresh & Milk with essentials, tiered pricing, fast delivery. |
| **Value Seekers** | Smaller frequent bundles, pricing incentives, retention via smart offers. |

