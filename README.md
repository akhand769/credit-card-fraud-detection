# 🧠 Credit Card Fraud Detection

This project aims to detect fraudulent credit card transactions using machine learning techniques.  
It involves data preprocessing, exploratory data analysis (EDA), model training, and evaluation of results.  

---

## 📂 Project Structure

├── README.md
├── data
│ ├── creditcard.csv # Raw dataset containing transaction data
│ └── processed_data # Preprocessed and split data
│ ├── X_test.pkl
│ ├── X_train.pkl
│ ├── y_test.pkl
│ └── y_train.pkl
├── models
│ └── random_forest_model.pkl # Trained Random Forest model saved for reuse
├── notebooks
│ ├── EDA.ipynb # Exploratory Data Analysis notebook
│ ├── data_preprocessing.ipynb # Data cleaning, scaling, and splitting
│ └── model_training.ipynb # Model training and evaluation
└── requirements.txt # Python dependencies


---

## 📊 Dataset

The dataset used is the **Credit Card Fraud Detection Dataset** from [Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud).  
It contains anonymized transaction data with 284,807 records and 31 features (including PCA-transformed variables `V1`–`V28`).

- **Classes:**
  - `0` → Non-fraudulent transaction  
  - `1` → Fraudulent transaction  

---

## ⚙️ Workflow Overview

1. **EDA (`notebooks/EDA.ipynb`)**
   - Understand class imbalance
   - Visualize feature distributions
   - Detect correlations

2. **Data Preprocessing (`notebooks/data_preprocessing.ipynb`)**
   - Handle missing values (if any)
   - Scale and normalize features
   - Split dataset into train/test sets
   - Save processed data as `.pkl` files

3. **Model Training (`notebooks/model_training.ipynb`)**
   - Train Random Forest and other classifiers
   - Evaluate model performance (Accuracy, Precision, Recall, F1, ROC-AUC)
   - Save the best-performing model as `.pkl`

---

## 📦 Installation

 Clone this repository:
   ```bash
   git clone https://github.com/akhand769/credit_card_fraud_detection.git
   cd credit_card_fraud_detection
