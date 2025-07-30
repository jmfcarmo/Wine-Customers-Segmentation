# Customer Segmentation for Wonderful Wines of the World 🍷

This project was developed in the context of the "Data Mining 1" course and focuses on clustering-based customer segmentation for the wine retailer **Wonderful Wines of the World (WWW)**. Using unsupervised learning techniques, the goal was to help WWW transition from mass marketing to personalized strategies by identifying distinct customer groups based on **value** and **buying behavior**.

---

## 🧠 Project Objectives

1. **Engagement & Value Segmentation**:  
   Segment customers based on engagement and value (recency, frequency, monetary, LTV, etc.) to identify loyal, high-value, and at-risk customers.

2. **Product Preference Segmentation**:  
   Identify customer segments based on wine type preferences (dry red, sweet white, dessert, etc.).

3. **Strategy Development**:  
   Combine both segmentations to create actionable marketing recommendations for each group.

---

## 📊 Dataset Overview

We worked with a dataset of **10,000 active customers**, including demographic, behavioral, and transactional variables:

| Variable | Description |
|----------|-------------|
| `AGE`, `INCOME`, `EDUCATION` | Demographics |
| `RECENCY`, `FREQ`, `MONETARY` | RFM values |
| `LTV` | Lifetime value |
| `PERDEAL` | Discount sensitivity |
| `WEBPURCH`, `WEBVISIT` | Digital behavior |
| `DRYRED`, `SWEETRED`, `DRYWH`, etc. | Wine type preferences |
| `ACCESS` | Wine accessory purchases |

---

## ⚙️ Methodology

### 1. Data Cleaning & Preprocessing
- Handled missing values and outliers
- Normalized variables using Min-Max scaling
- Selected relevant features per segmentation objective

### 2. Clustering Algorithms Used
- **K-Means Clustering**
- **Hierarchical Clustering**
- **DBSCAN** (tested but not selected in final solution)

### 3. Evaluation & Validation
- Chose optimal number of clusters using Elbow Method, Silhouette Score, and Dendrograms
- Visualized clusters using PCA and t-SNE projections

---

## 🔍 Key Insights

### Engagement & Value Segmentation:
- Identified 4 distinct groups:  
  - **High Value, High Engagement**
  - **New but Promising**
  - **Loyal but Low-Spending**
  - **At-Risk / Dormant**

### Buying Behavior Segmentation:
- Segmented customers into wine preference profiles:  
  - **Red Wine Lovers**  
  - **Sweet Wine Fans**  
  - **Experimental / Exotic Tastes**  
  - **Balanced Mix Consumers**

### Combined Strategy Matrix:
Mapped behavior segments with value segments to design targeted marketing actions, such as:
- **Upselling premium products to high-value red wine lovers**
- **Retention campaigns for at-risk dessert wine fans**
- **Cross-sell accessories to digital-savvy mixed consumers**

---

## 📦 Tools & Libraries

- Python 3.10
- Google Colab
- pandas, numpy
- matplotlib, seaborn, plotly
- scikit-learn (KMeans, DBSCAN, PCA, etc.)
- scipy (for hierarchical clustering)
- seaborn, plotly for visualizations

---
