# Health Insurance Premium Predictor 💻

## Overview
This project predicts health insurance premiums based on various customer attributes such as age, BMI, region, and more. Using advanced machine learning techniques, the model provides accurate predictions to help users estimate their insurance premiums.

The project includes:
- A cleaned and processed dataset.
- Two predictive models tailored for different age groups:
  - For users aged **≤ 25**, a **Linear Regression model** was trained with an additional feature called **Genetical Risk**.
  - For users aged **> 25**, an **XGBoost model** was employed for its superior performance on larger datasets.
- A user-friendly Streamlit application for interacting with the model.

🖥 **Deployed App:** [Health Insurance Premium Predictor](https://healthcare-premium-predictor-kesavadas.streamlit.app/)

---

## Features
- **Age-Specific Models**:
  - **Linear Regression** for users aged ≤ 25.
  - **XGBoost** for users aged > 25.
- **Interactive Interface**: Users can input their details (age, BMI, smoking status, etc.) to get an instant premium prediction.
- **Machine Learning Pipelines**: Tailored workflows for preprocessing and training the models.
- **Streamlit Deployment**: A simple and intuitive web app for easy usage.

![App Screenshot](image.png)

---

## Technologies Used
- **Python**: Data preprocessing, model building, and evaluation.
- **Streamlit**: For creating and deploying the web application.
- **Libraries**: pandas, scikit-learn, XGBoost, matplotlib, seaborn, numpy.

---

## How to Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/health-insurance-premium-predictor.git
