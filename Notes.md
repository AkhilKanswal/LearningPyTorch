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

##
##### **Creating Random Tensors zeros and one tensor and tensor datatype**


##### **video Timestamp :** ** 1:35:30 - 2:11:48*


*
    *Random Tensors are important because the way many neural networks learn is that they start with random numbersand then adjust those random numbers to better represent the data*

*
    *We can create zero and one tensor using torch.zeros and torch.ones*
*
    *We can also create a range tensor using torch.arange(start_index , end_index, step_ifRequired)*

*
    *we can create a tensor of another type similar to arange using _like()*
    - Example:  one_to_ten= torch.arange(1,11)

    another_tenor=torch.ones_like(one_to_ten)

*
    *default datatype of a tensor is float32*

*   
    *Some ther types are:*
    - $float16$ 
    - $float64$ 
    - $int32$ 
    - $int64$ 
    - $int16$ 

    *The number bascially represents presion in calculation of numbers*

***
### Tensor Issues
    *Tensors have biggest 3 issues causing errors which are as follow:*

    1. Tensors Not Right DataType - to get datatype we'll torch.datatype
    2. Tensors Not Right Shape - to get shape we'll torch.shape
    3. Tensors Not on Right Device - to get device we'll torch.device

***


##### **Tensor Operations**

##### **video Timestamp :** ** 2:11:49 - 2:17:48*

*
    *Tensor Operations include:*
    - $Addition$
    - $Substraction$
    - $multiplication (element -wise)$
    - $Division$
    - $Matrix Multiplication$

*
    *We can also uese inbuilt torch functions such as torch.add, torch.substract, torch.mul, torch.matmul etc*


##### **Matrix Multiplication**

##### **video Timestamp :** **2:17:48 - 2:34:59*
*
    *We'll use troch.mul() for element wise matrix multiplication*
*
    *Rules of Matrix Multiplications*

    - The Inner dimensions must match
        * example: (3,2) and (3,2) won't match but (3,2) and (2,3) will work
    - The resulting matrix is of **outer dimensions**
        * exapmle:  (3,3) and (3,2) => (3,2), (3,2) and (2,3) => (3,3)


##### **Matrix Multiplication(dealin with shape errors)**

##### **video Timestamp :** **2:35:18 - 2:48:15*

*
    *Its common to run into shape errors, to fix tensor shape issues, we'll use **Transpose** of a matrix(tensor)*

*
    *Transpose is changin g rows to column and column into rows **OR** It switches the axis or dimensions of a tensor*

*
    *Transpose can be used using  **.T** *

*
    **Example: tensor_B.T**

##### **Tensor aggeration i.e., finding min,max,mean, sum etc.**

##### **video Timestamp :** **2:48:17 - 2:54:28*

*
    *To find max well use torch.max(Definedtensor) & Definedtensor.max*
*
    *To find min well use torch.min(Definedtensor) & Definedtensor.min*
*
    *To find mean of tensor well use torch.mean(Definedtensor)*

*
    *we can convert the data type of tensor using x.type(torch.float32) or any other type*


##### **Finding positional min and max of tensors**

##### **video Timestamp :** **2:54:28 - 2:57:45*

*
    *To find the positional min and max of a tensor we'll argmin() and argmax() and returns the index*

##### **Reshaping, reviewing and stacking tensors**

##### **video Timestamp :** **2:57:50 - 3:11:28*
*
    ***Reshaping** - reshape an input tensor to a defined shape*
*
    *The reshaped dimensions must be comptable with the original shapes i.e., theiir size must match*

*
    ***View** - Return a view of an input tensor of a certain shape but keep the same memory as the original tensor*

*
    ***Stacking** - combine multiple tensore on top of each other (vstack) or side by side (hstack) **OR** concatinating tensors to a new dimensions.* 
*
    ***Squeeze** - removes all '1' dimensions from a tensor* 
*
   ***Unsqueeze** - adds all '1' dimensions from a tensor*
*
    ***Permute**-  Return a view of input with dimensions permuted/swapped in a certain way.*