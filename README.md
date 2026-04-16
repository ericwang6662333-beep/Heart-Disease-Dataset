# Heart Disease Prediction using Deep Learning

## Overview
This project predicts the presence of heart disease based on clinical measurements using the Cleveland Heart Disease dataset. It implements a Deep Learning model (Feedforward Artificial Neural Network) and compares its performance against a traditional Machine Learning baseline (Random Forest Classifier).

## Dataset
* **Source:** Cleveland Heart Disease dataset (derived from the UCI Machine Learning Repository).
* **Features:** 13 clinical attributes (e.g., age, resting blood pressure, cholesterol).
* **Target:** Binary classification (0 = No Heart Disease, 1 = Heart Disease Present).

## Project Structure
The Jupyter Notebook is organized into the following sequential sections:
1. **Data Loading:** Imports the dataset via a public CSV link into a pandas DataFrame.
2. **Data Preprocessing:** Cleans missing values, standardizes numerical features using `StandardScaler`, and splits the data into 80% training and 20% testing sets.
3. **Model Architecture:** Defines the PyTorch ANN architecture (Linear layers, ReLU activation, and Dropout regularization).
4. **Model Training:** Trains the network over 50 epochs using the Adam optimizer and `BCEWithLogitsLoss`.
5. **Evaluation:** Evaluates the ANN on the test set, outputting Accuracy, a Classification Report, and a Confusion Matrix.
6. **Baseline Comparison:** Trains and evaluates a Random Forest classifier on the same data for objective benchmarking.

## Prerequisites
The codebase relies on the following standard Python libraries:
* `pandas`
* `numpy`
* `torch`
* `scikit-learn`

## Execution Guide (Azure Machine Learning)
This notebook is designed to run seamlessly within Azure Machine Learning Studio without requiring local environment configuration.

1. Log in to **Azure Machine Learning Studio** and navigate to your compute instance.
2. Upload the Jupyter Notebook file to your working directory and open it.
3. In the kernel selection menu at the top right of the interface, select the **Python 3.10 - AzureML** kernel.
4. Wait for the kernel status to display as "Connected" or "Ready" (A standard CPU compute instance is sufficient; GPU acceleration is not required for this dataset).
5. Click the **Run All** button in the top toolbar.
6. The notebook will execute sequentially from top to bottom. Scroll down to view the automated data processing steps, training loss logs, and the final evaluation metrics.
