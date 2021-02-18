# Build Your First Model! (Sample Exercise)

## Context
It's time to start building your first model!  In this exercise we will start the workflow of build, compile, fit, evaluate, and predict.  The first step is to build the sequential model with an input layer, hidden layers, and an output layer using the `keras_model_sequential` and `layer_dense` functions from `library(keras)`. Next, we will compile the model by choosing an optimizer, a loss function, and evaluation metrics.  Remember: the activation function in the output layer and the loss function are different depending on the problem at hand!

## Instructions
* Instantiate a sequential model in Keras using `keras_model_sequential` and assign it to `dnn_binary_model`
* Create the first dense layer with `50` units, `'relu'` activation, and use `ncol` to set the input shape equal to the number of columns in X_train
* Assign the appropriate activation function to the output layer (Look back at the slides on activation if you forgot!)
* Assign the appropriate loss function to the compile function (Look back at the slides on loss if you forgot!)

## Code (Scaffolded)
```
# Instantiate a keras_model_sequential and assign it to dnn_binary_model
dnn_binary_model <- ___ %>%
# Create the first dense layer with 50 units, relu activation, and an input shape equal to the number of columns in X_train
                    layer_dense(units = 50,
                                activation = 'relu',
                                input_shape = c(___(X_train))) %>%
                    layer_dense(units = 50, activation = 'relu') %>%
# Assign the appropriate activation function to the output layer
                    layer_dense(units = 1, activation = '___') %>
                    compile(optimizer = 'adam',
# Assign the appropriate loss function
                            loss = '___',
                            metrics = c('accuracy'))
```
                      
                                  
## Code Solution
```
# Instantiate a keras_model_sequential and assign it to dnn_binary_model
dnn_binary_model <- keras_model_sequential %>%
# Create the first dense layer with 50 units, relu activation, and an input shape equal to the number of columns in X_train
                    layer_dense(units = 50,
                                activation = 'relu',
                                input_shape = c(ncol(X_train))) %>%
                    layer_dense(units = 50, activation = 'relu') %>%
# Assign the appropriate activation function to the output layer
                    layer_dense(units = 1, activation = 'sigmoid') %>
                    compile(optimizer = 'adam',
# Assign the appropriate loss function
                            loss = 'binary_crossentropy',
                            metrics = c('accuracy'))
```
