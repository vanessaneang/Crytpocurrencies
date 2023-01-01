# Crytpocurrencies

## Project Overview
For this module we utilized unsupervised machine learning to analyze the cryptocurrency market, first we processed the data, clustered the differenct cryptocurenncies, reduced the dimensions and PCA of the data. Then using 3D scatterplots and 2D.hvplots we visualized the spread of the various tradable cryptocurrencies. 

## Results
In order to begin working on the unsuperivsed machine learning model, we needed to preporess the data for PCA, we filtered the dataframe to include only tradable currencies that were being mined. Then we continued to use the StandardScaler to fit and transform the dataframe to further be used in the PCA.

Since the cryptocurrency data set is rather large we needed to reduce the data demension with PCA, 3 principal components were used to create the PCA dataframe.

Next with this new PCA dataframe we needed to cluster the cryptocurrencies using K-means. First we found the best value for k using the Elbow Curve, k=4 was the most optimal for running the prediction models.

Finally we created a 3D-Scatter with the clusters predicted from the previous steps and created a table to display the tradable cryptocurriencies with the funciton hvplot.table(). XFrom this we found that there are 532 tradable cryptocurrencies that are avaiable.

Lastly to confirm the results another scatter plot was created with scaled data that was fitted and transformed with the MixMinScaler() function. This gives a smaller subset of data points that allows the users to see what the TotalCoinSupply and TotalCoinsMined are based on the four classes we clustered the data into previously.
