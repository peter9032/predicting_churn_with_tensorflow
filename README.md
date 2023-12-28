# Predicting Client Churn with TensorFlow

![image](https://github.com/peter9032/predicting_churn_with_tensorflow/assets/129965664/42a1a86a-77a2-4fb8-a5ba-88abb4b53df9)


Churn, the departure of customers from a product or service, is a critical business metric affecting revenue. This Jupyter Notebook explores predicting client churn using TensorFlow. The process involves loading the dataset, preprocessing, building, compiling, fitting, and predicting using a neural network model.

## 1. Loading the Dataset

The dataset is loaded using pandas, containing 7044 data points. After an initial exploration, it's observed that features like "Customer ID," "Total Charges," and "Monthly Charges" contribute to the dataset's size. Consequently, these features are removed, and the dataset is re-encoded, resulting in 43 features.

## 2. Building and Compiling

A neural network model is created using TensorFlow's Keras API. The model consists of three layers: the first layer with 32 neurons, ReLU activation, and L1 regularization; the second layer with 64 neurons, ReLU activation, and L2 regularization; and the output layer with a single neuron and a sigmoid activation function. The model is compiled for binary classification, using binary crossentropy loss, stochastic gradient descent (SGD) optimizer, and accuracy metric.

## 3. Fitting and Predicting

The model is trained on the training data for 100 epochs, with batch size 32. The training history, including accuracy and loss metrics, is visualized using matplotlib. The maximum accuracy achieved during training is approximately 79.9%. The model is then evaluated on the test set, yielding a validation score of 79.9%.

## 4. Saving and Reloading

The trained model is saved and reloaded for future predictions. An example prediction is demonstrated using a single observation from the dataset.

This notebook provides a comprehensive overview of predicting client churn, showcasing the entire process from data loading to model evaluation and future predictions.
