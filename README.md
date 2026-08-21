# random-forest-customer-churn-classification
Random Forest Classification model for predicting customer churn using the Churn Modelling dataset.
# Random Forest - Customer Churn Classification

Random Forest Classification model for predicting whether a bank customer will leave the bank or stay.

## About the Project

This is a simple Machine Learning Classification project that I made using the Churn Modelling dataset.

I used the customer information in the dataset to predict if a customer will leave the bank.

The target column is `Exited`.

* `0` = Customer stayed
* `1` = Customer exited

## Dataset

The dataset contains information about bank customers.

It has 10,000 rows and 14 columns.

Some of the columns are:

* `CreditScore`
* `Geography`
* `Gender`
* `Age`
* `Tenure`
* `Balance`
* `NumOfProducts`
* `HasCrCard`
* `IsActiveMember`
* `EstimatedSalary`
* `Exited`

There were no missing values in the dataset.

I removed some columns that were not useful for the model:

* `RowNumber`
* `CustomerId`
* `Surname`

I also converted the categorical columns into numerical values before training the model.

## What I Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

## Steps

I followed these steps in the project:

1. Loaded the dataset.
2. Checked the data and missing values.
3. Removed the unnecessary columns.
4. Converted the categorical columns into numerical values.
5. Selected the features and the target.
6. Used `Exited` as the target.
7. Split the data into training and testing sets.
8. Created a Random Forest Classifier.
9. Trained the model.
10. Made predictions on the test data.
11. Evaluated the model.
12. Created a confusion matrix.
13. Plotted the feature importance.

## Model

**Algorithm:**

`RandomForestClassifier`

**Target:**

`Exited`

I used 80% of the data for training and 20% for testing.

The Random Forest model uses 100 decision trees.

## Results

The model gave me these results:

* Accuracy: `0.8610`
* Precision: `0.7699`
* Recall: `0.4521`
* F1 Score: `0.5697`

The model achieved an accuracy of about **86.1%** on the test data.

The confusion matrix was:

```text
[[1538   55]
 [ 223  184]]
```

This means:

* `1538` customers were correctly predicted as stayed.
* `55` customers were predicted as exited but actually stayed.
* `223` customers were predicted as stayed but actually exited.
* `184` customers were correctly predicted as exited.

## Visualization

I created a **Confusion Matrix** to see the correct and incorrect predictions made by the model.

I also created a **Feature Importance** graph to see which features were more important for the Random Forest model.

Some of the important features were:

* `Age`
* `EstimatedSalary`
* `CreditScore`
* `Balance`
* `NumOfProducts`
* `Tenure`

`Age` was the most important feature in the model.

## Files

* `churn_classification.ipynb` - The notebook containing the code and results.
* `Churn_Modelling.csv` - The dataset used in the project.
* `README.md` - Description of the project.

## What I Learned

From this project, I learned how to use a Classification algorithm to predict customer churn.

I practiced data cleaning, converting categorical data, splitting the dataset, training a Random Forest model, making predictions, evaluating the model, creating a confusion matrix, and checking feature importance.

## Author

**Omnia Mohamed**
