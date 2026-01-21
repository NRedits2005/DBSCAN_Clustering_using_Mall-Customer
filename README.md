# DBSCAN_Clustering_using_Mall-Customer
## 📌 Project Overview
This project applies **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** to perform **customer segmentation** on the Mall Customers dataset. Unlike K-Means or Hierarchical clustering, DBSCAN can identify **arbitrarily shaped clusters** and **outliers (noise points)**, making it effective for real-world data analysis.

---

## 📂 Dataset Description
- **Dataset Name:** Mall_Customers.csv  
- **Each Row Represents:** A single customer  
- **Key Features Used:**
  - Annual Income (k$)
  - Spending Score (1–100)

The following columns are excluded:
- CustomerID
- Age
- Genre (encoded but not used for clustering)

---

## ⚙️ Tools & Libraries Used
- **Python**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Matplotlib**
- **Seaborn**

---

## 🔄 Data Preprocessing
- Checked for missing values
- Encoded categorical feature **Genre** using Label Encoding
- Selected numerical features relevant for clustering
- Prepared clean input data for DBSCAN

---

## 🧠 DBSCAN Algorithm Details
- **Algorithm:** DBSCAN
- **Distance Metric:** Euclidean
- **Key Parameters:**
  - `eps` – Maximum distance between two points to be considered neighbors
  - `min_samples` – Minimum points required to form a dense region

DBSCAN automatically:
- Detects the number of clusters
- Identifies **outliers** (label = -1)

---

## 🔁 Parameter Exploration
A looping mechanism is implemented to experiment with different values of:
- `eps` (0.1 to 10)
- `min_samples` (2 to 10)

This helps in reducing outliers and improving cluster quality.

---

## 📊 Cluster Visualization
- Scatter plot between:
  - Annual Income (k$)
  - Spending Score
- Each cluster is color-coded
- Outliers are automatically highlighted
- Visualization created using Seaborn

---

## 📈 Applications
- Customer behavior analysis
- Detection of abnormal or rare customers
- Targeted marketing strategies
- Robust clustering without predefining cluster count

---

## ✅ Conclusion
This project demonstrates the power of **DBSCAN** in identifying meaningful customer segments while handling noise effectively. It is especially useful when the number of clusters is unknown and data contains outliers.

---

## 🚀 Future Enhancements
- Standardizing features before clustering
- Using Silhouette Score for parameter tuning
- Comparing DBSCAN with K-Means and Hierarchical clustering
- Visualizing clusters in interactive dashboards
