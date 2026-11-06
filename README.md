# EduPredict – Student Performance Prediction & Analysis

## Project Overview
EduPredict is a machine learning classification project developed as part of the Stack & Scale AI Engineering Internship – Week 02.

The project analyzes student educational and personal information and predicts academic performance categories using Logistic Regression.

## Dataset
- Source: UCI Machine Learning Repository
- Dataset: Student Performance (Mathematics)
- Records: 395
- Original Features: 33

## Performance Categories
The final grade (G3) is converted into three categories:

- Low: 0–9
- Average: 10–14
- High: 15–20

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Google Colab

## Project Workflow
1. Dataset loading and inspection
2. Exploratory Data Analysis
3. Performance category creation
4. Data preprocessing
5. Train/test splitting
6. Logistic Regression model training
7. Majority-class baseline comparison
8. Model evaluation
9. Prediction demonstration

## Data Preprocessing
- Missing value handling using SimpleImputer.
- Numerical feature scaling using StandardScaler.
- Categorical feature encoding using OneHotEncoder.
- Preprocessing using ColumnTransformer and Pipeline.

## Data Leakage Prevention
G1, G2, and G3 are excluded from input features. G3 is used only to create the target performance category.

Preprocessing is fitted on training data to avoid information leakage from the test set.

## Model Evaluation
The model is evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

The model is also compared against a majority-class baseline.

Actual evaluation results are available in the notebook.

## Repository Structure
```text
EduPredict/
├── EduPredict.ipynb
├── edupredict_model.pkl
├── README.md
├── requirements.txt
└── screenshots/
```

## How to Run
1. Clone or download this repository.
2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open EduPredict.ipynb using Jupyter Notebook or Google Colab.
4. Run the notebook cells from beginning to end.

## Limitations
- The dataset contains a relatively small number of students.
- Results may not generalize to other educational institutions.
- Student performance depends on many factors.
- This project is for educational purposes and not for automated grading or admissions decisions.

## Dataset Reference
Cortez, P. (2008). Student Performance. UCI Machine Learning Repository.

Dataset: https://archive.ics.uci.edu/dataset/320/student+performance

## Project Information
**Internship:** Stack & Scale – AI Engineering Internship 2026

**Project:** Week 02 – EduPredict
