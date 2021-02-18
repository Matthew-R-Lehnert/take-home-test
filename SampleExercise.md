# Build Your First Model! (Sample Exercise)
## Context
## Instructions
* Instantiate a sequential model in Keras using `keras_model_sequential` and assign it to `dnn_binary_model`
* Create the first dense layer with `50` units, `'relu'` activation, and use `ncol` to set the input shape equal to the number of columns in X_train
* Assign the appropriate activation function to the output layer
* Assign the appropriate loss function to the compile function
## Code (Scaffolded)
```
#Instantiate a keras_model_sequential and assign it to dnn_binary_model
dnn_binary_model <- ___ %>%
#Create the first dense layer with 50 units, relu activation, and an input shape equal to the number of columns in X_train
                    layer_dense(units = 50,
                                activation = 'relu',
                                input_shape = c(___(X_train))) %>%
                    layer_dense(units = 50, activation = 'relu') %>%
#Assign the appropriate activation function to the output layer
                    layer_dense(units = 1, activation = '___') %>
                    compile(optimizer = 'adam',
#Assign the appropriate loss function
                            loss = '___',
                            metrics = c('accuracy'))
```
                      
                                  
## Code Solution
```
#Instantiate a keras_model_sequential and assign it to dnn_binary_model
dnn_binary_model <- keras_model_sequential %>%
#Create the first dense layer with 50 units, relu activation, and an input shape equal to the number of columns in X_train
                    layer_dense(units = 50,
                                activation = 'relu',
                                input_shape = c(ncol(X_train))) %>%
                    layer_dense(units = 50, activation = 'relu') %>%
#Assign the appropriate activation function to the output layer
                    layer_dense(units = 1, activation = 'sigmoid') %>
                    compile(optimizer = 'adam',
#Assign the appropriate loss function
                            loss = 'binary_crossentropy',
                            metrics = c('accuracy'))
```
