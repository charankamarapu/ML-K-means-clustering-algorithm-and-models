# ML-K-means-clustering-algorithm-and-models
### INTRODUCTION
K-Means Clustering is an Unsupervised Learning algorithm, which groups the unlabeled dataset into different clusters. Here K defines the number of pre-defined clusters that need to be created in the process, as if K=2, there will be two clusters, and for K=3, there will be three clusters, and so on.
- It is a centroid-based algorithm, where each cluster is associated with a centroid. The main aim of this algorithm is to minimize the sum of distances between the data point and their corresponding clusters.\

The k-means clustering algorithm mainly performs two tasks:
- Firstly randomly decide k centers .
- Assigns each data point to its closest k-center. Those data points which are near to the particular k-center, create a cluster.
- Find the centroid for each cluster and reapeat till it becomes stable.
- No of clusters can be decided by elbow 
- We iterate the values of k from 1 to 9 and calculate the values of distortions for each value of k and calculate the distortion and inertia for each value of k in the given range.
- Distortion: It is calculated as the average of the squared distances from the cluster centers of the respective clusters. Typically, the Euclidean distance metric is used.
- Inertia: It is the sum of squared distances of samples to their closest cluster center.
- if we plot wccs vs k  we will find an elbow which is our no of clusters.

![Screenshot (163)](https://user-images.githubusercontent.com/72094895/124958170-7a067a00-e037-11eb-827d-4c5312c65c11.png)
the algorithm works like below steps\
Here the "E-step" or "Expectation step" is so-named because it involves updating our expectation of which cluster each point belongs to. The "M-step" or "Maximization step" is so-named because it involves maximizing some fitness function that defines the location of the cluster centers

![Screenshot (164)](https://user-images.githubusercontent.com/72094895/124958905-4e37c400-e038-11eb-9cd6-4f9dccddd4d1.png)

### When should we use K-means clustering...?
- It should be used to find the clusters in the huge data set.

### PROS
- It can used for clustering.
- It can be used clasiification.
- It can be used colour image compression.
- It can be used for image segmentation.

### CONS
- k-means is limited to linear cluster boundaries , so we use neariest neighbour too in this algo.
- k-means can be slow for large numbers of samples
- clusters depend on the intializing positions of the centroids so,we use k-means++ to eliminate this.
