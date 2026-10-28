# Heart Disease Prediction Using Machine Learning

## Project Overview

Heart Disease Prediction is a machine learning project that estimates the likelihood of coronary heart disease based on an individual's health parameters.

The project uses a **Random Forest Classifier** trained on health-related data and integrates the trained model into a Flask web application. Users can enter their health information through a web interface and receive a model-generated prediction.

This project demonstrates the application of machine learning, data preprocessing, feature scaling, model deployment, and web development in healthcare analytics.

## Objectives

- Analyze health-related data for heart disease prediction.
- Preprocess data and handle missing values.
- Train and evaluate classification models.
- Apply feature scaling using StandardScaler.
- Develop a web application using Flask.
- Accept user inputs and display prediction results.

## Technologies Used

- **Programming Language:** Python
- **Machine Learning:** Scikit-learn
- **Algorithm:** Random Forest Classifier
- **Data Processing:** NumPy, Pandas
- **Web Framework:** Flask
- **Development Environment:** Google Colab / PyCharm
- **Model Serialization:** Pickle

## Dataset

The project uses the Framingham heart disease dataset, which contains demographic and health-related attributes.

Features used by the prediction application include:

- Gender
- Age
- Current smoking status
- Cigarettes smoked per day
- Blood pressure medication
- Previous stroke
- Hypertension
- Diabetes
- Total cholesterol
- Systolic blood pressure
- Diastolic blood pressure
- Body Mass Index (BMI)
- Heart rate
- Glucose level

The target variable is `TenYearCHD`, representing the ten-year coronary heart disease outcome.

## Project Workflow

1. Load the dataset.
2. Explore and preprocess the data.
3. Handle missing values as required.
4. Split the dataset into training and testing sets.
5. Train and evaluate classification models.
6. Scale the features using a fitted StandardScaler.
7. Save the trained Random Forest model and scaler.
8. Load the saved artifacts in the Flask application.
9. Collect user inputs through an HTML form.
10. Display the model's prediction on the web page.

## Features

- Interactive web-based prediction form.
- Machine learning-powered classification.
- Input validation and error handling.
- Reuse of the trained model and feature scaler.
- Prediction results displayed through a Flask interface.

## Project Structure

```text
heart-disease-prediction-ml/
│
├── app.py
├── index.html
├── Heart_Disease_Prediction_Project.ipynb
├── datasets_4123_6408_framingham.csv
├── requirements.txt
├── README.md
│
├── Models/
│   ├── rf_classifier.pkl
│   └── scaler.pkl
│
└── templates/
    └── index.html
```

**Note:** Adjust this structure to match your actual repository. Flask normally looks for HTML templates inside the `templates/` directory, so place `index.html` there if your application uses `render_template("index.html")`.

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/heart-disease-prediction-ml.git
```

### 2. Navigate to the project directory

```bash
cd heart-disease-prediction-ml
```

### 3. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

### 4. Install dependencies

Create a `requirements.txt` file containing the dependencies required by your project. For the Flask prediction application, start with:

```text
Flask
numpy
scikit-learn
```

Install them using:

```bash
pip install -r requirements.txt
```

For reproducibility, use the compatible package versions from the environment in which the model was trained.

### 5. Verify the required files

Ensure the following files exist before starting the application:

- `Models/rf_classifier.pkl`
- `Models/scaler.pkl`
- The HTML template in the location expected by Flask.

### 6. Run the application

```bash
python app.py
```

Open the local address displayed in the terminal, usually:

```text
http://127.0.0.1:5000/
```

Enter the requested health information and submit the form to view the prediction.

## Model Evaluation

Classification models can be evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix
- Classification report

Add your actual test-set results here after verifying them in your notebook.

| Metric    | Result             |
| --------- | ------------------ |
| Accuracy  | Add measured value |
| Precision | Add measured value |
| Recall    | Add measured value |
| F1-score  | Add measured value |

