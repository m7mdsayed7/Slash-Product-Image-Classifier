# Slash-Product-Image-Classifier
Image binary classification project:
The project goal is to create a convolutional deep neural network model to decide whether an image is a cloth or home decoration through dataset of photos brought from Slash application.
The steps of the process can be explained briefly through these ten steps:

1- Importing necessary libraries: To be able to plot and load our data,as well as, building our model. Some of the main libraries are matplotlib,numpy and tesnorflow.

2- Loading dataset and Removing any corrupted photos: this to remove any damaged photo with unknown extension.

3- Classifying the datasets into two classes using keras: this to load the dataset using keras to divide it into batches classifying photos into 0s and 1s.

4- Scaling the data: Data need to be scaled as it will be easier for computations. the highest value in the rgb is 255, so by dividing the array of values by 255 we ensure that the range of values will be between 0 and 1.

5-Splitting the data: Data is splitted by splitting the number of batches as there are 5 batches in the training model, 2 batches in the validation model and 1 batch in the test model. The train model has the biggest size of batches as higher the data trained gives higher probability of high accuracy results.

6-Building a Sequential deep learning model by 2D convolution: We can use a sequential model as it is a simple model that does not have multiple of inputs/outputs. 2D convolution used for the 2d images. Relu activation function is used to remove negative values making the model non-linear, and the sigmoid activation function is used to define the final output into 0s and 1s. Pooling is for reducing output shape so fewer calculations are made, and flatten to take down the neural network layers into a 1-dimensional matrix.

7- Training and validating the model: It is the step where the train values are fitted into the model. A history file is added to be able to trace back the training model.

8- Plotting the loss and accuracy performance: To ensure there is no overfitting and trace the performance of the model. Matplotlib library is used to plot the graphs.

9- Evaluation and testing: The step where we evaluate how accurate is the model through predicting the test data.

10- Testing through external data: This is an extra step to see how the model will classify external data. The image has to be resized and scaled to be tested.

11- Saving the model: It is vital to save the model to be able to process it later at any time.
