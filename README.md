# 🛒 Customer Segmentation Using K-Means Clustering & RFM Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-K--Means%20Clustering-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 📌 Project Overview

This project performs **Customer Segmentation** for an Online Retail Store 
using the **K-Means Clustering** algorithm combined with **RFM Analysis** 
(Recency, Frequency, Monetary). The goal is to group customers into meaningful 
segments based on their purchase behavior — without any predefined labels — 
enabling the business to design targeted marketing campaigns for each group.

---

## 📊 Dataset

- **Source:** Online Retail Dataset (UCI Machine Learning Repository) - [Online_Retail_Dataset](https://drive.google.com/file/d/1XrCnmAAvT6D0TrtXacDbykUpwLAlUC03/view?usp=drive_link)
- **Size:** ~541,909 transaction records
- **Period:** December 2010 – December 2011
- **Features:** InvoiceNo, StockCode, Description, Quantity, InvoiceDate, 
  UnitPrice, CustomerID, Country

---

## 🛠️ Tools & Libraries

| Tool | Purpose |
|------|---------|
| Python | Core programming language |
| Pandas | Data loading and manipulation |
| NumPy | Numerical computations |
| Matplotlib & Seaborn | Data visualization |
| Scikit-learn | K-Means clustering, StandardScaler, Silhouette Score |
| SciPy | Euclidean distance calculation (cdist) |

---

## 🔄 Project Workflow

1. **Data Loading & Exploration** — Shape, dtypes, null values, basic stats
2. **Data Cleaning** — Removed nulls, negative quantities, invalid prices, cancelled invoices
3. **RFM Feature Engineering** — Created Recency, Frequency, Monetary per customer
4. **Outlier Removal** — IQR method (Q1 - 1.5×IQR to Q3 + 1.5×IQR)
5. **Feature Scaling** — StandardScaler (mean=0, std=1)
6. **Optimal K Selection** — Elbow Method + Silhouette Score → K=3
7. **K-Means Clustering** — Applied with K=3, random_state=42
8. **Cluster Analysis & Visualization** — 4 professional charts
9. **Outlier Detection** — Euclidean distance from centroids

---

## 📈 Key Results

| Cluster | Segment | Customers | Avg Recency | Avg Frequency | Avg Monetary |
|---------|---------|-----------|-------------|---------------|--------------|
| Cluster 0 | Regular Customers | 1,968 (53%) | 48.78 days | 2.12 times | £598.79 |
| Cluster 1 | At-Risk Customers | 920 (25%) | 226.80 days | 1.50 times | £414.09 |
| Cluster 2 | Premium Customers | 822 (22%) | 36.23 days | 6.05 times | £2,107.88 |

### Model Evaluation
- **Optimal K:** 3 (Elbow Method + Silhouette Score)
- **Final Inertia:** 3,502.54
- **Silhouette Score:** 0.4600

---

## 📂 Repository Structure

Customer-Segmentation-ML-Project/

├── Customer_segmentation_ML.py     # Complete Python source code

├── data/

│   └── data-dictionary.csv         # Dataset column descriptions

├── docs/

│   ├── Customer_Segmentation_Question.pdf

│   └── Customer_Segmentation_ML_Project_Completion.pdf

├── outputs/

│   └── (Visualization screenshots)

└── README.md


---

## 💡 Business Recommendations

| Segment | Strategy |
|---------|---------|
| Premium Customers | VIP rewards, loyalty programs, early access to products |
| Regular Customers | Upsell campaigns, engagement offers, product recommendations |
| At-Risk Customers | Win-back emails, discount offers, re-engagement campaigns |

---

## 👤 Author

**Swaroop Kumar Vathada**  
Data Analyst | Power BI Developer  
📧 swaroop.vathada@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/swaroopkumarvathada)  
🐙 [GitHub](https://github.com/swaroop456)  
🌐 [Portfolio](https://swaroop456.github.io/Data_Analyst_Portfolio/)
