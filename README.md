# 🎯 Heart Disease Prediction using Machine Learning ❤️

## 🏥 Overview
This project aims to **predict heart disease** using machine learning techniques. The dataset used is the **Heart Disease Dataset** from Kaggle, which contains various patient health metrics. The model is built using a **Random Forest Classifier** to classify whether a patient is at risk of heart disease. 🩺

---
## 📂 Dataset
**🔗 Source:** [Kaggle - Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)

### 🧬 Features:
✅ **Age, Sex**  
✅ **Chest Pain Type (CP)**  
✅ **Resting Blood Pressure (Trestbps)**  
✅ **Cholesterol Level (Chol)**  
✅ **Fasting Blood Sugar (Fbs)**  
✅ **Resting ECG Results (Restecg)**  
✅ **Maximum Heart Rate Achieved (Thalach)**  
✅ **Exercise Induced Angina (Exang)**  
✅ **ST Depression Induced by Exercise (Oldpeak)**  
✅ **Target Variable:** Presence of heart disease (💔 = Yes, ❤️ = No)  

---
## 🚀 Installation & Setup
### 🖥️ 1. Clone the Repository
```bash
git clone https://github.com/yourusername/heart-disease-prediction.git
cd heart-disease-prediction
```

### 📦 2. Install Required Dependencies
```bash
pip install -r requirements.txt
```

### 📑 3. Run the Jupyter Notebook
```bash
jupyter notebook
```
Open **`heart_disease_prediction.ipynb`** and run the cells to execute the project.

---
## 📝 Code Explanation

### 📌 Data Processing & Feature Selection
The dataset is first explored for missing values and data distributions. A correlation heatmap is used to identify relationships between features, helping in feature selection. **Highly correlated features** may provide redundant information, so feature importance is analyzed.

### 📌 Data Splitting & Scaling
The dataset is split into **training (80%) and testing (20%)** subsets to ensure that the model learns from historical data and generalizes well to new, unseen cases. Since numerical features have varying scales, **StandardScaler** is used to normalize them, improving model performance.

### 📌 Why Random Forest?
Random Forest is an **ensemble learning method** that combines multiple decision trees to improve classification accuracy and reduce overfitting. Here’s why it was chosen:
- 🌳 **Handles Non-Linearity:** Unlike linear models, it captures complex relationships between variables.
- 🔄 **Reduces Overfitting:** By averaging multiple decision trees, it generalizes well to unseen data.
- 📊 **Feature Importance:** It provides insights into which features contribute the most to predictions.
- ⚡ **Robust to Missing Data & Noise:** It can handle noisy and missing data better than single decision trees.

### 📌 Model Training & Evaluation
A **Random Forest Classifier with 100 trees** is trained using the preprocessed dataset. The trained model is evaluated using:
- ✅ **Accuracy Score** – Measures overall correctness of predictions.
- ✅ **Classification Report** – Provides **precision, recall, and F1-score** for both classes.
- ✅ **Confusion Matrix** – Visualizes correct vs. incorrect predictions.

The confusion matrix helps understand false positives (misclassified healthy patients) and false negatives (missed heart disease cases), which are crucial for healthcare applications.

---
## 🎯 Results
The model achieves a **high accuracy** in predicting heart disease, making it useful for **preliminary risk assessment** in healthcare applications. 🚑

### 🔍 Key Performance Metrics:
- **Accuracy Score:** The model achieved an accuracy of around **85-90%**, indicating strong predictive capability.
- **Precision & Recall:**
  - **Precision** (how many of the positive predictions were actually correct) was **high**, meaning the model effectively identifies patients with heart disease.
  - **Recall** (how many actual positive cases were correctly identified) was balanced, ensuring fewer false negatives (missed cases of heart disease).
- **Confusion Matrix Analysis:**
  - **True Positives (TP):** Cases correctly identified as heart disease.
  - **True Negatives (TN):** Cases correctly identified as non-heart disease.
  - **False Positives (FP):** Healthy patients incorrectly classified as having heart disease (overdiagnosis).
  - **False Negatives (FN):** Patients with heart disease incorrectly classified as healthy (underdiagnosis, which is riskier in a medical setting).

### 📊 Insights from the Results:
- The model shows **strong predictive performance**, but reducing false negatives is crucial to avoid missing real heart disease cases.
- **Feature importance analysis** reveals that factors like **chest pain type, maximum heart rate, and ST depression** are among the most influential predictors.
- The balance between **precision and recall** suggests the model is well-suited for **early risk assessment**, but should be used alongside expert diagnosis.

---
## 🔮 Future Improvements
🔹 **Hyperparameter tuning** to improve performance.  
🔹 **Deploying the model** as a web application using **Streamlit or Flask**.  
🔹 **Incorporating additional healthcare datasets** for better generalization.  

---
## 👨‍💻 Author
🔗 **Meghana** - [LinkedIn](https://www.linkedin.com/in/bgem/)  


