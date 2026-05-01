# ❤️ Heart Disease Prediction System

A production-style Machine Learning web application for predicting the likelihood of heart disease using patient clinical data. This project combines **data preprocessing**, **model training**, **feature scaling**, and **real-time prediction through a Flask web interface**.

---

## 📌 Project Overview

Heart disease remains one of the leading causes of death worldwide. Early detection can significantly improve treatment outcomes. This application leverages **Machine Learning (KNN Classification)** to predict heart disease risk based on medical attributes such as age, cholesterol, blood pressure, chest pain type, and other clinical indicators.

The project includes:

✔ Data cleaning & preprocessing
✔ Feature engineering
✔ Model training using KNN
✔ Scaler transformation for prediction consistency
✔ Saved ML pipeline artifacts (`.pkl`)
✔ Flask-based interactive prediction UI
✔ Jupyter Notebook experimentation & evaluation

---

## 🚀 Features

### Machine Learning Pipeline

* Data preprocessing and normalization
* Missing value handling
* Feature scaling using StandardScaler
* Feature column persistence
* Model serialization for deployment

### Prediction Engine

* Real-time prediction
* Probability-based classification
* Fast inference
* Production-ready model loading

### Web Application

* User-friendly UI
* Form-based patient input
* Instant prediction results
* Responsive design
* Easy deployment

---

## 🧠 Model Used

### K-Nearest Neighbors (KNN)

KNN was selected for classification because:

* Simple and effective
* Works well on structured datasets
* Good performance on medical classification tasks
* Non-parametric learning
* Strong baseline accuracy

---

## 📂 Project Structure

```bash
HeartDiseasePrediction/
│
├── HeartdiseaseFinal.ipynb      # Data analysis, preprocessing & model training
├── app.py                       # Flask backend application
├── heart_columns.pkl            # Saved feature columns
├── heart_scaler.pkl             # Trained feature scaler
├── knn_heart_model.pkl          # Trained KNN model
├── templates/                  # HTML templates
├── static/                     # CSS / JS / images
└── README.md                   # Documentation
```

---

## 📁 File Description

### `HeartdiseaseFinal.ipynb`

Contains:

* Data loading
* Data visualization
* Exploratory Data Analysis
* Feature selection
* Model training
* Accuracy comparison
* Model export

---

### `app.py`

Main application server that:

* Loads trained model
* Loads scaler
* Loads feature columns
* Accepts user input
* Converts input into model-ready format
* Predicts disease outcome
* Returns results to UI

---

### `heart_columns.pkl`

Stores:

* Feature names
* Input column ordering
* Encoded columns
* Required preprocessing structure

Used to maintain training/prediction consistency.

---

### `heart_scaler.pkl`

Stores:

* StandardScaler object
* Mean normalization parameters
* Variance scaling parameters

Ensures:
**training data format = prediction data format**

---

### `knn_heart_model.pkl`

Serialized trained KNN model used for:

* Classification
* Prediction scoring
* Real-time inference

---

## ⚙️ Installation

Clone repository:

```bash
git clone https://github.com/yourusername/HeartDiseasePrediction.git
cd HeartDiseasePrediction
```

Create virtual environment:

```bash
python -m venv venv
```

Activate:

### Windows

```bash
venv\Scripts\activate
```

### Linux / Mac

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install flask numpy pandas scikit-learn joblib pickle-mixin
```

---

## ▶ Run Application

```bash
python app.py
```

Server starts:

```bash
http://127.0.0.1:5000/
```

Open browser and start predicting.

---

## 🧪 Input Parameters

Typical model inputs:

* Age
* Sex
* Chest Pain Type
* Resting Blood Pressure
* Cholesterol
* Fasting Blood Sugar
* ECG Results
* Maximum Heart Rate
* Exercise Angina
* Oldpeak
* ST Slope
* Number of Major Vessels
* Thalassemia

---

## 📊 Workflow

```text
User Input
   ↓
Validation
   ↓
Column Mapping
   ↓
Feature Scaling
   ↓
KNN Model Prediction
   ↓
Result Output
```

---

## 🔐 Future Enhancements

* Authentication system
* Patient history dashboard
* Model comparison (RF / XGBoost / SVM)
* Cloud deployment
* API endpoints
* Prediction confidence score
* Medical report export (PDF)
* Explainable AI (SHAP/LIME)
* Doctor recommendation engine

---

## 🛠 Tech Stack

**Backend**

* Python
* Flask

**Machine Learning**

* Scikit-Learn
* NumPy
* Pandas

**Frontend**

* HTML5
* CSS3
* JavaScript

**Deployment**

* Render / Heroku / AWS / Docker

---

## 📈 Potential Use Cases

* Hospitals
* Diagnostic centers
* Health startups
* Preventive healthcare apps
* Telemedicine platforms

---

## 👨‍💻 Author

**Rahul**
Full Stack Developer | ML Enthusiast

---

## License

MIT License

---

⭐ If you found this project useful, consider starring the repository.
