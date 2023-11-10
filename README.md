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










# Task 2: SQLite Library Management

This code provides a basic implementation of a library management system using SQLite for storing information about authors and books.

## Installation

No additional libraries are required. SQLite is included in the Python standard library.

## Usage

1. Clone the repository:

```bash
git clone https://github.com/yourusername/yourrepository.git
```

2. Navigate to the Task2 directory:

```bash
cd yourrepository/Task2
```

3. Run the code:



## Code Overview

### 1. Connect to SQLite Database

The code connects to an SQLite database named `library.db` (creates a new one if it doesn't exist) and defines two tables: Authors and Books.

### 2. Functions for Database Operations

- `add_author(name, birth_date)`: Adds an author to the Authors table.
- `add_book(title, published_date, author_id)`: Adds a book to the Books table.
- `get_books_by_author(author_id)`: Retrieves all books by a specific author.
- `update_book(book_id, title, published_date)`: Updates book information.
- `delete_book(book_id)`: Deletes a book.

### 3. Example Usage

The code includes an example of adding an author, adding a book, retrieving books by an author, updating book information, and deleting a book.

## Output

The output will demonstrate the example usage, including retrieving and updating book information.

## Additional Notes

- Feel free to adapt the code for more complex scenarios, such as adding additional tables or fields.

- Ensure proper error handling and validation for a production environment.

- The database connection is closed at the end of the script. In larger applications, consider using context managers (`with` statement) for better resource management.

Copy and paste this into your GitHub README file for comprehensive documentation for Task 2.