# Principle Component Analysis (PCA)

## Goal of PCA

PCA aims to find the directions that maximize variance while retaining as much information as possible. As PCA does not depend on the labels of the samples, it is considered an unsupervised learning method.

## Training Data Representation

The training data is represented as an \( n \times m \) matrix:


Here, \( n \) is the number of samples, and \( m \) is the number of features. The average of each feature \( k \) is calculated as:


## Variance-Covariance Matrix

The variance-covariance matrix \( C \) is calculated through matrix \( Q \):


Then, \( C \) is the dot product of \( Q \) and its transpose \( Q^T \):


## Eigendecomposition

Eigendecomposition is used to decompose the variance-covariance matrix into eigenvalues \( \lambda_i \) and eigenvectors \( v_i \):


The eigenvalues are sorted in descending order:


The first principal component \( v_1 \) shows the most variance when data is projected onto it. Similarly, the second principal component \( v_2 \) shows the second most variance.

## Projection

The projections onto the principal components are calculated as:


## PCA Explained Variance

The explained variance for PCA is defined as the ratio of each eigenvalue to the sum of all eigenvalues, indicating how much variance each component explains.


## Principal Components

The first principal component is broken down as follows:


The weights \( w_{11}, \ldots, w_{m1} \) represent how much each feature contributes to PC1.

## Data Preprocessing

Prior to PCA, data normalization is essential. The Z-score method is used to standardize features and remove differences in variance magnitude that might affect PCA results.

