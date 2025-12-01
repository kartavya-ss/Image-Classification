**MNIST Digit Classification using TensorFlow/Keras**

This project implements a neural network to classify handwritten digits from the MNIST dataset using TensorFlow and Keras. The workflow includes data loading, preprocessing, model building, training, evaluation, and prediction.

**Steps Performed**

1. **Data Loading & Visualization**

Loaded MNIST using keras.datasets.mnist

Displayed sample images using Matplotlib

2. **Preprocessing**

Normalized pixel values (0–255 → 0–1)

Prepared data for training and testing

3.**Model Architecture**

A Sequential Neural Network with:

Layer	Description
Flatten	Converts 28×28 image → 784-dim vector
Dense (128, ReLU)	Fully connected hidden layer
Dense (32, ReLU)	Second hidden layer
Dense (10, Softmax)	Output layer for digit classes

4. **Model Compilation**

Loss: Sparse Categorical Crossentropy

Optimizer: Adam

Metric: Accuracy

5. **Training**

Trained for 25 epochs

Used validation_split = 0.2

Tracked accuracy and loss throughout training

6. **Evaluation & Predictions**

Predicted on test dataset

Calculated test accuracy using accuracy_score

**Plotted:**

Training vs validation loss

Training vs validation accuracy


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
