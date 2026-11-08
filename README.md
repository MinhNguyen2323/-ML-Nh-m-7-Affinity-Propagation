# Customer Segmentation with Affinity Propagation

**Unsupervised Machine Learning | Customer Analytics | Python**

## 📌 Overview

This project explores **Affinity Propagation (AP)** for customer segmentation using the *Customer Personality Analysis* dataset. The goal is to identify meaningful customer groups based on purchasing behavior and demographic characteristics, while evaluating AP against K-Means and Hierarchical Agglomerative Clustering (HAC).

## 🔍 Methodology

1. **Data Preprocessing:** Cleaned missing values, engineered customer features, encoded categorical variables, and standardized numerical data.
2. **Dimensionality Reduction:** Applied PCA to retain 10 principal components.
3. **Clustering:** Tuned Affinity Propagation's preference parameter and identified representative customer groups.
4. **Evaluation:** Compared clustering quality, execution time, and memory usage against K-Means and HAC.

## 📊 Key Results

| Metric | Result |
|---|---|
| Optimal AP Preference | -1800 |
| Identified Clusters | 2 |
| AP Silhouette Score | **0.406** |
| K-Means Silhouette Score | 0.396 |

Affinity Propagation achieved the strongest clustering quality among the three evaluated methods based on Silhouette, Davies–Bouldin, and Calinski–Harabasz metrics.

### Customer Insights

- **Cluster 0 | High-Value Customers:** Higher income and spending, particularly on wine and meat products, with stronger purchasing activity through catalogs and stores.
- **Cluster 1 | Budget-Conscious Customers:** Lower income and spending, with relatively greater online browsing activity.
- **Key Differentiators:** Income, wine expenditure, and meat expenditure were the most influential features in distinguishing customer segments.

These findings suggest opportunities for differentiated customer targeting and personalized marketing strategies.

## ⚖️ Strengths & Limitations

**Strengths**
- Automatically identifies cluster exemplars without requiring a predefined number of clusters.
- Produces interpretable customer segments with meaningful business implications.
- Outperforms the evaluated baselines on internal clustering quality metrics.

**Limitations**
- Higher computational time and memory consumption than K-Means and HAC.
- Scalability challenges for larger datasets.
- Customer segments are exploratory and require further validation before business deployment.

## 🛠️ Tech Stack

`Python` · `Pandas` · `NumPy` · `Scikit-learn` · `Matplotlib` · `Seaborn` · `Jupyter Notebook`

## 📂 Repository Structure

```text
├── 1 AP explanation.ipynb
├── 2 Preprocessing.ipynb
├── 3 AP clustering and Knowledge.ipynb
├── 4 Comparison.ipynb
├── marketing_campaign.csv
└── README.md
```

## 📚 Dataset & Acknowledgment

- **Dataset:** [Customer Personality Analysis (Kaggle)](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)
- **Project:** Machine Learning coursework, University of Economics Ho Chi Minh City (UEH).
- **Collaboration:** Developed as a five-member academic team project.

*This project demonstrates the trade-off between clustering quality, computational efficiency, and business interpretability.*
