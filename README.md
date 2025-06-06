# 🧪 K-Means Clustering on Customer Segmentation

This project applies **K-Means Clustering** on a customer dataset to discover patterns and perform segmentation. Multiple combinations of features were tested, and clustering performance was evaluated using **Silhouette Scores**.

---

## 📊 Dataset Description

The dataset contains the following attributes for each customer:

- `Gender`
- `Age`
- `Annual Income (k$)`
- `Spending Score (1-100)`

---

## ⚙️ K-Means Clustering Cases

The K-Means algorithm was applied using different combinations of features. Each case's clustering effectiveness was measured using the **Silhouette Score** (higher is better).

| Feature Combination                                       | k  | Silhouette Score |
|-----------------------------------------------------------|----|------------------|         
| `Age`, `Spending Score (1–100)`                           | 5  | 0.4463           |
| `Annual Income (k$)`, `Spending Score (1–100)`            | 5  | **0.5595**       |
| `Age`, `Annual Income (k$)`, `Spending Score (1–100)`     | 6  | 0.4235           |
| `Gender`, `Annual Income (k$)`, `Spending Score (1–100)`  | 5  | 0.4121           |
| `Age`, `Gender`, `Spending Score (1–100)`                 | 5  | 0.4772           |


## 📈 Visualizations

Clustering results were visualized using scatter plots for each case. Below are some sample visual outputs:
### 📌 Clustering with `Age`, `Gender`, `Spending Score` (k=5)
![Age , Gender,Spending Clusters](/fig55.png)

### 📌 Clustering `Gender`,`Annual Income` and `Spending Score` (k=5)
![Gender,Annual Spending Score Clusters](/fig66.png)

### 📌 Clustering with `Age` and  `Spending Score` (k=5)
![Age and Spending Clusters](/fig88.png)

### 📌 Clustering with `Annual Income`, `Spending Score` (k=5)
![Annual, Spending Clusters](/fig99.png)


---

## ✅ Conclusion

K-Means clustering was effective for customer segmentation. The best clustering performance was observed with:

- `Annual Income` and `Spending Score` (k=5) → **Silhouette Score: 0.5595**
- `Age` and `Gender` (k=4) → **Silhouette Score: 0.5595**

These feature pairs produced the most distinct clusters and highest silhouette scores, indicating strong intra-cluster cohesion and inter-cluster separation.

Other combinations yielded useful but slightly less defined clusters.

---

## 🛠 Tools Used

- Python 🐍
- Scikit-learn
- Pandas
- Matplotlib / Seaborn
- NumPy

---
