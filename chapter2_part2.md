## Normal equation
Normal equation is the new method of machine learning

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/dykma6dwEea3qApInhZCFg_333df5f11086fee19c4fb81bc34d5125_Screenshot-2016-11-10-10.06.16.png?expiry=1592092800000&hmac=HayVt_myTSrQy6M1nLRrirqt6eM18mhwYsWlrcjBenI)

Basically,it is just 2 steps to do:

1. idenitify what is X and Y martix is. X must be a (m * n+1) matrix, where m is number of feature and n is number of features. y is a m-dimension vectoral vector

2. calculate the (X^T*X)^-1 and calculate the theta by means of the formula on the pictures above

There is the comparison between Gradient Descent Method and Normal Equation

|parameter|Gradient Descent Method   | Normal Equation  |
|---|---|---|
|learning rate(alpha)|Need to use alpha|No need to use alpha|
| iteration   | need many iteration  |no need iteration|
| big O  | O(kn^2)  |O(n^3)|
|  speed |Works well when n is large   |Slow if n is very large
|
alogithm of determining the method(recommendation)

if (n >10000) then (choose iterative process)

## Normal Equation Noninvertibility(optional)

in normal equation,because it contains a inverse matrix (X^T*X)^-1 in its formula , some student ask that we may not calculate the theta if the inverse matrix is non - invertible (non-invertible means the inverse matrix cannot be calulated)

The answer is
```
No, is pinv() will help you to solve the theta even if it is non-invertible

```
To find out the root of the matrix is non- invertable

1. some features are dependent (which means redundent in training)

2. too many features (we need to delete it in regularzation)
