## Unsupervised Learning 
This chapter will introduce unsupervised learning.Comparing to supervised learning, we will not have y at all in unsupervised learning. We will use a pot to prpresent the training examples and we will use the clustering algoithm to group the cluster with simliar location together.

example of supervised learning:

![](picture/ch8_2.jpg)

example of unsupervised learning:

![](picture/ch8_1.png)

## K-means algoithm
K-means algoithm is one of the unsupervised algoithm.

We need to set the number of K cluster centroids at first. 
![](picture/ch8_3.png)

then you can see the red centroid will calculate the mean of the red region anf the blue centroid will calculate the mean of blue region and move the centroid until it can move in the middle of the clusters and stop moving in next iteration.

![](picture/ch8_3.jpg)

Parameter you need to know in this algoithm:

![](picture/ch8_4.png)

To implement the algoithm:
1. determine the number of k
2. assign the index of cluster to every training example x(with the closest distance from cluster to x)
3. calculate the mean of the every cluster
4. repeat the process until the point don't "move" in a iteration

![](picture/ch8_5.png)

Just a sweet reminder from lecturer, some of the case may not be as perfect as that you can see the clear clusters but we can still classify clusters in the algoithm.
![](picture/ch8_6.png)
## Optimization Objective
knoeing the objective have 2 purposes
1.it can help us to debug 
2.to prevent strucking on local optima

so the optimization objective is to minize the distance between cluster centroid and all its corresponding points

![](picture/ch8_7.jpeg)

K-means algoithm 
1. randomly initialize k cluster controids
2. to assign x to the cluster centroids
3. to move centroid

![](picture/ch8_8.jpeg)
## Random initialization
The random initia;ization is to pick random K examples and assign it to the cluster centroids

![](picture/ch8_9.jpeg)
local optima means the crntroids sometimes can not as perfect as we want. It may struck at the same cluster

![](picture/ch8_10.jpeg)
How to solve local optima?

We do the process so many times (100 times) and pick the clustering that give the lowest cost
![](picture/ch8_11.jpeg)
## Choosing the Number of Clusters
How to choose the number of clusters?
1. the cost function with different K, then find the elbow.
but elbow sometime is not sharp if the graph is quadratic
![](picture/ch8_12.jpeg)

Sometime you may have some specific value of K for example you need to have 3 cluster to classify the S , M ,L 
3 sizes of clothes respectively.
![](picture/ch8_13.jpeg)
## Dimensionality Reduction
## 1. Data Compression
Sometime , in order to keeps the algoithm run faster and reduce some features, we will use data compression.

For example, if you see two features are redundant or two features can combine it to form another new features. then you may need to compress your data
![](picture/ch8_14.jpeg)
the compressed results calls z in the exampleand lies on a new dimensions
![](picture/ch8_15.jpeg)
Here is the examples compressed from 3d to 2d.
![](picture/ch8_16.jpeg)

## 2. Data Visualization
This parts aims to reduce the feature until we can draw graphs with those features(2d & 3d) 
In this example you need to reduce the features to 2d or 3d as we can not plot graphs with 50 features
![](picture/ch8_18.jpeg)
the result like this
![](picture/ch8_17.jpeg)
graph like this
![](picture/ch8_19.jpeg)
## Principal Componont Analysis
PCA is an algoithm of Dimensionality Reduction
1. draw a line(a pair of vector)
2. minimize the perpendicular distance of each point to the line

![](picture/ch8_20.png)
If it is reduce from n to k dimension, you must have k vector with k dimension 
![](picture/ch8_21.png)
The main difference pf PCA and linear regression is that PCA is minimizing the perpendcular distance and linear regression is to minimize the vertical distance of the point to the line
![](picture/ch8_22.png)

## Reconstruction from Compressed Representation
We havew talked about the compression , to reconstruction from the compression 
```
x_approxiate = U_reduce * z
```

![](picture/ch8_23.jpeg)