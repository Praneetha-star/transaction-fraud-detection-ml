# Online Transaction Fraud Detection using Machine Learning

## 📌 Project Overview

This project is a **Machine Learning-based Online Transaction Fraud Detection system** that predicts whether a financial transaction is **Fraud** or **No Fraud**.

The model analyzes transaction details such as transaction type, transaction amount, and the sender's balance before and after the transaction. A **Decision Tree Classifier** is used to learn patterns from historical transaction data and classify new transactions.

## 🎯 Objective

The main objective of this project is to:

* Detect potentially fraudulent financial transactions.
* Analyze transaction patterns using Machine Learning.
* Preprocess and transform transaction data for model training.
* Predict whether a new transaction is fraudulent or genuine.

## 📊 Dataset

The dataset contains financial transaction records with features such as:

* `step` – Time step of the transaction
* `type` – Type of transaction
* `amount` – Transaction amount
* `nameOrig` – Sender account identifier
* `oldbalanceOrg` – Sender's balance before the transaction
* `newbalanceOrig` – Sender's balance after the transaction
* `nameDest` – Receiver account identifier
* `oldbalanceDest` – Receiver's balance before the transaction
* `newbalanceDest` – Receiver's balance after the transaction
* `isFraud` – Indicates whether the transaction is fraudulent
* `isFlaggedFraud` – Indicates whether the transaction was flagged

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Plotly
* Jupyter Notebook / Google Colab
* Decision Tree Classifier

## 🔄 Project Workflow

```text
Transaction Dataset
        ↓
Data Loading
        ↓
Data Exploration
        ↓
Missing Value Checking
        ↓
Transaction Type Analysis
        ↓
Correlation Analysis
        ↓
Data Preprocessing
        ↓
One-Hot Encoding
        ↓
Train-Test Split
        ↓
Decision Tree Classifier
        ↓
Model Evaluation
        ↓
Fraud / No Fraud Prediction
```

## 🔍 Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the transaction dataset using Pandas.
2. Checked the dataset for missing values.
3. Analyzed the distribution of transaction types.
4. Converted the transaction type into a machine-readable format.
5. Applied **One-Hot Encoding** to the transaction type.
6. Selected relevant features for model training.
7. Split the dataset into training and testing sets.

## 🤖 Machine Learning Model

A **Decision Tree Classifier** was used for fraud classification.

The model was trained using the following features:

```text
Transaction Type
Transaction Amount
Old Sender Balance
New Sender Balance
```

The target variable is:

```text
isFraud
```

where:

```text
0 → No Fraud
1 → Fraud
```

## 📈 Model Result

The initial model achieved approximately **99.94% accuracy** on the test dataset.

> **Note:** Since fraud detection datasets can be highly imbalanced, accuracy alone is not sufficient to evaluate the model. Precision, recall, F1-score, and a confusion matrix are useful additional evaluation metrics.

## 🔮 Prediction

The trained model can be used to classify a transaction as:

```text
Fraud
```

or

```text
No Fraud
```

based on its transaction details.

## 🚀 Future Improvements

The project can be improved by:

* Handling class imbalance using techniques such as SMOTE or class weights.
* Evaluating precision, recall, F1-score, and confusion matrix.
* Comparing multiple Machine Learning algorithms.
* Performing feature engineering.
* Using additional transaction features.
* Building a web interface for real-time fraud prediction.
* Deploying the model as a web application.

## 👩‍💻 Author

**Praneetha Chutla**

B.Tech – Computer Science and Engineering (AIML)

---

⭐ If you find this project useful, feel free to explore the repository!
