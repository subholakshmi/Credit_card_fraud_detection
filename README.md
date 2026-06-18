# 💳 Credit Card Fraud Detection using Machine Learning

A machine learning-based system for detecting fraudulent credit card transactions on a highly imbalanced dataset. The project applies data balancing techniques, compares multiple classification models, and selects the best-performing model based on robust evaluation metrics.

---

## 📌 Overview

Credit card fraud detection is a binary classification problem where transactions are classified as:

* **0 → Legitimate Transaction**
* **1 → Fraudulent Transaction**

Due to the highly imbalanced nature of the dataset, special techniques such as **SMOTE** are used to improve the model's ability to identify fraudulent transactions.

---

## 🚀 Features

* Exploratory Data Analysis (EDA)
* Handling class imbalance using **SMOTE**
* Feature importance analysis using Mutual Information
* Training and comparison of multiple ML models
* Hyperparameter tuning with **GridSearchCV**
* Model evaluation using various performance metrics
* Selection of the best-performing model

---

## 🛠️ Tech Stack

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **Matplotlib**
* **Seaborn**
* **Imbalanced-learn (SMOTE)**
* **Jupyter Notebook**

---

## 📂 Dataset

The project uses the **Credit Card Fraud Detection Dataset**, which contains:

* **284,807 transactions**
* **31 features**
* **V1–V28:** PCA-transformed features
* **Time:** Time elapsed between transactions
* **Amount:** Transaction amount
* **Class:** Target variable

  * 0 → Non-Fraud
  * 1 → Fraud

The dataset is highly imbalanced, with fraudulent transactions accounting for only about **0.17%** of all transactions.

---

## 📊 Workflow

```text
Dataset
   ↓
Data Preprocessing
   ↓
Exploratory Data Analysis
   ↓
Train-Test Split
   ↓
SMOTE for Class Balancing
   ↓
Feature Importance Analysis
   ↓
Model Training
   ↓
Hyperparameter Tuning
   ↓
Performance Evaluation
   ↓
Best Model Selection
```

---

## 🤖 Models Used

* Random Forest Classifier
* Logistic Regression
* K-Nearest Neighbors (KNN)
* SGD Classifier

---

## ⚙️ Hyperparameter Tuning

The models were optimized using:

* **GridSearchCV**
* **5-Fold Cross Validation**
* **Matthews Correlation Coefficient (MCC)** as the scoring metric

---

## 📈 Evaluation Metrics

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC Score
* Matthews Correlation Coefficient (MCC)

---

## 🏆 Best Performing Model

**Random Forest Classifier**

### Performance

* **Accuracy:** 99.96%
* **Precision:** 0.90
* **Recall:** 0.86
* **F1-Score:** 0.88
* **ROC-AUC:** 0.93

The Random Forest model achieved the best balance between detecting fraudulent transactions and minimizing false positives.

---

## 📁 Project Structure

```text
├── creditcard.csv
├── Model_Final.ipynb
├── README.md
└── requirements.txt
```

---

## ▶️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Credit-Card-Fraud-Detection.git
cd Credit-Card-Fraud-Detection
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the notebook:

```bash
jupyter notebook Model_Final.ipynb
```

---

## 📌 Results

* Successfully handled severe class imbalance using **SMOTE**.
* Compared multiple machine learning algorithms.
* Selected **Random Forest** as the final model based on F1-Score and MCC.
* Achieved **99.96% accuracy** and **0.88 F1-score**.

---

## 🔮 Future Improvements

* XGBoost and LightGBM implementation
* Real-time fraud detection API using Flask/FastAPI
* Model deployment using Streamlit
* Explainable AI techniques using SHAP and LIME
* Deep learning-based fraud detection approaches

---

