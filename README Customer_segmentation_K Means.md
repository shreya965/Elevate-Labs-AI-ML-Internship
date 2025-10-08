# Customer_Segmentation_Kmeans
Customer_Segmentation_Kmeans
This project demonstrates customer segmentation using the K-Means clustering algorithm. The goal is to divide customers based on their behaviors using data such as age, annual income, and spending score.

Project Steps
1. Importing the Data

The dataset used is the Mall_Customers.csv, which contains data about customers' age, annual income, and spending score.

2. Data Visualization

Visualize the relationships between Age, Annual Income (k$), and Spending Score (1-100) using pair plots to understand how the data points are distributed.

3. Data Cleaning and Standardization

The dataset is checked for missing values and then cleaned.

The continuous features (Age, Annual Income, and Spending Score) are standardized using StandardScaler to ensure fair clustering.

4. K-Means Clustering

K-Means clustering is applied to the standardized data to segment customers into clusters based on their behavior.

5. Elbow Method for Optimal K

The Elbow Method is used to determine the optimal number of clusters. This method calculates the inertia for different values of K and helps identify the "elbow" point that suggests the best K.

6. Visualizing Clusters

The clusters are visualized using Age and Annual Income (k$) to observe the segmentation.

Another visualization is created using Principal Component Analysis (PCA) to reduce the dimensions and show the clusters in 2D space.

7. Evaluating Clustering Quality

The Silhouette Score is calculated to evaluate how well the clusters are defined. A score close to 1 indicates well-separated clusters.

Conclusion

The K-Means algorithm effectively segments the customers, with the optimal number of clusters being 4, as determined by the Elbow Method. The Silhouette Score suggests that while the clustering is somewhat good, there is room for improvement in terms of separation between the clusters.
