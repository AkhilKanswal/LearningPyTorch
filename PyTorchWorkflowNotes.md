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

### Making random predictions from modle_0 using torch.inference_mode()
##### **video Timestamp :** **5:30:02 - 5:41:15**

*
    *We'll make predictions from modle_0 using torch.inference_mode()*

*
    *inference_mode() helps as a context manager, it is used in making predictions without gradient descent. That means it automatically turnsoff the required_grad.*

*
    *we can also use torch.no_grad()*


### Training a model with PyTorch
##### **video Timestamp :** **5:41:16 - 5:49:29**
*
    *The whole idea of training for a model to from some **Unknown** parameters.In other words it;s about how can we better represents our data*

*
    *One way to measure how pooor our model predictions are we can user loss function*


    **Thins we need to train :**

*
    ***Loss Function** - A function to measure how wrong our model prediction are to ideal outputs*
*
    ***Optimizer :** Takes into account the loss af a model and adjusts the model's parameters(e.g., weight & bias) to improve the loss function*

*
    *We'll typically need :*
    -   $TrainingLoop$
    -   $TestingLoop$

### Setting Up loss function and optimiser
##### **video Timestamp :** **5:49:29 - 6:02:22**

*
    *MAE- Mean Absolute Error l1*
*
    *MSE - Mean Squared Error l2*

### PyTorch training loop
##### **video Timestamp :** **6:02:22 - 6:40:04**

**Steps for building a training loop and testing loop in PyTorch :**

*0. loop through the data*
*1. Forward pass / propagation - This involved data moving through our model's forward() function to make predictions on data*
*2.Calculate the loss - compare forward pass predictions to grounf truth labels*
*3.Optimizer zero grad*
*4.Loss backwards - moves backwards through network to calculate the gradients of each of the parameters of our model with respect to loss(**Back Propogation**)*
*5.Optimiser step - uses optimizer to adjust our model's parameters to try and improve the loss(**Gradient Descent**)*

*
    *Every model is in train mode by default*
*
    *\"train\" mode inPyTorch sets all parametrs that requires gradients to require gradients*