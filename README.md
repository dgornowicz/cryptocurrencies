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
We don't know the optimal number of clusters for analyzing the cryptocurrencies. We produced the elbow curve below using the K-Means method iterating on k values from 1 to 10.
