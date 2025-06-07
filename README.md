# ❤️ Heart Disease Prediction

A machine learning project to predict the presence of heart disease using the **Kaggle Heart Disease Dataset**. The project uses data preprocessing, exploratory data analysis (EDA), feature engineering, and a Random Forest Classifier to achieve high prediction accuracy.

---

## 📊 Project Overview

- **Goal:** Binary classification – predict whether a patient has heart disease or not.
- **Dataset:** [Kaggle Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)
- **Model:** Random Forest Classifier (tuned with GridSearchCV)
- **Tools:** Python, Pandas, Scikit-learn, Seaborn, Matplotlib

---

## 🧱 Features Used

- `age`: Age of the patient
- `sex`: Sex (1 = male, 0 = female)
- `cp`: Chest pain type (0–3)
- `trestbps`: Resting blood pressure
- `chol`: Serum cholesterol (mg/dl)
- `fbs`: Fasting blood sugar > 120 mg/dl
- `restecg`: Resting electrocardiographic results
- `thalach`: Maximum heart rate achieved
- `exang`: Exercise-induced angina (1 = yes, 0 = no)
- `oldpeak`: ST depression induced by exercise
- `slope`: Slope of the ST segment
- `ca`: Number of major vessels (0–3)
- `thal`: Thalassemia (0 = normal, 1 = fixed defect, 2 = reversible defect)

---

## 🔍 Exploratory Data Analysis

- Checked for missing values
- Visualized class distribution (`target`)
- Correlation heatmap to analyze feature relationships
- Boxplots and pairplots for feature insights

---

## ⚙️ Preprocessing

- Scaled numerical features using `StandardScaler`
- Split dataset using `train_test_split()`

---

## 🤖 Model Training

- Trained multiple models, focused on **Random Forest Classifier**
- Evaluated using accuracy, classification report, ROC curve, and AUC score

---

## 📈 Performance

- **Best Accuracy:** ~100% (Random Forest Classifier)
- **AUC Score:** ~1.0
- ROC curve visualized to understand model performance under different thresholds

---

## 🔍 Example Prediction

```python
new_patient = {
    'age': 63,
    'sex': 1,
    'cp': 3,
    'trestbps': 145,
    'chol': 233,
    'fbs': 1,
    'restecg': 0,
    'thalach': 150,
    'exang': 0,
    'oldpeak': 2.3,
    'slope': 0,
    'ca': 0,
    'thal': 1
}
