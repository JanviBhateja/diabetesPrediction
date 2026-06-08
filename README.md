# Diabetes Prediction using Support Vector Machine (SVM)

## Overview

This project uses Machine Learning to predict whether a person is diabetic or non-diabetic based on various medical parameters. The model is trained on the Pima Indians Diabetes Dataset and implemented using Python and Scikit-learn.

The primary objective of this project is to build a reliable classification model that can assist in the early prediction of diabetes using patient health data.

---

## Dataset

The project uses the **Pima Indians Diabetes Dataset**, which contains diagnostic measurements collected from female patients.

### Features Used

* Pregnancies
* Glucose
* Blood Pressure
* Skin Thickness
* Insulin
* BMI (Body Mass Index)
* Diabetes Pedigree Function
* Age

### Target Variable

* **Outcome**

  * 0 → Non-Diabetic
  * 1 → Diabetic

---

## Machine Learning Model

This project uses the **Support Vector Machine (SVM)** algorithm for classification.

### Why SVM?

Support Vector Machine is a supervised learning algorithm that finds the optimal decision boundary (hyperplane) to separate different classes. It is effective for classification problems and performs well on structured datasets.

---

## Technologies Used

* Python
* NumPy
* Pandas
* Scikit-learn
* Google Colab

---

## Project Workflow

1. Data Collection and Loading
2. Exploratory Data Analysis
3. Data Preprocessing
4. Feature Standardization using StandardScaler
5. Train-Test Split using Stratified Sampling
6. Training the Support Vector Machine (SVM) Model
7. Model Evaluation
8. Building a Diabetes Prediction System

---

## Model Performance

* Training Accuracy:  0.7866449511400652
* Testing Accuracy: 0.7727272727272727

> Replace the above values with the exact accuracies obtained from your notebook.

---

## Key Features

* Clean and structured data preprocessing
* Stratified train-test splitting
* Feature scaling using StandardScaler
* Support Vector Machine (SVM) classifier
* Prediction system for new patient data
* Model performance evaluation

---

## Repository Structure

```text
diabetesPrediction/
│
├── diabetesPrediction.ipynb
├── diabetes.csv
└── README.md
```

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/JanviBhateja/diabetesPrediction.git
```

2. Install the required libraries:

```bash
pip install numpy pandas scikit-learn
```

3. Open the Jupyter Notebook or Google Colab.

4. Run all cells sequentially.

5. Use the prediction section to test new patient data.

---

## Future Improvements

* Hyperparameter tuning for improved accuracy
* Confusion Matrix visualization
* Precision, Recall, and F1-Score analysis
* Streamlit web application deployment
* Model comparison with other classification algorithms

---

## Author

**Janvi Bhateja**

Second-Year B.Tech Student | Electronics and Computer Engineering

Passionate about Machine Learning, Software Development, and Problem Solving.
