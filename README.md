<h1>Credit Card Fraud Detection Project</h1>

**This project is focused on detecting fraudulent credit card transactions using machine learning. The model was trained using the popular and publicly available creditcard.csv dataset.**

**Project Objective**

• The goal is to build a classification model that can identify whether a given transaction is fraudulent (Class = 1) or genuine (Class = 0) based on a number of input features.

**Dataset Overview**

• The dataset contains 284,807 transactions

• Only 492 are fraud cases (Class = 1), which makes the dataset highly imbalanced

• Features are labeled from V1 to V28 — these are anonymized components generated using PCA (Principal Component Analysis)

• Two additional columns:

-  Amount: The transaction amount

- Class: The target variable (0 = non-fraud, 1 = fraud)

- Time was dropped as it wasn’t useful for this model



**Tools and Libraries Used**

• Python

• Google Colab

• Pandas and NumPy for data handling

• Scikit-learn for machine learning and preprocessing


**Preprocessing Steps**

1. Uploaded the dataset using Google Colab's upload widget


2. Dropped the 'Time' column as it had no clear importance


3. Normalized the 'Amount' column using StandardScaler to bring it to a similar scale as the other features


4. Checked for missing values – the dataset had no nulls


5. Split the data into training and test sets (80% training, 20% testing)



**Model Used**

• Logistic Regression was used as the first (baseline) model due to its simplicity and interpretability

• Model was trained on the training dataset and predictions were made on the test dataset


**Evaluation Metrics**

• Accuracy: 99.91%

• Precision (Class 1 - Fraud): 85%

• Recall (Class 1 - Fraud): 57%

• F1 Score (Class 1 - Fraud): 68%

• Even though accuracy is very high, recall is more important for fraud detection (catching actual frauds)


**Results Summary**

• The model performed very well on overall accuracy

• It struggled a bit with recall on the fraud class due to the class imbalance

• Future improvements can include:

• Trying other ML algorithms like Random Forest, XGBoost, or Neural Networks

• Using SMOTE or oversampling techniques to handle imbalance

• Adding real-time monitoring or alert systems



**How to Run the Project**

1. Open the notebook in Google Colab


2. Upload the dataset creditcard.csv


3. Run each cell step-by-step to preprocess, train, and test the model


4. View the model performance using the printed classification report



**Final Notes**

• This project is great for understanding how to handle imbalanced datasets.

• It shows the basics of feature scaling, model training, evaluation, and performance metrics in fraud detection.

• Can be added to portfolio as a real-world machine learning use case.
