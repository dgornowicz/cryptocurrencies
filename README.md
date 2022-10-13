# Cryptocurrency Clustering

## Analysis Overview
The purpose of this project is to use unsupervised machine learning to analyze a database of cryptocurrentcies and create a report including the traded cryptocurrencies classified by group according to their features.\
This Classification report could be used by an investor to propose a new cryptocurrency investment portfolio to their client. \
We use the following methods for the analysis:
- Preprocessing data
- Reducing data dimensionality using Principal Component Analysis
- Clustering cryptocurrencies using K-Means
- Visualizing classification results with 2D and 3D scatter plots
<br><br>

## Resources
- Data Source:
- Software: Python, Anaconda Navigator, Conda, Jupyter Notebook

## Results
Following the preprocessing and cleaning phase, we have a total of 532 tradable cryptocurrencies.
<br><br>

### Clustering Cryptocurrencies using K-Means - Elbow Curve
We don't know the optimal number of clusters for analyzing the cryptocurrencies. \
We produced the elbow curve below using the K-Means method iterating on k values from 1 to 10.

<img width="375" alt="elbowcurve" src="https://user-images.githubusercontent.com/102050273/195731103-6a3ee81c-067c-40e6-9fa3-0ccab6531956.png">

The best K-Value appears to be 4 so we will use this value for our clustering.

### Visualizing Cryptocurrency Results
#### 3D-Scatter plot with clusters
<img width="305" alt="3dScatter" src="https://user-images.githubusercontent.com/102050273/195731254-d49bc9d3-ed96-4c9a-b41e-06e87a69e0d4.png">

This 3D-Scatter plot was obtained using the PCA algorithm to reduce the cryptocurrencies dimensions to three principal components.
<br><br>

