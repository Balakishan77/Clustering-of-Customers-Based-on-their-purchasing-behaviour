# Clustering-of-Customers based on K-Means clustering algorithm

Acknowledgements: I have taken this E-commerce dataset from Kaggle to practise purpose only If this is against the TOS, please let me know and I will take it down.

  Analyzing the content of an E-commerce dataset that lists purchases made by  4339 customers over a period of one year (from 2010/12/01 to 2011/12/09) and group them based on the purchases they made. Based on this analysis, I have developed a clustering model that allows to cluster the customers based on their purchases.


# K-Means Clustering Introduction:
  K-means clustering is a type of unsupervised learning, which is used when you have unlabeled data (i.e., data without defined categories or groups). The goal of this algorithm is to find groups(clusters) in the data and will find the number of groups(K) using Elbow method. The algorithm works iteratively to assign each data point to one of K groups based on the features that are provided. Data points are clustered based on feature similarity.
  
  Plot of Training data

  ![traing data](https://user-images.githubusercontent.com/40944675/43999552-0e8ff17a-9e2c-11e8-80d1-0cb2ec0aeb75.png)
  
# Choosing K : Using Elbow Method to find the number of clusters
  The algorithm described above finds the clusters and data set labels for a particular pre-chosen K. To find the number of clusters in the data,we need to run the K-means clustering algorithm for a range of K values and compare the results. In general, there is no method for determining exact value of K, but an accurate estimate can be obtained using the following techniques.
  One of the metrics that is commonly used to compare results across different values of K is the mean distance between data points and their cluster centroid(WCSS - With in Cluster Sum of Squares). Since increasing the number of clusters will always reduce the distance to data points, increasing K will always decrease this metric, to the extreme of reaching zero when K is the same as the number of data points. Thus, this metric cannot be used as the sole target. Instead, mean distance to the centroid as a function of K is plotted and the "elbow point," where the rate of decrease sharply shifts(where distortion goes rapidly), can be used to roughly determine K.
  
Based on the analysis below is  the Elbow method results.We can estimate that elbow point as 3 and have chosen K=3 for further analysis.
 
  ![no_of_clusters](https://user-images.githubusercontent.com/40944675/43999244-55f162ca-9e26-11e8-9d55-608b1bce64da.png)

Based on the analysis below are the final clustering of customers results and some analysis.

  ![final_results](https://user-images.githubusercontent.com/40944675/43999217-bcce1610-9e25-11e8-8af1-087cde7c700f.png)

Customer Type 1  : These customers like to purchase few products with low price

Customer Type 2  : These customers like to purchase more products with low price

Customer Type 3  : These customers like to purchase few products with high price
