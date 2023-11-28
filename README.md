# Unsupervised-Learning-Challenge

In this activity I've performed the following:
Combined financial Python programming skills with the new unsupervised learning skills that I acquired

Created a Jupyter notebook that clusters cryptocurrencies by their performance in different time periods. Then I plot the results so that I can visually show the performance to the board.

The provided CSV file contains the price change data of cryptocurrencies in different periods.

Instructions for this challenge are given below:

Import the data (provided in the starter code).

Prepare the data  (provided in the starter code).

Find the best value for k by using the original data.

Cluster the cryptocurrencies with K-means by using the original data.

Optimize the clusters with principal component analysis.

Find the best value for k by using the PCA data.

Cluster the cryptocurrencies with K-means by using the PCA data.

Visualize and compare the results.

IMPORTANT
For this Challenge, I assumed that k refers to lowercase k. The instructions will specify "uppercase K" where necessary.

Find the Best Value for k by Using the Original Data
In this section, I used the elbow method to find the best value for k by using the original data. To do so, I completed the following steps:

Coded the elbow method algorithm to find the best value for k. Used a range from 1 to 11.

To visually identify the optimal value for k, plot a line chart of all the inertia values computed with the different values of k.

Answered the following question: What’s the best value for k?

Cluster the Cryptocurrencies with K-Means by Using the Original Data
In this section, you’ll use the K-means algorithm along with the best value for k that you found by using the original data. Specifically, you’ll use them to cluster the cryptocurrencies according to the provided price changes of the cryptocurrencies provided. To do so, complete the following steps:

Initialized the K-means model with four clusters by using the best value for k.

Fit the K-means model by using the original data.

Predicted the clusters for grouping the cryptocurrencies by using the original data. Reviewed the resulting array of cluster values.

Created a copy of the original data, and then add a new column of the predicted clusters.

Using hvPlot, created a scatter plot by setting x="PC1" and y="PC2". Colored the graph points with the labels that you found by using K-means. Then added the crypto name to the hover_cols parameter to identify the cryptocurrency that each data point represents.

Optimized the Clusters with Principal Component Analysis
In this section, I performed PCA and reduce the features to three principal components. To do so, I completed the following steps:

Created a PCA model instance, and set n_components=3.

Used the PCA model to reduce the features to three principal components. Then reviewed the first five rows of the DataFrame.

Got the explained variance to determine how much information can be attributed to each principal component.

Answered the following question: What’s the total explained variance of the three principal components?

Created a new DataFrame with the PCA data. Set the coin_id index from the original DataFrame as the index for the new DataFrame. ReviewED the resulting DataFrame.

Find the Best Value for k by Using the PCA Data
In this section, I used the elbow method to find the best value for k by using the PCA data. To do so, I completed the following steps:

Coded the elbow method algorithm, and use the PCA data to find the best value for k. Use a range from 1 to 11.

To visually identify the optimal value for k, plot a line chart of all the inertia values computed with the different values of k.

Answered the following questions: What’s the best value for k when using the PCA data? Does it differ from the best value for k that you found when using the original data?

Cluster the Cryptocurrencies with K-means by Using the PCA Data
In this section, I used the PCA data, the K-means algorithm, and the best value for k that I found by using the PCA data. Specifically, I used them to cluster the cryptocurrencies according to the principal components. To do so, I complete the following steps:

Initialized the K-means model with four clusters by using the best value for k.

Fit the K-means model by using the PCA data.

Predicted the clusters for grouping the cryptocurrencies by using the PCA data. Reviewed the resulting array of cluster values.

Created a copy of the DataFrame with the PCA data, and then added a new column to store the predicted clusters.

Using hvPlot, created a scatter plot by setting x="PC1" and y="PC2". Colored the graph points with the labels that you found by using K-means. Then added the crypto name to the 'hover_cols' parameter to identify the represented by each data point.

Visualize and Compare the Results
In this section, I visually analyzed the cluster analysis results by observing the outcome both with and without the use of optimization techniques. To do so, I completed the following steps:

Created a composite plot by using hvPlot and the plus sign (+) operator to compare the elbow curve that you created from the original data with the one that you created from the PCA data.

Created a composite plot by using hvPlot and the plus (+) operator to compare the cryptocurrency clusters that resulted from using the original data with those that resulted from the PCA data.

Answered the following question: Based on visually analyzing the cluster analysis results, what’s the impact of using fewer features to cluster the data by using K-means?
