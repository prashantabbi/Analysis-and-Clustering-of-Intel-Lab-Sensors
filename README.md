# Analysis-and-Clustering-of-Intel-Lab-Sensors
The data used in this chapter is collected from an Intel repository, consisting of the details of 54 MicaDot2 sensors installed within the Intel Berkeley laboratory between the 28th of February and the 5th of April, 2004. The entire lab environment was planned precisely with coordinates and setups for each of the 54 sensors within the lab. These sensors collected dynamic environment variables like humidity and the temperature of the surrounding, the incident light and sensor voltage values, and recorded these values every 31 seconds. This resulted in recording 2.3 million readings in total.

K-means clustering is a widely used clustering technique attempting to find a certain number of clusters (k), as specified by the user, which are represented by their centroids. It is an unsupervised learning algorithm, meaning that it trains and learns from the data without receiving labels or assumptions. The number of clusters were determined using the K-Elbow Visualizer method. The K-Elbow Visualizer utilizes the elbow method for suggesting the best possible number of clusters for K-means clustering. The elbow method is used to check for the K-means clustering  algorithm for various values of K, and computes a mean score for all clusters for every value of K. Additionally, the distortion score is accordingly computed which is the value of the sum of square distances from each data point to the cluster centre. When the metrics for every model are consolidated and plotted, it's possible to visually conclude the optimal value of k. The point of inflection plotted is the best value of K if the road chart seems to be an arm. In the case when the arm is either up or down and there's a robust inflection point, it's an indication that the underlying model is deemed the best fit at that time.

The value of k at the point after which the distortion/inertia start decreasing in a linear fashion (‘elbow’) gives the best possible number of clusters to be formed. Thus, for the given data, the optimum k value was 3. Hence, 3 clusters were formed containing the sensor readings. On applying the model on the dataset, the clusters were formed and the corresponding labels were mentioned for each reading, for ease of classification using the KNN Classification algorithm.

__K Means METRICS__  
Silhouette Average - 94.58%  
Inertia - 5.378  

__KNN METRICS__  
f1 score - 97%
