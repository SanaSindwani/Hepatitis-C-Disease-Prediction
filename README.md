
# 🧬 Hepatitis C Disease Prediction

This project uses machine learning techniques to classify the stage of Hepatitis C disease based on biochemical markers. It includes exploratory data analysis, preprocessing, and model training using various classifiers.

---

## 📂 Dataset

The dataset used contains medical records with features such as:

- Age
- Sex
- ALB, ALP, ALT, AST (liver enzyme levels)
- BIL (bilirubin)
- CHE (cholinesterase)
- CHOL (cholesterol)
- PROT (protein)
- GGT (gamma-glutamyl transferase)
- Target: Disease category

The original dataset had missing values and an extra unnamed index column which were handled during preprocessing.

---

## 📊 Data Preprocessing

- Removed missing values
- Encoded categorical variables (`Sex` as 0/1 and `Category` into 0–3 classes)
- Dropped irrelevant columns
- Correlation heatmap to examine feature relationships

---

## 🔍 Exploratory Data Analysis (EDA)

- Visualizations with Seaborn and Matplotlib
- Heatmap showing correlations between liver enzyme values and disease stage

---

## 🤖 Models Used

Multiple classifiers were tested:

- **Support Vector Classifier (SVC)** — Best results with GridSearchCV
- **XGBoost**
- **Random Forest Classifier**

---

## 🏆 Best Model

The best performing model was:

- **SVC (Support Vector Classifier)**  
  **Best parameters:** `{'C': 10, 'gamma': 'scale', 'kernel': 'rbf'}`

---

## 📈 Evaluation Metrics

Model performance was evaluated using:

- Accuracy
- Confusion Matrix
- Cross-validation (via GridSearchCV)

---

## 🚀 How to Run

1. Clone the repository:
```bash
git clone https://github.com/SanaSindwani/Hepatitis-C-Disease-Prediction.git
cd Hepatitis-C-Disease-Prediction
```

2. Open the notebook:
```bash
jupyter notebook hepatitis-c-prediction.ipynb
```

3. Run all cells for data analysis, model training, and evaluation.

---

## 📌 Author

**Sana Sindwani**  
Data Science & Machine Learning Enthusiast  
[GitHub Profile](https://github.com/SanaSindwani)

