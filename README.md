# Credit Card Fraud Detection
Upgrad Capstone Project (Data Science Bootcamp)

## 📌 Project Overview
This project aims to detect fraudulent credit card transactions using machine learning techniques. The dataset used is highly imbalanced, as fraudulent transactions are rare compared to genuine ones. To tackle this issue, Synthetic Minority Over-sampling Technique (SMOTE) is applied. The model is trained using a **Random Forest Classifier** and evaluated based on various performance metrics.

## 🔍 Problem Statement
Financial fraud is a major challenge in the banking sector, leading to huge monetary losses. This project builds a fraud detection system that can classify transactions as **fraudulent (1) or non-fraudulent (0)** with high accuracy.

## 📂 Dataset
The dataset used for this project is the **Credit Card Fraud Detection dataset** from Kaggle. It contains **284,807 transactions**, of which only **492** are fraudulent (high class imbalance).

- **Features**: 30 numerical features (`V1` to `V28`), `Time`, and `Amount`
- **Target Variable**: `Class` (0 = Genuine, 1 = Fraudulent)

## 🛠️ Tech Stack & Dependencies
- **Python** (pandas, numpy, matplotlib, seaborn, scikit-learn, imbalanced-learn, joblib)
- **Machine Learning Algorithm**: Random Forest Classifier
- **Resampling Technique**: SMOTE (Synthetic Minority Over-sampling Technique)

## ⚙️ Project Setup

### 1️⃣ Install Dependencies
Ensure you have Python installed (preferably **Python 3.8+**). Then, install the required dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn joblib
```

### 2️⃣ Download Dataset
Download the `creditcard.csv` dataset from [Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud) and place it in the project directory.

### 3️⃣ Run the Code
Execute the Python script to train the model and generate results:
```bash
python fraud_detection.py
```

## 🔄 Data Preprocessing
1. **Feature Scaling**: The `Amount` column is scaled using `StandardScaler`.
2. **Dropping Irrelevant Features**: The `Time` column is removed.
3. **Handling Imbalanced Data**: SMOTE is applied to balance the fraud and non-fraud cases.
4. **Train-Test Split**: The dataset is split into 80% training and 20% testing data.

## 🎯 Model Training & Evaluation
- The **Random Forest Classifier** is trained with **100 estimators**.
- The model's performance is evaluated using:
  - **Accuracy Score**
  - **Classification Report** (Precision, Recall, F1-score)
  - **Confusion Matrix**

## 📊 Visualizations
- **Class Distribution**: Shows the data imbalance before applying SMOTE.
- **Feature Correlation Heatmap**: Helps understand feature relationships.
- **Confusion Matrix**: Evaluates model predictions.

## 🚀 Deployment Plan
- **Model Saving**: The trained model is saved as `credit_card_fraud_model.pkl` using `joblib`.
- The saved model can be used for real-time fraud detection by loading it and making predictions on new transaction data.

## 📜 Future Improvements
- Experiment with **deep learning** (e.g., LSTM, Autoencoders) for anomaly detection.
- Deploy the model as a **REST API** using Flask or FastAPI.
- Implement **real-time fraud detection** by integrating the model with a live transaction processing system.

## 👥 Contributors
- **Avinash_Naidu**

## 📝 License
This project is open-source under the **MIT License**.

