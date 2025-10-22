# Leaf Clustering Analysis

This project applies K-Means clustering to a morphometric dataset of 340 plant leaf specimens.  
It explores how shape and texture features can automatically group leaves into distinct morphological categories.

---

## Dataset
Dataset: Leaf (UCI Machine Learning Repository)  
Source: Silva & Marçal (2013), *Evaluation of Features for Leaf Discrimination*.

The data contains 14 quantitative features derived from scanned leaf images —  
8 describe shape (e.g., eccentricity, solidity, lobedness) and 6 describe texture (e.g., contrast, entropy).

---

## Objective
Identify clusters of leaves based on shape and texture to reveal natural groupings in plant morphology.

---

## Methodology
1. Data Standardization – All numeric features scaled to zero mean and unit variance.  
2. Dimensionality Reduction (PCA) – Simplified the dataset for visualization.  
3. K-Means Clustering – Explored k = 1–10, selected k = 4 via elbow and silhouette methods.  
4. Validation – Calculated R² = 0.664, indicating that 66.4% of total variance was explained by clusters.

---

## Results
The analysis identified four well-separated clusters representing combinations of leaf smoothness and texture:

| Cluster | Description |
|:--|:--|
| 1 | Smooth convex leaves with moderate texture |
| 2 | Deeply lobed leaves with muted texture |
| 3 | Smooth margins, strong surface texture |
| 4 | Moderately lobed and textured leaves |

These results align with both PCA projections and feature-pair scatterplots.

---

## File Structure

### Recommended File Order
GitHub displays files alphabetically. To maintain a logical order, rename the files with numeric prefixes as shown below.

