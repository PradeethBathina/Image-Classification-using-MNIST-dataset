# Image-Classification-using-MNIST-dataset

First we loaded the mnist dataset using load_data().
Using pyplot, We diplayed the test images. Then we changed the image shape, converted data to float and scaled the data.
We then changed the labels frominteger to one-hot encoding
We then applied Sequential model with 'relu' activation for input and 'softmax' activation for output.
Using optimizer as 'rmsprop' and loss funtion as 'categorical_crossentropy, we fit and evaluate the model and found the accuracy as 41.7%
Using same Sequential model but changing the activation function to tanh, we found the accuracy as 41.9% upon evaluation of model.
Similarly, Using Sequential model with elu activation function achieved 42.26% accuracy.
Using the history object, we did plot training and validation loss & training and validation accuracy.
We then skipped the scaling of data to fit the sequential model and found the accuracy as 42.17% which seems to be stable.
Now we implemented the Functional API with input and hidden layer activation functions as relu and output activation function as linear.
Using rmsprop optimizer and 'mse' as loss we found the accuracy as 42.2%. We also did observed the same functional API getting 90% accuracy with 'adam' optimizer,
We finally plotted one of the test image( letter 5) and did inferencing to predict the class which appears to be 5.
