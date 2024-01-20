# PCA Projection and Visualization

This README describes how to perform PCA (Principal Component Analysis) with 2 components on a dataset and how to visualize the explained variance and PCA projection.

## Performing PCA on the Dataset

To perform PCA on your dataset, follow these steps:

1. Initialize the PCA object with the desired number of components.
2. Fit the PCA on the dataset array.
3. Visualize the explained variance and the PCA projection.

To understand PCA concept, you may refer this.

Here is the Python code to accomplish this:
```python
# Assuming X is your data matrix
pca = PCA(n_components=2)
pca.fit(np.array(X))
pca.visualization(explained_variace=True, PCA_projection=True)
X_proj = pca.X_proj   # Projected data
PC1_X = pca.components[:, 0]  # First principal component

**Note:** This repo was a homework practice for ML class.
```bibtex
@author {
  author       = {Loci Tran},
  course       = {Introduction of Statistics and Machine Learning (II)},
  year         = {2023},
}
```


