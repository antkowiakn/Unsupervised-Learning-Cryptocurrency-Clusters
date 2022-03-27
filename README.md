# Unsupervised Learning: Cryptocurrency Clusters  

A prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, is lost in the vast universe of cryptocurrencies. They’ve asked to create a report that includes what cryptocurrencies are on the trading market and determine whether they can be grouped to create a classification system for this new investment.  
  
### Data Preparation

Read `crypto_data.csv` into Pandas. The dataset was obtained from [CryptoCompare](https://min-api.cryptocompare.com/data/all/coinlist).

Discard all cryptocurrencies that are not being traded.  
Remove all rows that have at least one null value.  
Filter for cryptocurrencies that have been mined.  
Convert the remaining features with text values into numerical data.  
Standardize the dataset so that columns that contain larger values do not unduly influence the outcome.  
  
### Dimensionality Reduction  
  
Perform dimensionality reduction with PCA.  Further reduce the dataset dimensions with t-SNE and visually inspect the results. In order to accomplish this task, run t-SNE on the principal components: the output of the PCA transformation. Then create a scatter plot of the t-SNE output. Observe whether there are distinct clusters or not.  
  
### Cluster Analysis with k-Means  
  
Create an elbow plot to identify the best number of clusters. Use a for-loop to determine the inertia for each `k` between 1 through 10. Determine, if possible, where the elbow of the plot is, and at which value of `k` it appears.  
  
## References  
  
Crypto Coin Comparison Ltd. (2020) Coin market capitalization lists of crypto currencies and prices. Retrieved from [https://www.cryptocompare.com/coins/list/all/USD/1](https://www.cryptocompare.com/coins/list/all/USD/1)  
