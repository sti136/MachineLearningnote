## Kernel
so given x ,we approxmately draw landmark(i) to present the predict

Kernel means the simliarty of x and landmark.

The equation is:
```
exp((x-li)^2/2/sigma^2)*-1

```

![](picture/ch7_10.png)
the graph below is proven that kernel will be 0 if x and l is not simliar and othervise.
![](picture/ch7_11.png)
The kernel we use is called <b>Guassian Kernel</b> 
![](picture/ch7_12.png)
As same as the graph below, we need to predict 1 when 

theta0 + theta1 f1+ theta2f2 + theta3f3 >= 0

through subsitution , we can circle the boundary which can draw some non-linear classifer.
![](picture/ch7_13.png)
we can express f in term of vector and the number of row of l should be equals to number of row of x
![](picture/ch7_14.png)
then we sub l to x in training and note that the summation of theta^2 is equals to theta^t * theta.
But we can use function like func() so don't worry about the math
![](picture/ch7_15.png)
What we should worry about is the SVM parameter

Larger C will leads to low bia, high variance,vice versa

Largr simgma^2 will leads to higher bias.and lower variance,vice versa.
![](picture/ch7_16.png)

## Using the SVM
We can use the software package, instead of build the SVM from scretch

we need to first choose the parameter C and the kernel

We can choose linear kernel,which means no kernel and SVM forms linear boundary 
![](picture/ch7_17.jpeg)
remember to do feature feature scaling
![](picture/ch7_18.jpeg)
beside Gaussian, it will have plenty of kernels(e.g:ploybomial) but it needs to satisfy Mercer's Theorem
![](picture/ch7_19.jpeg)
SVM packages already have bulti multi-class classification,if not you can use one-vs-all method to train K SVMs
![](picture/ch7_20.jpeg)
So, when to use those algos?
```
If n is large relative to m),then use logistic regression
If n is small and m is intermate, then use SVM withGaussian kernel
If n is small and m is large, use logistic regression or SVM without a kernel
```
![](picture/ch7_21.jpeg)