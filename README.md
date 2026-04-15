
# 🌳 Decision Tree Classifier – Heart Disease Prediction

## 📌 Project Overview
This project implements a **Decision Tree Classifier** to predict the presence of heart disease based on patient medical data. It covers the complete machine learning workflow including **EDA, preprocessing, model building, evaluation, and hyperparameter tuning**.

---

## 🎯 Objective
- Apply Decision Tree Classification on a real-world dataset  
- Perform data preprocessing and feature engineering  
- Evaluate model performance using multiple metrics  
- Optimize model using hyperparameter tuning  
- Interpret results using visualization and feature importance  

---

## 📂 Dataset
- **File:** `heart_disease.xlsx`  
- Contains features such as:
  - Age, Sex  
  - Chest pain type (`cp`)  
  - Resting ECG (`restecg`)  
  - Cholesterol, Blood Pressure  
  - Maximum heart rate  
  - Target variable (`num`) → Heart disease presence  

---

## 🔍 Exploratory Data Analysis (EDA)
- Checked dataset structure using `.info()` and `.describe()`  
- Identified missing values and duplicates  
- Detected outliers using:
  - Boxplots  
  - IQR (Interquartile Range) method  
- Visualizations performed:
  - Histograms for feature distribution  
  - Pairplot for relationships  
  - Correlation heatmap  
  - Target class distribution  

---

## ⚙️ Data Preprocessing & Feature Engineering

### Outlier Handling
- Removed outliers using IQR method  
- Applied capping (winsorization) to limit extreme values  

### Encoding Techniques
- Label Encoding for categorical variables  
- One-Hot Encoding using `pd.get_dummies()`  

### Feature Scaling
- Applied Standard Scaling using `StandardScaler`  

### Target Transformation
- Converted target variable into binary:
  - `0 → No Disease`
  - `1 → Disease`

---

## 🤖 Model Building – Decision Tree
- Split dataset into:
  - 80% Training  
  - 20% Testing  
- Trained using `DecisionTreeClassifier`  

---

## 📊 Model Evaluation
Performance evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1-Score  
- Confusion Matrix  
- ROC-AUC Score  

Visualizations:
- ROC Curve  
- Decision Tree Structure  

---

## 🔧 Hyperparameter Tuning
Used **GridSearchCV** to optimize:
- `criterion` (gini / entropy)  
- `max_depth`  
- `min_samples_split`  
- `min_samples_leaf`  

✔ Improved model performance after tuning  

---

## 🌳 Model Interpretation
- Visualized decision tree using `plot_tree()`  
- Extracted feature importance to identify key predictors  

---

## 💡 Key Learnings
- Understanding how Decision Trees split data using Gini and Entropy  
- Importance of hyperparameter tuning to avoid overfitting  
- Handling outliers improves model stability  
- Difference between Label Encoding and One-Hot Encoding  
- Model interpretability using tree visualization and feature importance  

---

## 🧠 Interview Questions

### 1. What are common hyperparameters of Decision Trees?
- `max_depth` → Controls tree depth (overfitting vs underfitting)  
- `min_samples_split` → Minimum samples to split a node  
- `min_samples_leaf` → Minimum samples in a leaf node  
- `criterion` → Split quality (gini / entropy)  

👉 Proper tuning balances bias and variance  

---

### 2. Label Encoding vs One-Hot Encoding

| Feature | Label Encoding | One-Hot Encoding |
|--------|----------------|------------------|
| Output | Integer values | Binary columns |
| Use Case | Ordinal data | Nominal data |
| Risk | Introduces false order | High dimensionality |

---

## 🛠️ Tech Stack
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## 🚀 How to Run

bash
git clone https://github.com/MeghanaCVarghese/Decision-Tree-Classifier
pip install -r requirements.txt


# Open Jupyter Notebook
jupyter notebook

---

## 👩‍💻 Author

*Meghana C Varghese*
