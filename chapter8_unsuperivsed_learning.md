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