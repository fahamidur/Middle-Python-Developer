# Middle-Python-Developer
This repository contains the tasks provided to me via Email. 

Certainly! Here's the text formatted for a GitHub README:


# Task 1: MNIST Image Classification

This code is a simple neural network implementation using TensorFlow and Keras to classify handwritten digits from the MNIST dataset.

## Installation

Ensure you have TensorFlow installed:

```bash
pip install tensorflow
```

## Usage

1. Clone the repository:

```bash
git clone https://github.com/yourusername/yourrepository.git
```

2. Navigate to the Task1 directory:

```bash
cd yourrepository/Task1
```

3. Run the code:

```bash
python mnist_classification.py
```

## Code Overview

### 1. Load and Preprocess Data

The code loads the MNIST dataset, reshapes the images, and normalizes pixel values to the range [0, 1].

### 2. Build Neural Network

A Convolutional Neural Network (CNN) is constructed with three convolutional layers, max-pooling layers, and dense layers for classification.

### 3. Compile the Model

The model is compiled with the Adam optimizer, categorical crossentropy loss, and accuracy metric.

### 4. Define Callback

A CSVLogger callback is defined to log training metrics to a CSV file (`mnist_training_log.csv`).

### 5. Train the Model

The model is trained on the training data with a validation split of 20%, and the training metrics are logged to the CSV file.

### 6. Evaluate the Model

The trained model is evaluated on the test data, and the test accuracy and loss are printed.

## Output

The test accuracy and loss will be printed at the end of the script execution.

## Additional Notes

- The `mnist_training_log.csv` file contains training metrics such as loss and accuracy for each epoch.

- Adjust the number of epochs, batch size, or model architecture to experiment with different configurations.

Feel free to explore and modify the code for your specific needs!