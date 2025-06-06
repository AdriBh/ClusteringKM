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
| `Age`, `Gender`                                           | 5  | **0.5595**       |
| `Age`, `Spending Score (1–100)`                           | 5  | 0.4463           |
| `Age`, `Annual Income (k$)`, `Spending Score (1–100)`     | 6  | 0.4235           |
| `Gender`, `Annual Income (k$)`, `Spending Score (1–100)`  | 5  | 0.4121           |
| `Age`, `Gender`, `Spending Score (1–100)`                 | 4  | 0.4772           |

---

## 📈 Visualizations

Clustering results were visualized using scatter plots for each case. Below are some sample visual outputs:
### 📌 Clustering with `Age` and `Gender` (k=5)
![Age and Gender Clusters](/fig55.png)

### 📌 Clustering with `Age` and `Spending Score` (k=5)
![Age and Spending Score Clusters](/fig66.png)

### 📌 Clustering with `Age`, `Annual Income`, `Spending Score` (k=6)
![Age, Income, Spending Clusters](/fig88.png)

### 📌 Clustering with `Gender`, `Income`, `Spending Score` (k=5)
![Gender, Income, Spending Clusters](/fig99.png)


---

## 📌 Observations

- The highest silhouette score was achieved using **`Age` and `Gender`** (`0.5595`), indicating more distinct clusters.
- Adding too many features did not always improve clustering quality.
- `Spending Score` paired with `Age` or `Gender` also gave meaningful clusters.

---

## 🛠 Tools Used

- Python 🐍
- Scikit-learn
- Pandas
- Matplotlib / Seaborn
- NumPy

---
