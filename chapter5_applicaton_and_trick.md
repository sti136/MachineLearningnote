## Unrolling the parameter
In the Nerual Network, we need to unroll the matrix to the one row vector in order to use optimizing functions such as "fminunc()"

```
thetaVector = [ Theta1(:); Theta2(:); Theta3(:); ]
deltaVector = [ D1(:); D2(:); D3(:) ]
```

if the dimensions of Theta1 is 10x11, Theta2 is 10x11 and Theta3 is 1x11, then we can get back our original matrices from the "unrolled" versions as follows:

```
Theta1 = reshape(thetaVector(1:110),10,11)
Theta2 = reshape(thetaVector(111:220),10,11)
Theta3 = reshape(thetaVector(221:231),1,11)
```
To summarize:

![](picture/ch5_7.png)

## Gradient Checking
In order to check the gradient descent is in the right direction, we can use gradient checking.
![](picture/ch5_8.jpg)
The code expression of gradient checking:
![](picture/ch5_9.jpg)
Some important notes of gradient checking: 
![](picture/ch5_10.jpg)
1. turn off gradient checking before training thr classifier or it will be very slow