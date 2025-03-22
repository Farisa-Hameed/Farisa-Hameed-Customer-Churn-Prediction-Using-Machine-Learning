# Farisa-Hameed-Customer-Churn-Prediction-Using-Machine-Learning
Overview

This project aims to predict customer churn in a telecom company using advanced machine learning techniques. By leveraging multiple classification models and ensemble learning strategies, we achieve high predictive accuracy and gain insights into key factors influencing customer retention.

Dataset

The dataset used in this project is the Telco Customer Churn dataset. It contains customer demographics, service usage patterns, and account information.

Key Features:

Demographic information (gender, senior citizen status, partner, and dependents)

Service subscription details (contract type, tenure, payment method, etc.)

Billing information (monthly charges, total charges)

Churn status (whether a customer has churned or not)

Project Workflow

1. Data Preprocessing

Handling missing values in TotalCharges

Encoding categorical features using LabelEncoder

Standardizing numerical features using StandardScaler

Handling class imbalance using SMOTE

2. Feature Selection

Initial feature importance analysis using Random Forest

Selecting the top 15 most relevant features

3. Model Training & Optimization

The project implements multiple models:

Random Forest Classifier

Gradient Boosting Classifier

XGBoost Classifier (Optimized using Bayesian Search)

LightGBM Classifier (Optimized using Bayesian Search)

Decision Tree Classifier

4. Ensemble Learning

To improve prediction performance, we employ:

Stacked Model: Combines multiple models with a Logistic Regression final estimator.

Voting Classifier: Uses soft voting among the best-performing models.

5. Model Evaluation

Models are evaluated using:

Accuracy Score

Classification Report (Precision, Recall, F1-score)

Confusion Matrix

ROC Curve and AUC Score

Results

Model Performance

Model

Accuracy

Stacked Model

0.7892

Voting Model

0.8006

Decision Tree

0.7594

The Voting Model achieved the highest accuracy (80.06%).

The Stacked Model provided competitive performance with robust generalization.

Feature Importance

Top features influencing churn include tenure, monthly charges, contract type, and payment method.

Visualization

The project includes:

Feature importance plots (Before & After Model Training)

Confusion Matrices

ROC Curve for Model Performance Comparison

Installation & Usage

Requirements

Install the required dependencies using:

pip install -r requirements.txt

Running the Project

To execute the pipeline, run:

python churn_prediction.py

Conclusion

This project demonstrates the effectiveness of ensemble models in predicting customer churn. The results provide actionable insights for telecom companies to retain customers and minimize churn rates.

Future Improvements

Hyperparameter tuning using Grid Search or Genetic Algorithms

Deployment as a web service using Flask or FastAPI

Integration with real-time customer data for live predictions

