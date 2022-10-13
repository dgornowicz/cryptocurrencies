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
- Data Source: [crypto_data.csv](https://github.com/dgornowicz/cryptocurrencies/blob/main/crypto_data.csv), [CryptoCompare](https://min-api.cryptocompare.com/data/all/coinlist)
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

#### 2D-Scatter plot with clusters
<img width="358" alt="2pcaScatter" src="https://user-images.githubusercontent.com/102050273/195731582-e8ab7d28-6786-4827-bce9-96c0c3c9dcac.png">

This scatter plot was obtained using the PCA algorithm to reduce the cryptocurrencies dimensions to two principal components.
<br><br>
Both of the scatter plots show the distribution and the four clusters of cryptocurrencies. We can identify the outliers like the unique cryptocurrency in class 2.

#### Tradable Crytocurrencies Table
<img width="340" alt="hvplotTable" src="https://user-images.githubusercontent.com/102050273/195731540-2e62f5eb-6c2d-4d73-ac9f-e090f7f9f02b.png">
Most of the cryptocurrencies are part of class 0 or 1. The table above shows that BitTorrent is the only cryptocurrency in class 2.

#### 2D-Scatter plot with TotalCoinsMined vs TotalCoinSupply
<img width="355" alt="supplyVSmined" src="https://user-images.githubusercontent.com/102050273/195732136-88970769-2498-4077-870c-654e13d14794.png">
Plotting the scatter plot from two cryptocurrency features directly does not efficiently segregate the different classes. Therefore, using the PCA algorithm is the right method for better visualizations.
<br><br>

## Summary
We have identified the classification of 532 cryptocurrencies based on similarties between their features.\
Further analysis of the cryptocurrencies would be needed to asses their performance for potential investment.

