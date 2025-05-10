# Noble_ANA-680_1-3
##Design a Three-Layered ANN Classifier
**Customer Churn Prediction Using Artificial Neural Networks (ANN)**

## Overview
This assignment involves building a three-layered Artificial Neural Network (ANN) to predict whether a bank customer is likely to leave based on their profile and activity history. The model will be trained and evaluated using the `Churn_Modelling.csv` dataset. Will not be tuning hyperparameters or using callbacks on this specific model.

---

## Dataset Details
* **File:** `Churn_Modelling.csv`
* **Samples:** \~10,000 bank customers
* **Features:** Multiple attributes including geography, gender, credit score, age, tenure, and account activity
* **Target Column:**
    * `Exited = 0` → Customer retained
    * `Exited = 1` → Customer turnover

---

## Objective
* **Identify key features** that contribute significantly to customer churn.
* **Preprocess the data**:
    * Encode categorical variables (e.g., Geography, Gender)
    * Perform feature scaling
* **Design a three-layer ANN** using TensorFlow/Keras to predict customer churn:
    * First hidden layer: ReLU activation
    * Second hidden layer: ReLU activation
    * Output layer: Sigmoid activation
* **Compile using**:
    * Optimizer: `adam`
    * Loss: `binary_crossentropy`
    * Metric: `accuracy`
* **Evaluate model performance** using:
    * Confusion matrix
    * Accuracy score

---

## Implementation Requirements
1. **Train/test split**:
     * Use 80% of data for training
     * Use 20% of data for testing
2. **Model architecture**:
     * Input layer based on number of features
     * 2 hidden layers with ReLU activation
     * Output layer with sigmoid activation
3. **Print outputs**:
     * Final accuracy on test set
     * Confusion matrix

---

## Modeling Options
* Use `OneHotEncoder` or `pd.get_dummies()` for geography
* Use `LabelEncoder` for binary categorical columns like gender
* Use `StandardScaler` from `sklearn` for scaling features
* Use `Sequential` model from `tensorflow.keras.models`
* Use `model.evaluate()` and `confusion_matrix()` from `sklearn.metrics`

---
