# prodigy_ml_02

## Step 1: Importing the Libraries
We import the requisite libraries:
1. pandas for data manipulation.
2. numpy for numerical computations.
3. matplotlib.pyplot for data visualization.
4. KMeans from sklearn.cluster for performing the K-Means clustering algorithm.
   
## Step 2: Loading the Dataset
We load the dataset from a specified URL, which contains information about various customers, including their annual income and spending score. We utilize the pd.read_csv function from the pandas library to read the dataset. To understand the structure of the dataset, we display the first few rows using the head method.

## Step 3: Extracting Features for Clustering
We focus on two specific features for clustering: 'Annual Income (k$)' and 'Spending Score (1-100)'. These features are extracted using the iloc method from the pandas DataFrame and converted into a NumPy array for further processing.

## Step 4: Using the Elbow Method to Find the Optimal Number of Clusters
To determine the optimal number of clusters, we employ the Elbow Method. This involves calculating the within-cluster sum of squares (WCSS) for various numbers of clusters, ranging from 1 to 10. The WCSS values are stored in a list and plotted against the number of clusters.

## Step 5: Plotting the Elbow Graph
The WCSS values are plotted to visualize the Elbow Graph. The point where the curve bends (resembling an elbow) suggests the optimal number of clusters.

## Step 6: Applying K-Means Clustering with the Optimal Number of Clusters
Based on the Elbow Graph, we decide on the optimal number of clusters, which is 5. We then apply K-Means clustering with 5 clusters. The fit_predict method is used to fit the model and predict the cluster labels for each data point, which are stored in the y_kmeans variable.

## Step 7: Visualizing the Clusters
Finally, we visualize the clusters using a scatter plot. Each cluster is represented by a different color. The centroids of the clusters are highlighted in yellow. Labels for the axes and a legend are added to enhance the plot's readability.

Through these steps, we have successfully applied K-Means clustering to segment the customers into five distinct groups based on their annual income and spending score. This clustering provides valuable insights that can be leveraged for targeted marketing and customer relationship management.
