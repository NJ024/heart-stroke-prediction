# Heart Stroke Prediction App

A simple web app that predicts the risk of heart disease based on a patient's clinical details, built with **Streamlit** and a **K-Nearest Neighbors (KNN)** classification model.

## Description

This project uses a machine learning model trained on heart disease clinical data to estimate whether a person is at **high risk** or **low risk** of heart disease. Users input details like age, sex, chest pain type, blood pressure, cholesterol, and other clinical indicators through an interactive web interface, and the app returns an instant prediction.

The model was trained and evaluated in `heart_project.ipynb`, and the final trained KNN model, feature scaler, and expected input columns were exported as `.pkl` files for use in the Streamlit app (`app.py`).

### Features used for prediction
- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Cholesterol
- Fasting Blood Sugar
- Resting ECG
- Max Heart Rate
- Exercise-Induced Angina
- Oldpeak (ST Depression)
- ST Slope

## Project Structure

```
heart-stroke-prediction/
├── app.py                  # Streamlit web app
├── KNN_heart.pkl            # Trained KNN model
├── scaler.pkl                # Fitted feature scaler
├── columns.pkl                # Expected input columns for the model
├── heart_project.ipynb     # Notebook with data analysis & model training
├── requirements.txt          # Python dependencies
├── README.md                 # Project documentation
└── .gitignore
```

## How to Run Locally

1. Clone the repository
   ```bash
   git clone https://github.com/<your-username>/heart-stroke-prediction.git
   cd heart-stroke-prediction
   ```

2. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Streamlit app
   ```bash
   streamlit run app.py
   ```

4. Open the local URL shown in the terminal (usually `http://localhost:8501`) in your browser.

## Deployment

This app can be deployed for free on [Streamlit Community Cloud](https://streamlit.io/cloud) by connecting your GitHub repository.

## Disclaimer

This tool is for educational purposes only and is **not a substitute for professional medical advice, diagnosis, or treatment**. Always consult a qualified healthcare provider regarding any medical condition.

## Author

Built by Nupur
