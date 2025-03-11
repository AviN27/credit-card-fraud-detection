# Credit Card Fraud Detection

## Overview
This project implements a **Credit Card Fraud Detection** system using **Random Forest Classifier**. The dataset is highly imbalanced, so **SMOTE (Synthetic Minority Over-sampling Technique)** is used to balance the data. The model is trained and evaluated using various performance metrics.

## Features
- **Data Preprocessing:**
  - Standardization of the `Amount` column
  - Removal of the `Time` column
  - Handling imbalanced data using **SMOTE**
- **Exploratory Data Analysis (EDA):**
  - Class distribution visualization
  - Log-scaled y-axis for better visibility of fraud transactions
- **Model Training & Evaluation:**
  - **Random Forest Classifier** for fraud detection
  - **Confusion Matrix, Accuracy, and Classification Report** for evaluation
- **Model Persistence:**
  - Saves the trained model using **joblib**

## Prerequisites
Ensure you have **Python 3.7+** installed along with the required dependencies:
```sh
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn joblib
```

## Dataset
The dataset should be named **`creditcard.csv`** and must be placed in the same directory as the script. If the file is missing, the script will raise an error.

## Installation & Execution
1. Clone the repository or download the script.
2. Install dependencies using the command:
   ```sh
   pip install -r requirements.txt  # (if provided)
   ```
3. Run the script:
   ```sh
   python fraud_detection.py
   ```

## Output
- **Class Distribution Graph:** A log-scaled bar plot of fraud vs. non-fraud transactions.
- **Model Evaluation Metrics:** Accuracy, classification report, and confusion matrix.
- **Trained Model:** The trained model is saved as `credit_card_fraud_model.pkl`.

## Code Breakdown
1. **Load Dataset:** Reads `creditcard.csv` and checks for missing values.
2. **EDA:** Plots class distribution with log-scaling.
3. **Preprocessing:** Standardizes the `Amount` column and removes `Time`.
4. **Data Balancing:** Uses SMOTE to handle class imbalance.
5. **Train-Test Split:** Splits the balanced data into training and testing sets.
6. **Model Training:** Uses a **Random Forest Classifier**.
7. **Evaluation:** Computes accuracy, classification report, and confusion matrix.
8. **Model Saving:** Saves the trained model for future use.

## Results
The model aims to detect fraudulent transactions efficiently. Performance can be improved by experimenting with different algorithms or feature engineering techniques.

## License
This project is open-source and can be modified or distributed as needed.

## Author
Developed by **Avinash**

