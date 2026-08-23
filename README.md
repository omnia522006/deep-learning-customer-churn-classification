# Deep Learning - Customer Churn Classification

Deep Learning (Multilayer Perceptron) model for predicting whether a bank customer will leave the bank or stay using the Churn Modelling dataset.

## About the Project
This is a Deep Learning Classification project that I built using the Churn Modelling dataset.

I used customer information in the dataset to build and train an Artificial Neural Network (Multilayer Perceptron) using TensorFlow and Keras to predict if a customer will leave the bank.

The target column is **Exited**.
* 0 = Customer stayed
* 1 = Customer exited

## Dataset
The dataset contains information about bank customers.

It has 10,000 rows and 14 columns.

Some of the key columns are:
* CreditScore
* Geography
* Gender
* Age
* Tenure
* Balance
* NumOfProducts
* HasCrCard
* IsActiveMember
* EstimatedSalary
* Exited

There were no missing values in the dataset.

I removed columns that were not useful for model training:
* RowNumber
* CustomerId
* Surname

I also converted the categorical columns (Geography and Gender) into numerical values using One-Hot Encoding before scaling and training.

## What I Used
* Python
* Pandas
* NumPy
* Scikit-learn
* TensorFlow / Keras
* Jupyter Notebook / Google Colab

## Steps
I followed these steps in the project:
1. Loaded the dataset.
2. Checked the data and missing values.
3. Removed unnecessary columns.
4. Converted categorical columns into numerical values.
5. Selected features and the target.
6. Split data into training and testing sets.
7. Scaled input features using StandardScaler.
8. Built Deep Learning Model (MLP Architecture).
9. Compiled the model with Adam optimizer and Binary Cross-Entropy loss.
10. Trained the model over 50 epochs.
11. Evaluated the model performance.
12. Generated predictions, Confusion Matrix, and Classification Report.

## Model Architecture
* Algorithm: Multilayer Perceptron (MLP) / Deep Neural Network
* Framework: TensorFlow 2.x + Keras
* Loss Function: Binary Cross-Entropy
* Optimizer: Adam
* Target: Exited

Input Features -> Dense(16, ReLU) -> Dense(8, ReLU) -> Output(1, Sigmoid)

## Results
The Deep Learning model achieved strong performance on the test data:
* Accuracy: ~86.0%
* Binary Cross-Entropy Loss optimization on test set
* Classification Threshold: 0.5

## Files
* churn_deep_learning.ipynb - The notebook containing code and results.
* Churn_Modelling.csv - The dataset used in the project.
* README.md - Description of the project.

## What I Learned
From this project, I learned how to build and train a Deep Learning Neural Network for Binary Classification tasks, scale features for neural networks, choose appropriate activation functions (ReLU and Sigmoid), compile models using TensorFlow/Keras, and evaluate network performance using classification metrics.

## Author
Omnia Mohamed
