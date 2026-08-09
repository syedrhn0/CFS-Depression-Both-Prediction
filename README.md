# CFS vs Depression Prediction

A machine learning classification project that predicts whether a person is likely experiencing **Chronic Fatigue Syndrome (ME/CFS), Depression, or both conditions** based on clinical symptoms and lifestyle-related features. The project includes data preprocessing, model training, evaluation, and a **Streamlit web application** for interactive predictions.

## Project Overview

ME/CFS and Depression share several overlapping symptoms such as fatigue, poor sleep, reduced activity levels, and cognitive difficulties. This project aims to assist in distinguishing between these conditions using machine learning models trained on patient-related features.

The application allows users to enter symptom and lifestyle information and receive a prediction using one of three trained classification models.

## Features

- Predicts **CFS**, **Depression**, or **Both**
- Interactive **Streamlit web application**
- Multiple model support:
  - Logistic Regression
  - Decision Tree
  - Random Forest
- Real-time prediction from user input
- Encoded categorical features and structured preprocessing pipeline

## Tech Stack

- **Python**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Streamlit**
- **Pickle**

## Dataset Features

The model uses patient-related features including:

- Age
- Gender
- Sleep Quality Index
- Brain Fog Level
- Physical Pain Score
- Stress Level
- PHQ-9 Depression Score
- Fatigue Severity Scale Score
- Post-Exertional Malaise (PEM) Duration
- Hours of Sleep per Night
- PEM Presence
- Meditation / Mindfulness
- Work Status
- Social Activity Level
- Exercise Frequency

## Machine Learning Models

Three classification algorithms were trained and compared:

| Model | Purpose |
|------|---------|
| Logistic Regression | Baseline linear classifier |
| Decision Tree | Interpretable rule-based classifier |
| Random Forest | Ensemble model for improved prediction performance |

Users can select the desired model directly from the Streamlit sidebar.

## Project Structure

```text
CFS-vs-Depression-Prediction/
│
├── data/
│   └── me_cfs_vs_depression.csv
│
├── Jupyter Notebook/
│   └── CFS-Depression-Both-Prediction.ipynb
│
├── models/
│   ├── dt.pkl
│   ├── lr.pkl
│   └── rf.pkl
│
├── app.py
├── requirements.txt
└── README.md
```

## How to Run

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/CFS-vs-Depression-Prediction.git
cd CFS-vs-Depression-Prediction
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the Streamlit application

```bash
streamlit run app.py
```

The application will open in your browser, where you can enter patient information and generate predictions.

## Streamlit Application

The app provides:

- Model selection from the sidebar
- User-friendly symptom input form
- Automatic feature encoding
- Display of entered values
- Instant prediction output

## Future Improvements

- Hyperparameter tuning
- Cross-validation and model comparison dashboard
- Probability/confidence score display
- Explainable AI integration (SHAP / feature importance)
- Deployment on Streamlit Cloud

## Disclaimer

This project is intended for **educational and portfolio purposes only**. It is **not a medical diagnostic tool** and should not be used for clinical decision-making.

## Author

**Syed Rehan**

If you found this project useful, consider giving the repository a ⭐ on GitHub.