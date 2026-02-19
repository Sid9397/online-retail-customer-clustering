# 🛒 Customer Segmentation using RFM Analysis & K-Means Clustering

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1rgihQbzhOQKZoO5lSZZQxqqfKVHbS6CA)

---

## 🎯 Business Objective

An online retail company wants to understand customer purchasing behavior in order to:

- Identify high-value customers
- Improve marketing strategies
- Increase customer retention
- Enable data-driven business decisions

This project applies **RFM Analysis (Recency, Frequency, Monetary)** combined with **K-Means Clustering** to segment customers into meaningful business groups.

---

## 📊 Dataset

The dataset contains real-world online retail transactions including:

- CustomerID
- InvoiceNo
- InvoiceDate
- Quantity
- UnitPrice
- Country

Initial Size: **541K+ transactions**

---

## 🧹 Data Preprocessing

Key cleaning steps performed:

- Removed negative Quantity values (product returns)
- Removed rows with missing CustomerID
- Converted InvoiceDate to datetime format
- Created TotalAmount feature:
  
TotalAmount = Quantity × UnitPrice


---

## ⚙️ Feature Engineering (RFM Model)

Customer-level features were created using groupby(CustomerID):

- **Recency** → Days since last purchase
- **Frequency** → Number of transactions
- **Monetary** → Total spending amount

This transforms transaction data into customer behavior data.

---

## 🤖 Model Training

Clustering performed using:

- K-Means++
- StandardScaler for normalization

Optimal clusters determined using:

- Elbow Method
- Silhouette Score

---

## 📈 Model Evaluation

| Metric | Score |
|------|------|
| Silhouette Score | 0.61 |
| Davies–Bouldin Index | 0.75 |
| Calinski–Harabasz Score | 3149.99 |

These metrics indicate strong cluster separation and compact grouping.

---

## 👥 Customer Segments (RFM Interpretation)

| Cluster Type | Business Meaning |
|-------------|------------------|
| High Value Customers | Recent, frequent, high spending |
| Loyal Customers | Frequent buyers with steady spending |
| At-Risk Customers | Long time since last purchase |
| Low Engagement Customers | Low frequency and spending |

---

## 📊 Visualization

- Elbow curve for optimal K selection
- Silhouette validation
- 3D Customer Segmentation (Recency–Frequency–Monetary)

---

## 💼 Business Insights

✅ Focus retention campaigns on high-value customers  
✅ Re-engage at-risk customers with targeted offers  
✅ Maintain loyalty programs for frequent buyers  
✅ Reduce marketing cost on low-engagement segments

---

## 🛠 Tools & Libraries

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## 🚀 Key Learning Outcomes

- End-to-end unsupervised ML workflow
- Real-world customer analytics
- Feature engineering using RFM modeling
- Cluster validation techniques
- Business interpretation of ML results

---

## 📂 Project Structure

customer-segmentation-rfm-kmeans/
│
├── Online_Retail_KMeans.ipynb
└── README.md


---

## ⭐ Author

**Siddharth Asha**  
Machine Learning & Data Analytics Enthusiast
