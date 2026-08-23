Deep Learning - Customer Churn Classification
​Deep Learning (Multilayer Perceptron) model for predicting whether a bank customer will leave the bank or stay using the Churn Modelling dataset.
​About the Project
​This is a Deep Learning Classification project that I built using the Churn Modelling dataset.
​I used customer information in the dataset to build and train an Artificial Neural Network (Multilayer Perceptron) using TensorFlow and Keras to predict if a customer will leave the bank.
​The target column is Exited.
​0 = Customer stayed
​1 = Customer exited
​Dataset
​The dataset contains information about bank customers.
​It has 10,000 rows and 14 columns.
​Some of the key columns are:
​CreditScore
​Geography
​Gender
​Age
​Tenure
​Balance
​NumOfProducts
​HasCrCard
​IsActiveMember
​EstimatedSalary
​Exited
​There were no missing values in the dataset.
​I removed columns that were not useful for model training:
​RowNumber
​CustomerId
​Surname
​I also converted the categorical columns (Geography and Gender) into numerical values using One-Hot Encoding before scaling and training.
​What I Used
​Python
​Pandas & NumPy (Data Manipulation & Preprocessing)
​Scikit-learn (Dataset Splitting & Feature Scaling)
​TensorFlow / Keras (Building & Training the Deep Learning Model)
​Jupyter Notebook / Google Colab
​Steps
​I followed these steps in the project:
​Imported Libraries: Loaded necessary tools for data preprocessing and TensorFlow/Keras for model building.
​Loaded Dataset: Loaded Churn_Modelling.csv.
​Explored Data: Checked general dataset info, shapes, and verified no missing values exist.
​Cleaned Data: Dropped unnecessary identifier columns (RowNumber, CustomerId, Surname).
​Encoded Categorical Variables: Converted Geography and Gender into binary numeric values using pd.get_dummies(drop_first=True).
​Separated Features & Target: Set Exited as the target variable (y) and remaining features as (X).
​Split Data: Applied stratified split with 80% training data and 20% testing data.
​Feature Scaling: Scaled input features using StandardScaler to optimize Neural Network convergence.
​Built Neural Network Architecture:
​Input Layer: Features shape
​Hidden Layer 1: 16 Neurons + ReLU activation
​Hidden Layer 2: 8 Neurons + ReLU activation
​Output Layer: 1 Neuron + Sigmoid activation
​Compiled Model: Used Adam optimizer, binary_crossentropy loss function, and accuracy metric.
​Trained Model: Fit the model over 50 epochs with a batch size of 32 and a 20% validation split.
​Evaluated Model: Measured performance on the unseen test set using accuracy, confusion matrix, and classification report.
​Model Architecture
​Algorithm: Multilayer Perceptron (MLP) / Deep Neural Network
​Framework: TensorFlow 2.x + Keras
​Loss Function: Binary Cross-Entropy
​Optimizer: Adam
​Target: ExitedInput Features
      ↓
Dense Layer (16 Neurons, ReLU)
      ↓
Dense Layer (8 Neurons, ReLU)
      ↓
Output Layer (1 Neuron, Sigmoid)
      ↓
Exited (0 = No Churn, 1 = Churn)
Results
​The Deep Learning model achieved strong performance on the test data:
​Accuracy: ~86.0%
​Loss: Binary Cross-Entropy Loss on test set
​Decision Threshold: 0.5 (probabilities \ge 0.5 mapped to class 1)
​The classification results showed high precision and accuracy in distinguishing between customers who stay vs. those who exit.
​Files
​churn_deep_learning.ipynb - The notebook containing full code, model training history, and evaluation.
​Churn_Modelling.csv - The dataset used in the project.
​README.md - Complete description and documentations of the project.
​What I Learned
​From this project, I learned how to build and train a Deep Learning Neural Network for Binary Classification tasks:
​Preprocessing data specifically for Neural Networks (Scaling and One-Hot Encoding).
​Structuring dense layers with proper activation functions (ReLU for hidden layers, Sigmoid for binary output).
​Compiling Deep Learning models with appropriate loss functions (binary_crossentropy) and optimizers (Adam).
​Training models with epochs, batch sizes, and validation splits, then evaluating performance with classification metrics.
​Author
​Omnia Mohamed
