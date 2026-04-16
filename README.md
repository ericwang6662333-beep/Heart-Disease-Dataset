README: Heart Disease Prediction Project
Overview
This project predicts the presence of heart disease using the Cleveland dataset (13 clinical features). It builds a Deep Learning model (ANN) and compares its performance against a traditional Machine Learning baseline (Random Forest).

Project Structure
Data Loading: Imports the raw dataset into pandas.

Preprocessing: Cleans missing values, standardizes numerical features, and splits the data (80% training / 20% testing).

Model Design: Constructs a Feedforward Neural Network (2 hidden layers, ReLU activation, Dropout layer).

Training: Trains the ANN for 50 epochs using the Adam optimizer.

Evaluation: Evaluates the ANN using a confusion matrix and classification report, with a strict focus on minimizing False Negatives.

Baseline Comparison: Trains a Random Forest classifier on the same data for objective benchmarking.

How to Run in Azure ML
Log in to Azure Machine Learning Studio and upload this Jupyter Notebook to your workspace.

In the top right corner, set the kernel to Python 3.10 - AzureML.

Wait for the kernel to connect (a standard CPU instance is sufficient).

Click Run All in the top toolbar.

Scroll through the notebook to see the data processing steps, training loss, and final evaluation metrics.
