# Image-Classification-using-MNIST-dataset

1. First we loaded the mnist dataset using load_data().
2. Using pyplot, We diplayed the test images. Then we changed the image shape, converted data to float and scaled the data.
3. We then changed the labels frominteger to one-hot encoding
4. We then applied Sequential model with 'relu' activation for input and 'softmax' activation for output.
5. Using optimizer as 'rmsprop' and loss funtion as 'categorical_crossentropy, we fit and evaluate the model and found the accuracy as 41.7%
6. Using same Sequential model but changing the activation function to tanh, we found the accuracy as 41.9% upon evaluation of model.
7. Similarly, Using Sequential model with elu activation function achieved 42.26% accuracy.
8. Using the history object, we did plot training and validation loss & training and validation accuracy.
9. We then skipped the scaling of data to fit the sequential model and found the accuracy as 42.17% which seems to be stable.
10. Now we implemented the Functional API with input and hidden layer activation functions as relu and output activation function as linear.
11. Using rmsprop optimizer and 'mse' as loss we found the accuracy as 42.2%. We also did observed the same functional API getting 90% accuracy with 'adam' optimizer,
12. We finally plotted one of the test image( letter 5) and did inferencing to predict the class which appears to be 5.
