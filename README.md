# Diabetes Prediction using Machine Learning

A complete end-to-end machine learning project to predict whether a patient is diabetic or non-diabetic based on medical diagnostic data. Trained on the **Pima Indians Diabetes Dataset** using Python and Scikit-learn.

---

## Demo Outputs

| Feature Distributions | Correlation Heatmap |
|---|---|
| ![Feature Distributions](feature_distributions.png) | ![Correlation Heatmap](correlation_heatmap.png) |

| Model Comparison | ROC Curve |
|---|---|
| ![Model Comparison](model_comparison.png) | ![ROC Curve](roc_curve.png) |

> Run the notebook to regenerate all plots.

---

## Dataset

**Pima Indians Diabetes Dataset** — 768 patient records, 8 medical features, binary classification target.

| Feature | Description |
|---|---|
| Pregnancies | Number of pregnancies |
| Glucose | Plasma glucose concentration |
| BloodPressure | Diastolic blood pressure (mm Hg) |
| SkinThickness | Triceps skin fold thickness (mm) |
| Insulin | 2-hour serum insulin (mu U/ml) |
| BMI | Body mass index |
| DiabetesPedigreeFunction | Genetic risk score |
| Age | Age in years |
| **Outcome** | **0 = Non-Diabetic, 1 = Diabetic** |

Class distribution: **500 Non-Diabetic / 268 Diabetic**

---

## Project Workflow

```
1. Data Loading & Exploration
        ↓
2. Exploratory Data Analysis (EDA)
   - Feature distributions
   - Correlation heatmap
   - Class imbalance analysis
        ↓
3. Data Preprocessing
   - Zero-value handling
   - Feature standardization (StandardScaler)
        ↓
4. Train-Test Split (Stratified, 80-20)
        ↓
5. Model Training & Comparison
   - Logistic Regression
   - Random Forest Classifier
   - Support Vector Machine (SVM) ← Best performer
        ↓
6. Evaluation
   - Accuracy, Precision, Recall, F1-Score
   - Confusion Matrix
   - ROC Curve & AUC Score
        ↓
7. Prediction System for new patient data
```

---

## Model Performance

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---|---|---|---|
| Logistic Regression | ~77% | ~77% | ~77% | ~77% |
| Random Forest | ~76% | ~76% | ~76% | ~75% |
| **SVM (Linear Kernel)** | **~77%** | **~77%** | **~77%** | **~77%** |

> SVM achieved the best overall F1-Score on the test set. Update table with your exact values after running the notebook.

---

## Technologies Used

- **Language:** Python 3
- **Libraries:** NumPy, Pandas, Scikit-learn, Matplotlib, Seaborn
- **Environment:** Google Colab / Jupyter Notebook
- **Version Control:** Git, GitHub

---

## Repository Structure

```
diabetesPrediction/
│
├── diabetesPrediction.ipynb   ← Main notebook (EDA + Models + Evaluation)
├── diabetes.csv               ← Dataset
├── feature_distributions.png  ← EDA plot
├── correlation_heatmap.png    ← EDA plot
├── class_distribution.png     ← EDA plot
├── model_comparison.png       ← Evaluation plot
├── confusion_matrix.png       ← Evaluation plot
├── roc_curve.png              ← Evaluation plot
└── README.md
```

---

## How to Run

1. Clone the repository:
```bash
git clone https://github.com/JanviBhateja/diabetesPrediction.git
cd diabetesPrediction
```

2. Install dependencies:
```bash
pip install numpy pandas scikit-learn matplotlib seaborn
```

3. Open the notebook:
```bash
jupyter notebook diabetesPrediction.ipynb
```
Or upload directly to **Google Colab**.

4. Run all cells sequentially. Plots are auto-saved as `.png` files.

5. Use the **Prediction System** cell at the end to test new patient data.

---

## Key Learnings

- Applied **feature standardization** to handle differing feature scales before SVM training
- Used **stratified train-test split** to preserve class ratio in imbalanced data
- Compared three classifiers — SVM outperformed others in F1-Score
- Visualized decision boundaries via **ROC curves** and **AUC scores**
- Identified **Glucose** and **BMI** as the strongest predictors via correlation analysis

---

## Author

**Janvi Bhateja**
B.Tech Electronics and Computer Engineering (2024–2028)
Thapar Institute of Engineering and Technology, Patiala


