##### **Introduction to Machine Learning**

##

##### **video Timestamp :** **02:36 - 07:15**



**Machine Learning :**

*
    *It is the process by which a machine or a computer program/algorithm learns pattern from the data which is converted to set of numbers*

*  
    *Machine learning is the subset of Artificial Intelligence and deep learning is the subset of Machine Learning*

##### **Reason of using Machine Learning and Deep Learning Algorithms :**

##

##### **video Timestamp :** **07:41 - 13:47**

*
    *Helps in determining rules for solving complex problems*
*
    *They helps when we need to have large set of rules*
*
    *We'll use deep learning where the algorithm can adapt to changes as they are applied to continiously changing envirnoment*
*
    *Discovering insights within large data sets*

*
    
    **Google's number 1 rule for ML : <br> if you don't need it don't use it**


##### **Cons of using Deep Learning (typically)**

##

##### **video Timestamp :** **13:48 - 16:50**


*
    *Deep Learning Models are non interpretable by humans*

*
    *Deep Learning Models are not used when we dont have adequate amount of data*


##### **Machine Learning vs Deep Learning**

##

##### **video Timestamp :** **16:51 - 23:00**

*
    *Ml is used with structured data and Dl is used with unstructured data*

*
    *Algorithms for Ml:*<br>
    *1. Random Forest*<br>
    *2. Naive bias*<br>
    *3. Nearest Neighbour*<br>
    *4. Support Vector Machine*<br>

*
    *Algorithms for Dl:*<br>
    *1. Neural networks*<br>
    *2. Fast Forward Neural Network*<br>
    *3. Recurrent Neural Network*<br>
    *4. Convoulational Neural Network*<br>

##### **Neural Networks**

##

##### **video Timestamp :** **23:00 - 32:23**

*
    *Neural Networks are network of perceptrons(an equivalent of a neuron of brain) where each neuron process the data it received from the other neuron perform some mathematical operation on the data called activation function.*

*
    *The data is generally numerical representation of data.*

*
    *There are input layer, output layer and some hidden layer.*

*
    *Activation functions are mathematical operations can be linear or non linear deponding upon the case*

*
    *The neural network learns the hidden feature/patterns/weight from the data*


##### **Types of Learning**

##

##### **video Timestamp :** **32:23 - 43:16**

*
    *There are following types of learning :*
    
    1. Supervised Learning
    2. Unsupervised Learning/ self supervised Learning
    3. Transfer Learning
    4. Reinforcement Learning



##### **Introduction to tensors**

##

##### **video Timestamp :** **53:33 - 1:03:34**

*
    *Tensors are mathematical representation of the data as simple as that for the time being .They are quiet complex as mathematical concepts but we'll only learn about them in context to pytorch*

##### $Basics of what we'll do from here as in the video$
1. Get the data ready(convet to tensors)
2. Build or pick a pre-trained model
    - pick a loss function and optimiser
    - build a training loop
3. Fit the data to the model make prediction.
4. Evaluate the model
5. Improve through expreimentation
6. Save and reload your trained model

##

###  Gettign started with code

##
##### **getting started with tensors with code**


##### **video Timestamp :** **1:24:46* - 1:35:30*

*
    *pytorch tensors are created using torch.tensor*
    - *it takes an argument i.e, the tensor has it's value*

    *ndim - is number of dimension of a tensor*

*
    *There are 4 types of tensors which are as follow:*

    - $Scalar$
    - $Vector$
    - $Matrix$
    - $Tensor$

*
    *Examples :*
    - Scalar : [7]
    - vector : [2,8]
    - Matrix : [[2,5],
                [9,6]]
    - Tensor : [[7,8],
                [9,5],
                [6,7],
                [4,3]]

