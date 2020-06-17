## Neural Networks
Why we need the Neural Networks while we have linear regression and logistic regression?
Although those two regression is useful, but it is costly in computation when the number of feature is too large (>100)

![](picture/ch4_1.png)

In a neuron in the brain, it mainly consists of three part
Dendrite(input)wire, Nucleus(process unit),Axon(output)
![](picture/ch4_2.png)
In a Neuron model, it is as same as a logistic function with more than one layer.
![](picture/ch4_3.png)
In a Neural Network, the first layer called input layer,the final layer called output layer and the layer between two layers are hidden layer, a0 is the bias unit

![](picture/ch4_4.png)
the value of element in the second layer is calculated with same x but different value of theta ,then the output is also calculated as above. the dimension of theta is sj+1*(sj+1)
![](picture/ch4_5.png)
How to calulate the output with vectorized implementation?
1. caluate z1 = theta1 * a1
2. calculate a(2)= g(z2)
3. a0^2 = 1
4. calulate z2 = theta2 * a2
and loop until you find the output
