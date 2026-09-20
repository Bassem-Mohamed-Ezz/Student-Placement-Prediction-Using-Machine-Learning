# AI-Based Student Placement Prediction

## Predicting Student Placement Potential Before the Interview Using Machine Learning

### 📌 Project Overview

This project aims to predict whether a student is likely to be placed before the interview stage using Machine Learning.

The system analyzes pre-interview student information such as academic performance, technical skills, projects, certifications, internships, and soft skills to predict the student's placement status.

The main goal is to help companies reduce unnecessary interview workload by identifying students who are more likely to be successfully placed.

---

## 🎯 Project Objective

The objective of this project is to build a Machine Learning classification model that predicts:

- **Placed**
- **Not Placed**

based on student-related features available before the interview.

---

## 📊 Dataset

The dataset contains information about students including:

- Age
- Gender
- University Year
- Major
- Study Hours Per Week
- CGPA
- Academic Performance
- Programming Skill
- Projects Completed
- Certifications
- Hackathons
- GitHub Profile
- Internships
- Leadership Experience
- LinkedIn Profile
- Communication Skills
- Teamwork
- Problem Solving
- English Proficiency

### Target Variable

`Placement_Status`

- `Placed` → 1
- `Not Placed` → 0

---

## 🧹 Data Preprocessing

The following preprocessing steps were applied:

1. Data cleaning
2. Handling categorical variables
3. Ordinal encoding for ordered categorical features
4. One-hot encoding for nominal categorical features
5. Binary encoding for binary features
6. Train-Test Split
7. Feature Scaling using StandardScaler
8. Handling class imbalance using SMOTE

---

## ⚖️ Class Imbalance

The dataset contains an imbalance between the two placement classes.

Therefore, **SMOTE (Synthetic Minority Over-sampling Technique)** was used to improve the representation of the minority class during model training.

---

## 🤖 Machine Learning Models

Several Machine Learning algorithms were evaluated, including:

- Random Forest
- Logistic Regression
- XGBoost
- AdaBoost

Different configurations were tested to compare their performance.

---

## 📈 Model Evaluation

The models were evaluated using multiple metrics:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

Accuracy alone was not considered sufficient because the dataset contains class imbalance.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn
- XGBoost
- Jupyter Notebook

---

## 📁 Project Structure

```text
Student-Placement-Classification/
│
├── README.md
├── requirements.txt
│
├── notebooks/
│   └── student_placement_classification.ipynb
│
├── data/
│   └── student_placement.csv
