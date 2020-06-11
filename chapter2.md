 ## Multiple variables linear regression
 - linear regression with multiple varables

Notation
-
- x^i the input in ith training example
- m = the number of trsining example
- n = the number of multiable variable(features)

![](https://i.stack.imgur.com/TPOVM.png) 

note that x0 = 1 and we have n+1 terms as x from x0 to xn

## Gradient Descent for Multiple Variables

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/MYm8uqafEeaZoQ7hPZtKqg_c974c2e2953662e9578b38c7b04591ed_Screenshot-2016-11-09-09.07.04.png?expiry=1592006400000&hmac=b2jcEDdHKtAYEZFHVKd8VqrxvC03OVCiWu4GC1lWnis)

repeat until convergence:
{θj:= θj−α1/m∑i=1m(hθ(x(i))−y(i))⋅x(i)jfor j := 0...n}

## Practial skills

## Gradient Descent normalization and scaling

after normalization, the effiency of gradient descent will be faster

the normalization is to minus x with the mean and divide it with (max - min)

## Gradient Descent choose a learning rate
Two test to know the cost function is minimized correctly

1.Debugging gradient descent: to see the trend of cost function is decreasing not increasing.If it is increasing, you may use the smaller rate to fix it

2.Automatic convergence test: the iteration stop if the value of cost function descrease is smaller than 10^-3(threshold value), it is difficult to fina a good threshold value

two phenomemon of alpha(learning rate)
1. the learning will be slow if alpha is too small
2. the cost function will increase and not converge if the alpha is too large
## Abour the Feature and Polynomial regression
1. you can combine some features together to be a feature if needed
2. If you want a specific trend in your regression you can adjust it to square,cubic function if you want
3. but the range will be different through adjust and the value of normalization is different
