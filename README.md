# Sound Clustering Assignment  

## Overview  
This notebook explores clustering techniques for unlabeled sound data, focusing on dimensionality reduction and clustering algorithms. The goal is to improve cluster separability and interpretability of the data.  

## Key Concepts  

### **Dimensionality Reduction**  
- The dataset contains high-dimensional features, making direct visualization and clustering difficult.  
- **Principal Component Analysis (PCA)**: Used to reduce dimensionality while preserving variance.  
- **t-Distributed Stochastic Neighbor Embedding (t-SNE)**: Helps in visualizing non-linear relationships and improving cluster separability.  
- **Findings**: t-SNE provides better separation of clusters compared to PCA due to its ability to preserve local structures.  

### **Clustering Techniques**  
- **K-Means Clustering**: Assigns data points into clusters based on feature similarities.  
- **DBSCAN (Density-Based Spatial Clustering)**: Identifies clusters based on density, useful for irregularly shaped clusters.  
- **Evaluation Metrics**:  
  - **Silhouette Score**: Measures how well clusters are separated.  
  - **Davies-Bouldin Score**: Evaluates cluster compactness and separation.  

## Steps in the Notebook  
1. **Load and Preprocess Data**: Standardize features for consistency.  
2. **Apply Dimensionality Reduction**: Use PCA and t-SNE to visualize data.  
3. **Perform Clustering**: Compare K-Means and DBSCAN for grouping similar sounds.  
4. **Evaluate Results**: Use metrics and visualizations to analyze cluster quality.  

## Observations  
- t-SNE provides a clearer separation of clusters compared to PCA.  
- K-Means performs well but may struggle with complex shapes.  
- DBSCAN is effective for identifying noise and irregular patterns.  

## Dependencies  
- `numpy`, `pandas`, `matplotlib`, `seaborn`  
- `scikit-learn` for PCA, clustering, and metrics  
- `librosa` for sound feature extraction  

---
