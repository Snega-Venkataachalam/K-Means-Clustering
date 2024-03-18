## Introduction

[K-Means Clustering](https://wikipedia.org/wiki/K-means_clustering) is a method derived from the domain of signal processing. It is used to divide and partition groups of data into 'k' clusters using a series of observations. Each observation works to group a given datapoint closest to its nearest 'mean', or the center point of a cluster.
The K-Means clustering process [executes in a three-step process](https://scikit-learn.org/stable/modules/clustering.html#k-means):

1. The algorithm selects k-number of center points by sampling from the dataset. After this, it loops:
    1. It assigns each sample to the nearest centroid.
    2. It creates new centroids by taking the mean value of all of the samples assigned to the previous centroids.
    3. Then, it calculates the difference between the new and old centroids and repeats until the centroids are stabilized.

One drawback of using K-Means includes the fact that you will need to establish 'k', that is the number of centroids. Fortunately the  'elbow method' helps to estimate a good starting value for 'k'. You'll try it in a minute.
