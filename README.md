# Leaf Clustering Analysis 🌿

This project applies **k-means clustering** to a morphometric dataset of 340 plant leaf specimens, 
using 14 quantitative features describing **shape** and **texture** to explore morphological diversity.

## 🧩 Dataset
Dataset: *Leaf* (UCI Machine Learning Repository)  
Source: Silva & Marçal (2013), *Evaluation of Features for Leaf Discrimination*.  
The data includes features such as:
- Eccentricity, Aspect Ratio, Elongation, Solidity
- Stochastic Convexity, Isoperimetric Factor, Max Indentation Depth, Lobedness
- Average Intensity, Contrast, Smoothness, Third Moment, Uniformity, Entropy

## 🔍 Objective
Identify distinct leaf morphology groups based on shape and texture descriptors.

## 🧠 Methodology
- **Standardization** of features  
- **PCA** for dimensionality reduction  
- **k-Means Clustering** (k = 4) chosen via elbow & silhouette methods  
- **Validation metrics:** inertia, silhouette score, and R² (BSS/TSS = 0.664)

## 📈 Results
Four distinct morphological clusters:
1. Smooth convex leaves, moderate texture  
2. Deeply lobed leaves, subtle texture  
3. Smooth margins, strong texture  
4. Moderately lobed, moderately textured  

These clusters captured **66.4% of total variance** and visually separated well in PCA plots.

## 📘 Files
| File | Description |
|------|--------------|
| `Clustering Leaves.ipynb` | Notebook implementing preprocessing, PCA, and k-means |
| `Identifying Leaves using Clustering.pdf` | Project report |
| `Appendix A - ReadMe Documentation on Leaf Features.pdf` | Feature definitions |

## 🧾 References
Silva, P.F. & Marçal, A.R.S. (2013). *Evaluation of Features for Leaf Discrimination*.  
James et al. (2023). *An Introduction to Statistical Learning with Applications in Python*.  
Rousseeuw (1987). *Silhouettes: A Graphical Aid to the Interpretation and Validation of Cluster Analysis*.

## 🧑‍💻 How to Run
1. Install dependencies:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
