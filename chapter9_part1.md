## Anomaly detection
We have trained a model with a cluster.But sometime the new example will lie out of the cluster we train. So we call it anomaly. But now to determine the example is anomaly or not?
![](picture/ch9_1.jpeg)
If the model p(x) calculate the new example is smaller than a threshold sigma, we will call it anomaly, othervise we will call it ok
![](picture/ch9_2.jpeg)
The anomaly detection will use in fraud detection/Manufactering.monitoring computers in a data centre.
![](picture/ch9_3.jpeg)
## Gaussian Distribution
It is a brief introduction of normal distribution.

This function has 2 variables mu and sigma. mu is the mean of this distribution and sigma^2 is the variance of this distribution. The formula of this distribution is in below(no need to memorise) 
![](picture/ch9_4.jpg)
How does to the graph when changing the parameters?

If the value of sigma become smaller. the crest of the distribution is become narrow.

The value of the mu is the centre of the distribution
![](picture/ch9_5.jpg)
How to apply to machine learning?

mu is the mean of those example.

sigma^2 is the variance of those example.

![](picture/ch9_6.jpg)