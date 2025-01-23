# Health Insurance Premium Predictor 💻

## Overview  
The **Health Insurance Premium Predictor** is a machine learning-based application designed to estimate health insurance premiums based on user inputs such as age, BMI, smoking habits, income, and medical history. This project leverages advanced machine learning models to provide accurate and real-time predictions through an intuitive Streamlit web application.  

---

## Features  
- Predicts health insurance premiums based on 13 input features, including age, BMI, smoking status, and medical history.  
- Uses segmented models for different age groups to improve accuracy.  
- Interactive and user-friendly web interface built with Streamlit.  
- Deployed on Streamlit Cloud for accessibility.  

---

## Demo  
 https://healthcare-premium-predictor-kesavadas.streamlit.app/

---

## App Screenshot
![image](https://github.com/user-attachments/assets/c86b9a9a-c2a7-4927-9d44-2b02a699c401)

---

## Dataset  
- **Source:** Custom dataset with 50,000 rows and 13 columns.  
- **Features:**  
  - Age  
  - Number of Dependents  
  - Income (in Lakhs)  
  - Genetical Risk  
  - Insurance Plan  
  - Employment Status  
  - Gender  
  - Marital Status  
  - BMI Category  
  - Smoking Status  
  - Region  
  - Medical History  

---

## Machine Learning Pipeline  
1. **Feature Selection:**  
   - Variables selected using VIF (Variance Inflation Factor) and domain knowledge.  
2. **Data Splitting:**  
   - 70% training, 30% testing split.  
3. **Model Training:**  
   - Algorithms used:  
     - Logistic Regression  
     - Ridge Regression  
     - XGBoost  
   - Segmented models:  
     - **Model A (Age ≤ 25):** Trained using Linear Regression (Accuracy: 95%)
       ![image](https://github.com/user-attachments/assets/34a86386-01c5-482b-ae73-a6ae0f311410) 
     - **Model B (Age > 25):** Trained using XGBoost (Accuracy: 98%)
       ![image](https://github.com/user-attachments/assets/0790d34d-3748-4c37-9748-110e1bc66115)  
4. **Hyperparameter Tuning:**  
   - Fine-tuned using RandomizedSearchCV.  
5. **Model Retraining:**  
   - Added "Genetical Risk" feature to improve Model A’s accuracy.  

---

## Tech Stack  
- **Programming Language:** Python  
- **Frameworks/Libraries:**  
  - scikit-learn  
  - pandas  
  - numpy  
  - joblib  
  - XGBoost  
  - Streamlit  

---

## Installation  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/yourusername/health-insurance-premium-predictor.git  
   cd health-insurance-premium-predictor  

