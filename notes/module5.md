# Module 5

clustering 
- segmentation 
- cluster : a group of objects that are similar to other objects in the cluster, and dissimilar to data points in other clusters 
- used for 
    - explotory data anlysis 
    - summary generation 
    - outlier detection 
    - finding duplicates in dataset 
    - pre-processing step 
- clustering algorithms 
    - partitioned-based clustering 
        - relatively efficient 
        - eg. k-means, k-median, fuzzy c-means 
    - hierarchical clustering 
        - produces trees of clusters 
        - eg. agglomerative, divisive 
    - density-based clustering 
        - produces arbitrary shaped clusters 
        - eg. DBSCAN 

k-means clustering  
- can group data unsupervised 
- k-means algorithm 
    - partitioning clustering 
    - k-means divides the data into non-overlapping subsets (clusters) without any cluster-internal structure 
    - objects within a cluster are very similar 
    - objects across different clusters are very different 
    - minimize intra-cluster distances 
    - maximize inter-cluster distances 
1. initialize k (centroids are placed randomly)
2. distance calculation 
3. assign each data point to closest centroid 
- error is the total distance of each point from its centroid (want to minimize error) 
4. compute the new centroids for each cluster; updated to be the mean for datapoints in its cluster 
5. repeat until centroid don't change 
- guaranteed to converge to a result, but may converge to a local optimum --> repeat with different initial centroids 

k-means 
- k-means accuracy 
    - external approach 
        - compare the clusters with the ground truth, if available (usually not because unsupervised learning)
    - internal approach 
        - average the distance between data points within a cluster 
- choosing k 
    - dependent on dataset 
    - run clustering across different values of k 
    - elbow point (rate of decrease sharply shifts)
- med and large sized databases (relative efficient)
- produce sphere-like clusters 
- needs number of clusters (k)