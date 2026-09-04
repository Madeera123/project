Smart Diabetes Risk Predictor 🩺🤖

An interpretable machine learning-based decision support system for early diabetes risk prediction using lifestyle, demographic, and clinical health information.

The system combines machine learning, explainable AI, and an interactive Streamlit web application to provide users with a diabetes risk prediction, risk classification, explanatory insights, and basic lifestyle recommendations.

Disclaimer: This project is intended for educational and decision-support purposes only. It is not a medical diagnostic tool and should not replace professional medical advice or clinical testing.

📌 Project Overview

Diabetes can develop gradually and may remain undetected during its early stages. This project explores how machine learning can be used to identify patterns associated with diabetes risk and provide an accessible way for users to understand their predicted risk.

The project uses a publicly available dataset containing 10,000 records and follows an end-to-end machine learning workflow:

Data preprocessing
Exploratory data analysis
Feature analysis
Machine learning model development
Model comparison and evaluation
Hyperparameter optimization
Decision-threshold optimization
Explainable AI
Web application deployment
Functional testing and validation

The final system uses a Random Forest classifier and integrates SHAP and LIME to make predictions more interpretable.

✨ Key Features
🔮 Diabetes Risk Prediction

Users can enter relevant demographic, lifestyle, and clinical information and receive a real-time diabetes risk prediction.

📊 Probability-Based Results

The application provides a prediction probability and converts the model output into a risk category using an optimized classification threshold.

🧠 Explainable AI

The system uses two explainability approaches:

SHAP – Provides global feature importance and individual prediction explanations.
LIME – Provides local, model-agnostic explanations for individual predictions.

Important predictors identified by the model include factors such as:

Fasting blood glucose
HbA1c
Dietary calorie intake
Waist circumference
Body mass index (BMI)
Age
💡 Lifestyle Recommendations

The application provides basic context-aware lifestyle recommendations based on user-provided lifestyle factors.

🌐 Interactive Web Application

The trained model is integrated into a Streamlit application that allows users to interact with the prediction system without directly interacting with Python or machine-learning code.

✅ Input Validation

The application validates user inputs and handles invalid or extreme values to prevent inappropriate predictions and improve system stability.

🧪 Machine Learning Approach

Several supervised machine learning algorithms were developed and compared during the project.

The final model selected was a:

Random Forest Classifier

Model evaluation considered:

Accuracy
Precision
Recall
F1-score
ROC-AUC
Confusion matrix
ROC curve

The project also applied cross-validation, hyperparameter optimization, and decision-threshold optimization to improve model reliability and balance sensitivity and specificity.

Decision Threshold

Instead of relying exclusively on the default classification threshold, the project uses an optimized threshold for risk classification.

The testing report documents a threshold of approximately 0.89 for the implemented classification logic.

🧠 Explainability

Interpretability is one of the main objectives of this project.

SHAP

SHAP is used to understand:

Overall feature importance
Individual prediction contributions
Factors increasing or decreasing predicted risk
LIME

LIME provides local explanations by approximating the model around an individual prediction.

Together, SHAP and LIME allow the application to communicate not only what the model predicts, but also why the prediction was produced.

🛠️ Technology Stack
Technology	Purpose
Python	Core programming language
Scikit-learn	Machine learning and preprocessing
Pandas	Data manipulation and analysis
NumPy	Numerical operations
SHAP	Explainable AI
LIME	Local model explanations
Matplotlib	Data visualization
Seaborn	Statistical visualization
Streamlit	Interactive web application
Visual Studio Code	Development environment

The project was developed using open-source technologies and standard computing resources, keeping implementation costs low.
