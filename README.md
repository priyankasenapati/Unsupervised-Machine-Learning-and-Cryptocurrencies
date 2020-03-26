# Unsupervised-Machine-Learning-and-Cryptocurrencies
## Purpose :

In this project, we used unsupervised learning to analyze data on Crytocurrencies traded on market.


## Objectives:

The goals for this challenge are for you to:

* Prepare the data for dimensions reduction with PCA and clustering using K-means.

* Reduce data dimensions using PCA algorithms from sklearn.

* Predict clusters using cryptocurrencies data using the K-means algorithm form sklearn.

* Create some plots and data tables to present your results.

## Resources:
* Data source: crypto_data.csv.

* Software: Python 3.7 using libraries: Pandas, Scikit-learn, hvplot and Plotly Express; Jupyter Notebook.


## Data Preprocessing:

1. Remove all cryptocurrencies that aren’t trading.

2. Remove all cryptocurrencies that don’t have an algorithm defined.

3. Remove the "IsTrading" column.

4. Remove all cryptocurrencies with at least one null value.

5. Remove all cryptocurrencies without coins mined.

6. Store the names of all cryptocurrencies on a DataFramed named coins_name.

7. Remove the CoinName column.

8. Create dummies variables for all of the text features, and store the resulting data on a DataFrame named X.

9. Use the StandardScaler from sklearn (Links to an external site.) to standardize all of the data from the X DataFrame.
<img width="789" alt="Xscaled png " src="https://user-images.githubusercontent.com/55486501/77685842-1717dd80-6fc2-11ea-8292-65793ec2e480.png">


## Reducing Data Dimensions Using PCA:
Created a DataFrame named “pcs_df” that includes the following columns: PC1, PC2, and PC3.

<img width="813" alt="pca" src="https://user-images.githubusercontent.com/55486501/77685970-4595b880-6fc2-11ea-94b8-5a518be5d7ef.png">

## Clustering Cryptocurrencies Using K-means:

1- Create an elbow curve to find the best value for K.
<img width="836" alt="elbowcurve" src="https://user-images.githubusercontent.com/55486501/77686106-70800c80-6fc2-11ea-92d2-f084d5a4af9c.png">

*The best value for K is 4.
2. Run the K-means algorithm to predict the K clusters for the cryptocurrencies’ data.

3. Create a new DataFrame named “clustered_df” with columns: Algorithm, ProofType, TotalCoinsMined, TotalCoinSupply, PC 1, PC 2, PC 3, CoinName, and Class.
<img width="687" alt="finaldf" src="https://user-images.githubusercontent.com/55486501/77686214-94dbe900-6fc2-11ea-9271-6325a4ae2a55.png">

## Visualizing Results:

1. Created a 3D scatter plot using Plotly Express to plot the clusters using the clustered_df DataFrame. 
<img width="945" alt="3D" src="https://user-images.githubusercontent.com/55486501/77686287-b3da7b00-6fc2-11ea-870a-20eac34e3c98.png">

2.Use hvplot.table to create a data table with all the current tradable cryptocurrencies.
<img width="527" alt="table" src="https://user-images.githubusercontent.com/55486501/77686344-d2d90d00-6fc2-11ea-9509-9b1c8a967735.png">

3.Created a scatter plot using hvplot.scatter to present the clustered data about cryptocurrencies.
<img width="781" alt="chart" src="https://user-images.githubusercontent.com/55486501/77686406-edab8180-6fc2-11ea-890d-1fa57c81f577.png">











