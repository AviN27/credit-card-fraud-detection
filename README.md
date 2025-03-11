# 📌 Credit Card Fraud Detection
Upgrad Data Science Bootcamp - Capstone Project.

## 📖 Project Overview
This project aims to detect fraudulent transactions in credit card data using machine learning techniques. The dataset used is a well-known credit card fraud dataset, where transactions are labeled as either legitimate (0) or fraudulent (1). The goal is to build a model that can accurately distinguish between these two classes.

## ✅ Problem Statement
Credit card fraud is a significant financial crime affecting consumers and institutions. Identifying fraudulent transactions quickly and accurately is crucial to minimize losses. This project applies data science and machine learning techniques to analyze transaction patterns and classify them accordingly.

## 📂 Dataset Information
The dataset consists of **284,807** transactions with **31 features**:
- **Time**: Number of seconds elapsed between the first transaction and the given transaction.
- **V1-V28**: Principal components obtained using PCA to anonymize original features.
- **Amount**: Transaction amount.
- **Class**: The target variable (0 = Legitimate, 1 = Fraudulent).

## ⚙️ Methodology
1. **Data Preprocessing**: Handling missing values, normalizing numerical features, and performing exploratory data analysis (EDA).
2. **Feature Engineering**: Using feature selection and transformation techniques to enhance model performance.
3. **Model Training**: Training machine learning models such as logistic regression, decision trees, random forests, and deep learning-based methods.
4. **Evaluation**: Assessing performance using accuracy, precision, recall, F1-score, and ROC-AUC metrics.

## 🛠️ Installation & Setup
### Prerequisites
Ensure you have the following installed:
- Python (>=3.8)
- Jupyter Notebook (optional for interactive analysis)
- Required libraries:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn
  ```

### 🚀 Running the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repository.git
   cd credit-card-fraud-detection
   ```
2. Run the Jupyter Notebook or Python script:
   ```bash
   jupyter notebook analysis.ipynb
   ```
   or
   ```bash
   python main.py
   ```

## 📊 Model Training & Evaluation
- The dataset is highly imbalanced, so techniques like **SMOTE (Synthetic Minority Over-sampling Technique)** and **class weighting** are applied.
- Evaluation is performed using various classification metrics to ensure robustness.
- The final trained model can be saved and used for real-time fraud detection.

## 🎯 Results & Insights
- The dataset contains a highly imbalanced class distribution (fraud cases are rare).
- Logistic regression, random forests, and neural networks show varying levels of performance.
- Feature importance analysis helps in understanding transaction behavior.

## 📢 Future Improvements
- Experimenting with deep learning techniques (e.g., LSTMs, autoencoders) for anomaly detection.
- Deploying the model as an API for real-time fraud detection.
- Improving data preprocessing strategies for better model generalization.

## Contributing
Feel free to contribute to this project by submitting pull requests or reporting issues.

## License
This project is released under the MIT License.

