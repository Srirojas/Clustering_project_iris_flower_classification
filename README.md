# Clustering Project : Iris Flower Classification

## Project Overview :
This project applies K-Means Clustering to a supervised dataset (Iris Flower Classification) to evaluate how effectively an unsupervised algorithm can classify species based on feature similarities. The goal is to determine the optimal number of clusters and compare the predicted groups with actual species labels.

## Objective :
 - Apply clustering on labeled data to assess the performance of K-Means in classifying species.
 - Identify the optimal number of clusters (K) using the Elbow Method.
 - Compare predicted clusters with actual species labels to analyze misclassifications.

## Dataset : 
Shape: (210, 6) → 210 samples & 6 features
Features: Area, Perimeter, Compactness, Kernel length, Kernel width, Asymmetry Coefficient
Target: Species
Excluded Feature: Groove Length (not required for classification) 

## Approach & Methodology :
1.Data Preprocessing
 - Imported necessary libraries: pandas, sklearn (MinMaxScaler, PCA, KMeans), matplotlib 
 - Scaled the data for uniform feature distribution.
2.Finding the Optimal K
 - Used Within-Cluster Sum of Squares (WCSS) to determine the best K value.
 - The Elbow Method identified K=3 as the ideal number of clusters.
3.Applying K-Means Clustering
 - Fit the model to create 3 clusters.
 - Compared predicted vs actual species to evaluate performance.

## Key Observations :
### Elbow Method Analysis
 - The WCSS decreases significantly from K=1 to K=2, with a further drop at K=3.
 - Beyond K=3, the reduction in WCSS is minimal, indicating three well-separated clusters.
### Cluster Performance
 - Most data points are classified correctly.
 - Some boundary cases show misclassification, but the overall clustering performance is strong.

## Visualization :
Elbow Method plot, which helped identify the optimal number of clusters.

## Technologies Used : 
 - Python 
 - Pandas – Data handling
 - Matplotlib – Data visualization
 - Scikit-learn – Machine learning models

## Results & Impact :
 - Successfully classified Iris flowers into 3 clusters.
 - Demonstrated how clustering can work on supervised data.
 - Identified misclassified data points near boundaries.
 - Proved that K-Means can effectively detect patterns in labeled datasets.
