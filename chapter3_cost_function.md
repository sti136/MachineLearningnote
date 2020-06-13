## Cost Function

![](picture/chapter3.5.png)
We take the cost function in lienar function and modify it to be logistic function as below
```
cost(h(x),y) = 1/2 (h(x)-y)^2
```
The cost function is said be convex if it is being used as logistic regression

![](picture/chapter3.6.png)
in the cost function, it has two function used if y = 1 or y = 0

if y = 1, h(x) = 0 , the cost function will be equals to inf(the cost is extremely high)
![](picture/chapter3.7.jpeg)
On the other hand, when y = 0, h(x) = 1 , the cost is also high, and the shape is came as above

## Apply gradient descent to simplified cost function

![](picture/chapter3.9.png)

- we use the new cost function as above to calculate logistic regression, the y = 0 part will be cancel out if y is equals to 1,vice versa.

![](picture/chapter3_10.png)

the algoithm is doing the iteration which is same as the linear regression, it is recommended to use vector to calculate each iteration in the programming assignment


