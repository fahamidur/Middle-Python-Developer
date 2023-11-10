# Project Documentation

## Overview

This project consists of three tasks, each located in its respective folder:

1. **Task 1: MNIST Image Classification**
   - Task1/mnist_classification.py

2. **Task 2: SQLite Library Management**
   - Task2/database.ipynb (Jupyter Notebook version)

3. **Task 3: Google Sheets Data Manipulation**
   - Task3/google_sheets_manipulation.ipynb (Jupyter Notebook version)

The purpose of this documentation is to provide comprehensive information on each task, including installation instructions, usage guidelines, and an overview of the code.


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



# Task 3: Google Sheets Data Manipulation

This code interacts with a Google Sheet using the `gspread` library to retrieve, update, and clear data.

## Installation

Ensure you have the `gspread` library installed:

```bash
pip install gspread
```

You'll also need a `service_account.json` file. Follow the instructions [here](https://docs.gspread.org/en/latest/oauth2.html) to obtain this file.

## Usage

1. Clone the repository:

```bash
git clone https://github.com/yourusername/yourrepository.git
```

2. Navigate to the Task3 directory:

```bash
cd yourrepository/Task3
```

3. Place your `service_account.json` file in the Task3 directory.

4. Run the code:



## Code Overview

The code uses the `gspread` library to interact with a Google Sheet named "myInfo." It performs the following operations:

### 1. Open Google Sheet and Retrieve Data

- Opens the "myInfo" Google Sheet using the provided `service_account.json` file.
- Retrieves all information from the first sheet and prints it.

### 2. Update Cells E1 and E2

- Updates the content of cells E1 and E2 with new values.
- Retrieves and prints the updated information.

### 3. Clear Updated Cells

- Clears the content of cells E1 and E2.
- Retrieves and prints the cleared information.

## Output

The output will demonstrate the retrieved, updated, and cleared information from the Google Sheet.

## Additional Notes

- Ensure that the Google Sheet has the appropriate permissions for the service account associated with `service_account.json`.

- Modify the code as needed for your specific Google Sheet structure and data.


Feel free to explore and modify the codes for your specific needs!























































## Task 1: MNIST Image Classification

### Installation

Ensure you have TensorFlow installed:

```bash
pip install tensorflow
```

### Usage

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

### Code Overview

- **Load and Preprocess Data:** Load and preprocess the MNIST dataset.
- **Build Neural Network:** Construct a Convolutional Neural Network (CNN) for image classification.
- **Compile the Model:** Compile the model with the Adam optimizer, categorical crossentropy loss, and accuracy metric.
- **Define Callback:** Log training metrics to a CSV file (`mnist_training_log.csv`).
- **Train the Model:** Train the model on the training data with a validation split of 20%.
- **Evaluate the Model:** Evaluate the trained model on the test data.

### Output

Test accuracy and loss will be printed at the end of the script execution.

### Additional Notes

- The `mnist_training_log.csv` file contains training metrics for each epoch.
- Adjust parameters such as epochs, batch size, or model architecture for experimentation.

## Task 2: SQLite Library Management

### Installation

No additional libraries are required. SQLite is included in the Python standard library.

### Usage

1. Clone the repository:

```bash
git clone https://github.com/yourusername/yourrepository.git
```

2. Navigate to the Task2 directory:

```bash
cd yourrepository/Task2
```

3. Run the code:

```bash
python library_management.py
```

### Code Overview

- **Connect to SQLite Database:** Connect to or create an SQLite database and define Authors and Books tables.
- **Functions for Database Operations:**
  - `add_author(name, birth_date)`: Adds an author to the Authors table.
  - `add_book(title, published_date, author_id)`: Adds a book to the Books table.
  - `get_books_by_author(author_id)`: Retrieves all books by a specific author.
  - `update_book(book_id, title, published_date)`: Updates book information.
  - `delete_book(book_id)`: Deletes a book.
- **Example Usage:** Example of adding an author, adding a book, retrieving books by an author, updating book information, and deleting a book.

### Output

The output will demonstrate example usage, including retrieving and updating book information.

### Additional Notes

- Adapt the code for more complex scenarios or additional features.
- Ensure proper error handling and validation for a production environment.

## Task 3: Google Sheets Data Manipulation

### Installation

Ensure you have the `gspread` library installed:

```bash
pip install gspread
```

### Usage

1. Clone the repository:

```bash
git clone https://github.com/yourusername/yourrepository.git
```

2. Navigate to the Task3 directory:

```bash
cd yourrepository/Task3
```

3. Place your `service_account.json` file in the Task3 directory.

4. Run the code:

```bash
python google_sheets_manipulation.py
```

### Code Overview

- **Open Google Sheet and Retrieve Data:** Open the "myInfo" Google Sheet and retrieve all information.
- **Update Cells E1 and E2:** Update the content of cells E1 and E2 with new values.
- **Clear Updated Cells:** Clear the content of cells E1 and E2.

### Output

The output will demonstrate retrieved, updated, and cleared information from the Google Sheet.

### Additional Notes

- Ensure the Google Sheet has the appropriate permissions for the service account.
- Modify the code for your specific Google Sheet structure and data.

Feel free to explore, modify, and experiment with the provided code for your specific needs!