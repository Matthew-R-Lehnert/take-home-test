# Build Your First Model! (Sample Exercise)
## Context
## Instructions
## Code (Scaffolded)
  #Instantiate a keras_model_sequential and assign it to dnn_binary_model
  dnn_binary_model <- keras_model_sequential %>%
                      layer_dense(units = 50,
                                  activation = 'relu',
                                  input_shape = c(ncol(X_train))) %>%
                      layer_dense(units = 50, activation = 'relu') %>%
                      layer_dense(units = 1, activation = 'sigmoid') %>
                      compile(optimizer = 'adam',
                              loss = 'binary_crossentropy',
                              metrics = c('accuracy'))
                      
                                  
## Code Solution
