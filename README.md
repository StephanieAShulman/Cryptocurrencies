
# Cryptocurrencies
Using unsupervised machine learning to discover patterns in the data

![crypto](https://user-images.githubusercontent.com/30667001/163814093-7852c317-83a9-4d43-8921-7d60f8f94137.png)

### Resources
- Data Sources: crypto_data.csv
- Software: Python 3.7.6, Jupyter Notebook 6.4.5
- Libraries: Pandas, Scikit-learn, Plotly, hvPlot

### Project Overview
The influential investment bank Accountability Accounting plans to offer a new cryptocurrency investment portfolio to its customers. The group is interested in a classification system for existing currencies. The data, however, don’t lend themselves to the discrete categories that are needed in fitting a structured machine learning model. Rather, the qualitative nature of the data requires an unstructured approach. </br>

With a clustering algorithm decided upon, the following steps were taken: </br>
- Data were preprocessed with feature extraction and standardized for use in Principal Component Analysis.
- Cryptocurrency features (mined coins, supplied coins, algorithms for encryption and transaction validations) were reduced to three dimensions using PCA.
- The reduced dimensions were clustered into groups of similar means using K-means in order to determine patterns in the cryptocurrencies. </br>
  - Prior to running the algorithm, an elbow curve was created to find the best value for K when clustering data. </br>
  - A new data frame was created using coin names, feature data, cluster data and predicted class.
- Visualization was used to present the results with a 3D scatterplot of three clusters and an interactive hvplot of coins by class.

### Results
Elbow curve results indicated that running K-Means on four clusters would be sufficient. </br>
![crypto_elbow curve](https://user-images.githubusercontent.com/30667001/163815069-25b4e380-888d-4994-9e15-41fecd0d49eb.png) </br> </br> </br>
A 3D scatterplot displayed the groups corresponding with the four clusters into which the model was expected to parse the data. </br>
![crypto_pca](https://user-images.githubusercontent.com/30667001/163815093-1106c6dc-3ad9-437c-92cd-c265eb5ccde9.png) </br> </br> </br>
Data exploration of 532 tradable cryptocurrencies was made easier with an hvplot.</br>
![crypto_plothv](https://user-images.githubusercontent.com/30667001/163840678-cbcb0572-d869-47fa-b5d0-ff50b8bfa461.png)
