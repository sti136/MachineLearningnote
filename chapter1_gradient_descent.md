## Gradient descent
It is to change the value the theta 0 and theta 1 in order to reduce J (theta 0,theta1)

![Cost function](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/bn9SyaDIEeav5QpTGIv-Pg_0d06dca3d225f3de8b5a4a7e92254153_Screenshot-2016-11-01-23.48.26.png?expiry=1592006400000&hmac=pYhwaUgqk7YC7sJ1dHhB-8INeydYVYlT-nfsWSJsL4E)
![Cost function](https://2.bp.blogspot.com/-AdV-O-MoZHE/TtLibFTaf9I/AAAAAAAAAVM/aOxUGP7zl98/s1600/gradient+descent+algorithm+OLS.png)
- slope at that point is to give the direction of the next "step"
- alpha : it is the learning rate, the bigger the alpha, the larger the "step"
if the alpha is small, the process is slow;If the alpha is large, the process is too fast that it may miss the minimum and become diverge.
![update](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/yr-D1aDMEeai9RKvXdDYag_627e5ab52d5ff941c0fcc741c2b162a0_Screenshot-2016-11-02-00.19.56.png?expiry=1592006400000&hmac=rOi1NQtsOHZis3z9XUck5v6xS4oBe_j4i7HvHHSaVbE)
- update it simultaneously means you need to update the parameters together in each loop
1. calulate the new value of each theta with reference to the old set of theta
2. update each theta with their new value correspondingly

