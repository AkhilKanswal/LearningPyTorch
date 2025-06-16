### Getting started with classifications problems and Input and Output shapes of classification problems
##### **video Timestamp :** **8:32:12 - 8:50:48**

*
    *Classification is a problem of predictiong weather something one thing or the other.*

*
    *Types of classification problems:*
    - $BinaryClassification$
    - $MulticlassClassification$
    - $MultilabelClassification$

*
    *Binary classification will solve problems where only two categories are conserned where as multiclass classification deals with more than two classes/categories*

*
    *Input shapes amy be different from output shapes deponding upon the problem. We are dealing with*

*
    *Inputs are generally numerical encoding and outputs are prediction probablities*

### Making a classification dataset
##### **video Timestamp :** **8:57:22 - 9:09:41**

*
    *The data we're working woth is referred to as toy dataset, adataset that is small enough for experiment and still sizeable enough to practice the funadamentals.*


### Making training and testing splits and building a model 
##### **video Timestamp :** **9:09:42 - 9:36:56**

*We'll build a model to classify red and blue dots Steps to do so are as follow :*

1. *Set up device agnostic code*
2. *Construct amodel using torch.nn.Module*
<br>
    *i. Subclass nn.Module*<br>
    *ii. Create 2 nn.Linear() layer that are capable of handling the shape of our data*<br>
    *iii. Defines a forward method() that outlines the forward pass of the model*<br>
    *iv. Instatiate an instance of our model class and send it to the target device* 
3. *Define loss functio and optimizeer*
4. *Creating a train and test loop*


### Making our neural network visible,Representing our model using torch.nn.Sequential,
##### **video Timestamp :** **9:36:57 - 9:57:10**

---
Only some code
---

### Setting up loss function, optimizer
##### **video Timestamp :** **9:57:12 - **

*
    *For problems like regression we will use MAE(Mean Absolute Error) or MSE(Mean squared Error)*

*
    *For classification we 'll use binary cross entropy or categorical cross entropy*