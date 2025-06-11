### Getting started with PyTorch Workflow code 
##### **video Timestamp :** **4:20:14 - 4:27:28**


1. *Data( Preparing and loading)*
2.*Build Model*
3.*Fitting the modle to data*
4.*making predictions and evaluting a model(inferences)*
5.*Saving and loading*
6.*Putting it all togehter*

### Creating a simple data set using linear regression
##### **video Timestamp :** **4:27:29 - 4:37:10**
*
    *data can be anything ... in machine learning*
    - $Excel/Spreadsheet$
    - $Images$
    - $Video$
    - $DNA Sequences$
    - $Text$
*
    *Machine learning is mostly about two things:*

    **1. Get data in numerical representation**
    **2. Build a modle to learn patterns in that numerical representation** 

### Spliting data into test and training sets (and using data visiulation)
##### **video Timestamp :** **4:37:10 - 4:52:18**


*
    *A machine learning model must be able to perform well on data it hadn't seen before.*


### Creating a model for linear regression
##### **video Timestamp :** **4:53:18 - 5:07:28**

*
    *We'll Build a Linear regression model using Pytorch*
*
    *Linear Regression is easy. It uses the formula y=mx+c*

*
    *How will our model work :*
    *1. Start with random values*
    *2. Look at training data and adjust the random values to better represents the data (or close to) ideal values.*

*
    *It'll do so using two main algorithm*
    1. Gradient Desent
    2. Backpropagation

*
    *Forward method is important as it is the operation that is performed at each computation/call*

### PyTorch model building essentials 
##### **video Timestamp :** **5:13:40 - 5:20:08**
*
    *torch.nn - contains all the building blocks for neural network*
*
    *torch.nn.Parameter - What parameter should our model try and learn, generally from a PyTorch layer from torch.nn*
*
    *torch.nn.Module - The base class for all neural network modules if you subclass it, you should override forward()*

*
    *torch.optim - This is a optimisers rhat helps in gradient descent*


### Checking internals of PyTorch Module
##### **video Timestamp :** **5:20:09 - 5:30:01**

*   
    *Model has random value*