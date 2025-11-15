# 📊 Clustering Analysis Project  
**Author:** Chengze Liu  
**UH ID:** 2316609  

This project implements and analyzes multiple clustering algorithms — **K-Means**, **DBSCAN**, and **Agglomerative (Hierarchical) Clustering** — on an Air Quality dataset. It includes custom implementations of evaluation metrics, parameter sweeps, visualizations, and comparisons of clustering performance.

---

## 🚀 Project Overview

The project consists of six main tasks executed in the notebook `clustering.ipynb`.

### **✓ Task 1 — Compute Purity**
Implemented a custom `compute_purity(y_true, y_pred)` function.  
Purity measures the proportion of dominant class labels within each cluster.



### **✓ Task 2 — Compute SSE (Sum of Squared Errors)**
Implemented `compute_sse(x, y_pred)` to evaluate cluster compactness.  
Tested using the **Iris dataset**.



### **✓ Task 3 — K-Means with k = 4**
Ran K-Means with `k=4` and reported: 
- Number of points per cluster  
- Percentage of points per cluster
- Overall purity and cluster purities



### **✓ Task 4 — K-Means on k = 2, 3, 4, 10, 20, 30**
For each value of `k`:
- Ran K-Means **10 times**  
- Computed **average purity**  
- Computed **average SSE**  
- Organized results into a summary table
- Investigated the influence of k on purity and SSE





### **✓ Task 5 — DBSCAN Parameter Sweep**
Ran DBSCAN with: `eps=0.8, 0.9, 1.0, 1.1, 1.2, minPts=5` and reported:
- Number of clusters
- Number of anomalies
- Purity
- SSE
- Silhouette coefficient
- Organized results into a summary table
- Investigated the influence of eps on purity, SSE, and Silhouette coefficient



## **✓ Task 6 — Agglomerative Clustering**
Ran Agglomerative Clustering with: `distance_threshold=25, 75, 125, n_cluster=none`
- plotted the dendrogram using `scipy.cluster.hierarchy.dendrogram` 
- For each distance_threshold:
- Computed number of clusters
- Computed purity
- Computed SSE
- Organized rusults into a table 
- Selected `distance_threshold` among `[22, 29, 46, 60, 91]` that gives 5 clusters, using the dendrogram

---
## Structure

- `clustering.ipynb` — Main notebook containing preprocessing, clustering experiments, visualizations, and analysis.
- `README.md` — Project overview.
- `air_quality.csv` - Air Quality dataset
- `Iris.csv` - Iris dataset
- `report 3 clustering.pdf` - Report

---
## Technologies Used

- Python 3  
- NumPy  
- Pandas  
- Scikit-learn  
- Matplotlib  

---
## How to Run

1. Install dependencies  
2. Open and run the Jupyter notebook

---

## License
MIT License


