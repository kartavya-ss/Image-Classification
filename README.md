**MNIST Digit Classification using TensorFlow/Keras**

This project implements a neural network to classify handwritten digits from the MNIST dataset using TensorFlow and Keras. The workflow includes data loading, preprocessing, model building, training, evaluation, and prediction.

**Project Overview**

•Loaded the MNIST dataset and visualized sample images

•Normalized the pixel values for faster and stable training

•Built a Sequential Neural Network consisting of:

•Flatten layer to convert images into vectors

•Dense layer with 128 neurons (ReLU activation)

•Dense layer with 32 neurons (ReLU activation)

•Output layer with 10 neurons (Softmax activation)

•Compiled the model using:

•Adam optimizer

•Sparse Categorical Crossentropy loss

•Accuracy as the evaluation metric

•Trained the model for 25 epochs using an 80-20 train/validation split

•Generated predictions for the test dataset and calculated the overall test accuracy

•Plotted training curves for loss and accuracy

•Performed a sample prediction on a single test image

 **Model Performance**

The model trains smoothly and produces strong test accuracy on the MNIST dataset.
Both training vs. validation loss and training vs. validation accuracy curves are plotted to visualize performance.

 **Sample Prediction Code**
 
 model.predict(X_test[1].reshape(1, 28, 28)).argmax(axis=1)

 **Technologies Used**

•Python

•TensorFlow / Keras

•NumPy

•Matplotlib

•Scikit-Learn
