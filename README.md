# Customer-Segmentation-2

# 🛍️ Customer Segmentation using K-Means Clustering

This project applies unsupervised machine learning (K-Means Clustering) to group customers based on their annual income and spending score. The goal is to uncover distinct customer segments for better marketing strategies.

---

## 📊 Dataset Overview

- **Source**: [Mall Customer Segmentation Dataset (Kaggle)](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **Rows**: 200  
- **Columns**:
  - `CustomerID`
  - `Gender`
  - `Age`
  - `Annual Income (k$)`
  - `Spending Score (1–100)`

---

## 🧼 Data Preprocessing

- Removed `CustomerID` (not relevant for clustering)  
- Encoded `Gender` using `LabelEncoder`  
- Scaled features using `StandardScaler` to normalize all numeric columns  
- Final dataset included features like `Age`, `Income`, and `Spending Score`

---

## 🤖 Model: K-Means Clustering

- Applied the **Elbow Method** to determine optimal number of clusters  
- Selected **K = 5** based on visual elbow point  
- Trained KMeans model and predicted cluster labels for each customer

---

## 📈 Cluster Interpretation

| Cluster | Segment Description              |
|---------|----------------------------------|
| 0       | Low Income, Low Spending         |
| 1       | High Income, Low Spending        |
| 2       | Medium Income, High Spending     |
| 3       | High Income, High Spending (VIP) |
| 4       | Low Income, High Spending        |

---

## 🔍 Visualization

- Scatter plot of **Annual Income vs Spending Score**, color-coded by cluster  
- Clear segmentation of 5 distinct customer groups  
- Insights can inform personalized marketing and targeting

---

## 🧠 Libraries Used

- `pandas`, `numpy`  
- `matplotlib`, `seaborn`  
- `scikit-learn`: KMeans, LabelEncoder, StandardScaler

---

## ✨ Author

**Lokesh Mandarapu** – [LinkedIn](https://linkedin.com/in/lokeshmandarapu)

---

## 🏁 Project Status

✅ Completed | 📊 Clustered | 🎯 Visualized 
