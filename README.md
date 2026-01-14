Assignment 2: KMNIST Classification – Introduction to Machine Learning
This project was developed as part of the "Introduction to Machine Learning" course (January 2025). The primary goal is to build, train, and optimize a Deep Neural Network to classify characters from the Kuzushiji-MNIST (KMNIST) dataset.

📋 Project Overview
The project focuses on creating a robust Multi-Layer Perceptron (MLP) model. It includes a comprehensive pipeline for data preprocessing, hyperparameter tuning, and experiment tracking to achieve high accuracy while preventing overfitting.

🛠 Technologies & Libraries
The following tools and libraries were used:

PyTorch: Framework for building and training the neural network.

MLFlow: Used for experiment tracking, logging parameters, and monitoring metrics.

Scikit-Learn: For performance evaluation (Precision, Recall, F1-Score, Confusion Matrix).

Matplotlib: For visualizing training curves and data samples.

Torchinfo: For model architecture summarization.

🏗 Key Components
The code is structured into modular classes for better maintainability:

DataManager: Handles KMNIST data fetching, normalization, and splitting into Training, Validation, and Test sets.

MLPFromConfig: A dynamic model builder that constructs the network based on a configuration object (supports Linear layers, BatchNorm, Dropout, and various Activations).

Trainer: A robust training class that manages the training loop, SGD optimization, Mixed Precision (AMP) for speed, and logging to MLFlow.

EarlyStopping: A mechanism to monitor validation loss and stop training early to prevent overfitting.

🧪 Experiments and Results
Performed at least 10 different experiments with various architectures and hyperparameters.

All runs were logged and compared using MLFlow.

Performance: The final model achieved an accuracy range of 85% - 93% on the Test set.

A detailed Excel report is included in the repository, documenting the metrics (Precision, Recall, F1) for every experiment conducted.

🚀 How to Run
Clone the repository:

Bash

git clone https://github.com/your-username/kmnist-classification.git
Install dependencies:

Bash

pip install torch torchvision torchinfo mlflow scikit-learn matplotlib
Run the Notebook: Open Ido_Abodi_Amarteli_ex2.ipynb in Google Colab or Jupyter Notebook and run all cells.

View MLFlow Dashboard: To see the experiment logs, run the following in your terminal:

Bash

mlflow ui
