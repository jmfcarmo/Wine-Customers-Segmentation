# Customer Segmentation for Wonderful Wines of the World 🍷

This project was developed in the context of an academic course and focuses on clustering-based customer segmentation for the wine retailer **Wonderful Wines of the World (WWW)**. Using unsupervised learning techniques, the goal was to help WWW transition from mass marketing to personalized strategies by identifying distinct customer groups based on **value** and **buying behavior**.

---

## 🧠 Project Objectives

1. **Engagement & Value Segmentation**  
   Identify distinct groups of customers based on their purchasing frequency, recency, monetary value, and lifetime value. The goal is to highlight loyal customers, high-spenders, and at-risk clients.

2. **Product Preference Segmentation**  
   Analyze customer preferences based on wine types (e.g., dry red, sweet white, dessert wines) to uncover behavioral clusters related to taste and buying patterns.

3. **Strategic Alignment**  
   Combine the two segmentations to create a practical framework for **targeted marketing strategies**, cross-selling, and loyalty programs.

---

## 📊 Dataset Summary

The dataset includes **10,000 active customers** who made at least one purchase in the last 18 months. Each customer is described by demographic, behavioral, and transactional variables:

| Type         | Variables Included                                                   |
|--------------|-----------------------------------------------------------------------|
| Demographics | `AGE`, `EDUCATION`, `INCOME`, `KIDHOME`, `TEENHOME`                  |
| Engagement   | `RECENCY`, `FREQ`, `MONETARY`, `LTV`, `DAYSWUS`                      |
| Discounts    | `PERDEAL`                                                             |
| Channels     | `WEBPURCH`, `WEBVISIT`, `ACCESS`                                     |
| Preferences  | `% of wine types purchased: DRYRED, SWEETRED, DRYWH, SWEETWH, etc.`  |

---

## ⚙️ Methodology

### 🧼 Preprocessing
- Outlier detection and removal
- Imputation of missing values
- Feature selection tailored to each segmentation goal
- Normalization using Min-Max scaling

### 📈 Clustering Techniques
- **K-Means Clustering**
- **Agglomerative Hierarchical Clustering**

> We also tested DBSCAN, but it was not selected due to poor cluster definition on this dataset.

### 🔍 Model Evaluation
- Elbow Method  
- Silhouette Score  
- Dendrogram inspection (for hierarchical clustering)  
- Dimensionality reduction with PCA for visualization

---

## 🔍 Key Insights

### 1. Engagement & Value Clustering
Segmented the customer base into groups such as:
- **High Value Loyalists**: Frequent, high spenders with recent activity  
- **Dormant Clients**: Long inactive, low frequency  
- **Newcomers**: Recent activity but lower spending  
- **Discount Seekers**: High % of purchases on deals

### 2. Wine Preference Clustering
Found consistent consumer types:
- **Red Wine Enthusiasts**  
- **Sweet Wine Lovers**  
- **Experimental Tasters**  
- **Balanced Drinkers**

### 3. Combined Customer Matrix
By cross-referencing both segmentations, we proposed **customized marketing plans**:
- Upselling accessories to digital-savvy red wine fans  
- Loyalty incentives for high-value sweet wine buyers  
- Reactivation campaigns for dormant but once-profitable customers
---

## 📦 Tools & Libraries

- Google Colab
- pandas, numpy, matplotlib, seaborn
- scikit-learn (`KMeans`, `AgglomerativeClustering`, `PCA`, `MinMaxScaler`)
- scipy (`linkage`, `dendrogram`)
- plotly for interactive visualizations
---
