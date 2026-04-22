# Demographic Segmentation & PCA Analysis

This project applies unsupervised learning techniques to segment demographic data from the "Adult Income" dataset. The goal is to identify distinct population subgroups and reduce data complexity while retaining the most significant statistical information.

## 📊 Dataset Analysis
The project utilizes a dataset of 32,560 entries featuring 15 demographic attributes, including:
* **Numerical:** Age, Education-num, Capital Gain/Loss, Hours per week.
* **Categorical:** Workclass, Marital Status, Occupation, Relationship, Race, and Native Country.

## 🚀 Key Features
### 1. Dimensionality Reduction (PCA)
To handle the high-dimensional nature of the dataset, **Principal Component Analysis (PCA)** was implemented. This allowed for:
* Reducing the feature space while maintaining maximum variance.
* 2D and 3D visualization of complex demographic patterns.

### 2. Clustering Algorithms
The project implements and compares two primary clustering methods:
* **K-Means Clustering:** Optimized using the **Elbow Method** and **Silhouette Scores** to determine the ideal number of segments (k=8).
* **Agglomerative Hierarchical Clustering:** Used to explore the nested relationships within the data.

### 3. Advanced Visualization
* **Dendrograms:** A hierarchical tree diagram was generated to visualize the distance between clusters and justify the "cut" at 8 clusters.
* **Cluster Scatter Plots:** Visualizing segments within the PCA-transformed space.
* **Heatmaps:** Analyzing feature importance across different clusters.

## 🛠️ Tech Stack
* **Language:** Python
* **Data Processing:** Pandas, NumPy
* **Visualization:** Seaborn, Matplotlib
* **Machine Learning:** Scikit-learn (PCA, KMeans, AgglomerativeClustering)
* **Statistics:** Scipy (Linkage, Dendrogram)

## 📈 Key Insights
* **Component Variance:** PCA revealed how a small subset of transformed features captures the majority of the population's variance.
* **Hierarchical Structure:** The dendrogram analysis provided a clear visual threshold for defining demographic groups, showing how education and occupation often group together to define socio-economic segments.

## 📂 Repository Structure
* `adult.ipynb`: The complete analysis pipeline, from preprocessing to hierarchical clustering.
* `dendrogram_plot.png`: Exported visualization of the cluster hierarchy.
