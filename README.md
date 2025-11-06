Heart Disease Prediction using Machine Learning

This project uses Machine Learning to predict the likelihood of heart disease based on a person’s medical parameters such as age, blood pressure, cholesterol, ECG results, and heart rate.
It applies Logistic Regression with calibration to provide more realistic probability predictions.
The app is built using Streamlit for an interactive, user-friendly interface and deployed using Ngrok.

---

Overview
This project demonstrates an end-to-end machine learning pipeline — from data preprocessing, training, scaling, and calibration to building a live prediction web app.
Users can enter their health details and instantly get an AI-based assessment of their heart disease risk level (Low, Moderate, or High).

The dataset used typically contains 13 medical features and a binary target variable (1 = Heart Disease, 0 = No Heart Disease).

---

Features

* Interactive Streamlit web interface
* Predicts heart disease likelihood with probability-based confidence
* Shows color-coded safe/risky feedback for each input
* Calibrated Logistic Regression for accurate probability estimates
* Deployed online using Ngrok

---

Tech Stack
Programming Language: Python 3
Libraries: scikit-learn, pandas, numpy, joblib, streamlit, pyngrok
Algorithm: Logistic Regression with Calibration
Deployment: Streamlit + Ngrok
Model Saving: joblib

---

Project Structure

heart-disease-prediction-ml
│
├── heart_disease_notebook.ipynb      (Model training notebook)
├── app.py                            (Streamlit app for prediction)
├── heart_disease_model.pkl           (Trained Logistic Regression model)
├── scaler.pkl                        (Saved StandardScaler)
├── requirements.txt                  (Dependencies)
└── README.md                         (Project documentation)

---

Installation and Running

Step 1 — Clone the Repository

Step 2 — Install Dependencies
pip install -r requirements.txt

Step 3 — Run the Streamlit App
streamlit run app.py

Step 4 — (Optional) Host Publicly with Ngrok
from pyngrok import ngrok
ngrok.connect(8501)

---

Model Details
Dataset: Heart Disease Dataset (13 features + target)
Algorithm: Logistic Regression with calibration (sigmoid method)
Target: 1 = Heart Disease, 0 = Healthy
Evaluation Metrics: Accuracy, Precision, Recall, F1-score

---

Example Output

User Input:
Age = 54
Cholesterol = 220
Resting BP = 140
Max Heart Rate = 160
Oldpeak = 2.1

Output:
Predicted Class: High Risk
Confidence: 87%
Interpretation: Strong indicators of cardiac stress — doctor consultation advised.

---

Future Improvements

* Add advanced models (Random Forest, XGBoost, or Neural Networks)
* Add visualization dashboard for health metrics
* Deploy on Streamlit Cloud or Hugging Face Spaces
* Add feature importance explanation using SHAP


Conclusion
This project demonstrates how Machine Learning can assist in preventive healthcare by analyzing patient data and providing early warnings about potential heart disease risks.
It is designed for educational and awareness purposes and not as a substitute for medical advice.

