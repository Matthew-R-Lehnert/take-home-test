# Deep Neural Networks in R (Course Outline)
## Course Marketing Description
Deep Neural Networks (DNNs) are working behind the scenes of your everyday life. From recommeding products for you to buy, classifying your favorite cat pictures, forecasting the weather, to predicting tomorrow's stock prices, DNNs are only getting more powerful. With RStudio's creation of the Keras package it is now possible to deploy powerful DNNs within R. After a broad discussion of DNNs, this course will introduce you to the basic layered architecture of Keras and teach you to build different models for classification and regression problems.
## Course Learning Objectives
* Learner will be able to modify datasets into train/test/validation sets
* Learner will be able to differentiate classification and regression problems
* Learner will be able to construct neural network models for both classification and regression within Keras
### Chapter 1 - Introduction to Deep Neural Networks
#### Lesson 1.1 - What are Deep Neural Networks?
* Learner will be able to identify use cases where Deep Learning is a better candidate compared to parametric methods and other machine learning algorithms
#### Lesson 1.2 - Introduction to Layers in Keras
* Learner will be able to recall the steps of build and compile
* Some functions introduced/used:`%>%`,`keras_model_sequential()`, `layer_dense()`, `compile()`
#### Lesson 1.3 - Build Your First Model!
* Learner will be able to recall the steps of fit, predict, and evaluate
* Some functions introduced/used: `fit()`, `predict_classes()`, `evaluate()`
### Chapter 2 - Classification with Deep Neural Networks
#### Lesson 2.1 - What is Classification again?
* Learner will be able to differentiate classification and regression problems
#### Lesson 2.2 - Binary Classification
* Learner will be able to modify datasets into train/test/validation sets
* Learner will be able to identify appropriate activation function for output layer of binary classification problem
* Some functions introduced/used: `%<-%`, `%>%`,`keras_model_sequential()`, `layer_dense()`, `compile()`,`fit()`, `predict_classes()`, `evaluate()`
#### Lesson 2.3 - Multi-Label Classification 
* Learner will be able to modify datasets into train/test/validation sets
* Learner will be able to identify appropriate activation function for output layer of multi-label classification problem
* Some functions introduced/used: `%<-%`, `%>%`,`keras_model_sequential()`, `layer_dense()`, `compile()`,`fit()`, `predict_classes()`, `evaluate()`
#### Lesson 2.4 - Can We Make These Classification Models Better?
* Learner will be able to modify tuning parameters such as epochs, learning rate, and dropout rate in order to improve model performance
* Learner will be able to integrate early stopping to improve training time
* Some functions introduced/used: `layer_dropout()`, `callback_early_stopping()` 
### Chapter 3 - Regression with Deep Neural Networks
#### Lesson 3.1 - What is Regression again?
* Learner will be able to differentiate classification and regression problems
#### Lesson 3.2 - Single Target Regression
* Learner will be able to modify datasets into train/test/validation sets
* Learner will be able to identify appropriate activation function for output layer of single target regression problem
* Some functions introduced/used: `%<-%`, `%>%`,`keras_model_sequential()`, `layer_dense()`, `compile()`,`fit()`, `predict()`, `evaluate()`
#### Lesson 3.3 - Multi Target Regression
* Learner will be able to modify datasets into train/test/validation sets
* Learner will be able to identify appropriate activation function for output layer of multi-target regression problem
* Some functions introduced/used: `%<-%`, `%>%`,`keras_model_sequential()`, `layer_dense()`, `compile()`,`fit()`, `predict()`, `evaluate()`
#### Lesson 3.4 - Can We Make These Regression Models Better?
* Learner will be able to modify tuning parameters such as epochs, learning rate, and dropout rate in order to improve model performance
* * Learner will be able to integrate early stopping to improve training time
* Some functions introduced/used: `layer_dropout()`,`callback_early_stopping()` 
### Chapter 4 - Build Your Own Model
#### Lesson 4.1 - Build Your Own Classification Model!
* Learner will be able to construct neural network models for classification within Keras
* Some functions introduced/used: `%<-%`, `%>%`,`keras_model_sequential()`, `layer_dense()`, `compile()`,`fit()`, `predict_classes()
#### Lesson 4.2 - Build Your Own Regression Model!
* Learner will be able to construct neural network models for regression within Keras
* Some functions introduced/used: `%<-%`, `%>%`,`keras_model_sequential()`, `layer_dense()`, `compile()`,`fit()`, `predict()
#### Lesson 4.3 - Let's Wrap Things Up
* Learner will be able to evaluate the model performance for both classification and regression
* Some functions introduced/used: `evaluate()`

