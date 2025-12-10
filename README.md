# Customer Segmentation Using K-Means Clustering

This project presents a complete, reproducible tutorial on performing customer segmentation using K-Means Clustering with Principal Component Analysis (PCA) for visualisation. The objective is to identify behavioural groups within the Mall Customers dataset using numerical features such as Age, Annual Income, and Spending Score.

The notebook demonstrates the following workflow:

1. Exploratory Data Analysis (EDA)
2. Feature selection and standardisation
3. Determination of the optimal number of clusters using:
   - Elbow Method
   - Silhouette Coefficient
4. Running K-Means Clustering
5. Applying PCA for two-dimensional projection
6. Profiling and interpreting clusters
7. Discussion of limitations and methodological considerations

## Dataset

Mall Customers Dataset (200 rows, 5 columns).

Features used in clustering:
- Age
- Annual Income (k$)
- Spending Score (1-100)

Non-numerical features were excluded to maintain compatibility with Euclidean distance used by K-Means.

## Methods Used

### K-Means Clustering
A partition-based unsupervised learning method suitable for dividing data into K groups. Cluster validity is assessed using inertia and silhouette scores.

### Principal Component Analysis (PCA)
Used for visualising clusters in a reduced two-dimensional feature space.

## Workflow Summary

1. Load dataset and inspect its structure.
2. Plot distributions of Age, Income and Spending Score.
3. Standardise numerical features.
4. Evaluate inertia values across multiple K values.
5. Compute silhouette coefficients to support model selection.
6. Fit K-Means and generate cluster assignments.
7. Apply PCA and visualise clusters.
8. Produce cluster summary statistics.
9. Interpret cluster characteristics.

## Running the Notebook

Install dependencies:

```
pip install -r requirements.txt
```

Launch Jupyter:

```
jupyter notebook
```

Open the notebook file and execute all cells sequentially.

## Reproducibility

- A fixed random_state was used.
- All computations rely on standard open-source Python packages.
- Cluster profiles and PCA structure are consistent when dependencies are installed as listed.

## References

Jain, A. K. (2010). Data clustering: 50 years beyond K-means. Pattern Recognition Letters.

Jolliffe, I. T. (2002). Principal Component Analysis. Springer.

Lloyd, S. (1982). Least squares quantization in PCM. IEEE Transactions on Information Theory.

MacQueen, J. (1967). Some methods for classification and analysis of multivariate observations. University of California Press.

Wedel, M. & Kamakura, W. (2000). Market Segmentation. Springer.

## Repository Structure

- Notebook file  
- README.md  
- requirements.txt  
