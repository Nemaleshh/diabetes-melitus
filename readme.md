# 🩺 Diabetes Mellitus Prediction & Insulin Recommendation System  

🚀 **An AI-powered system to predict diabetes and recommend insulin dosage based on glucose levels and biomarkers.**  

---

## 📌 Table of Contents  
- [🔍 Problem Statement](#-problem-statement)  
- [💡 Solution Overview](#-solution-overview)  
- [📊 Mathematical Model](#-mathematical-model)  
- [✨ Features](#-features)  
- [🛠 Tech Stack](#-tech-stack)  
- [📥 Installation](#-installation)  
- [⚙️ Usage](#-usage)  
- [📊 Data Visualization](#-data-visualization)  
- [📜 License](#-license)  

---

## 🔍 Problem Statement  
Diabetes mellitus, especially autoimmune-related cases, often remains undiagnosed until after the age of 20, leading to severe health complications. This system provides **early detection** and **personalized insulin recommendations** to improve patient outcomes.  

---

## 💡 Solution Overview  
This system leverages **machine learning (ML) and mathematical models** to:  
✔ Predict the likelihood of diabetes based on biomarkers (Glucose, HbA1c, GAD antibodies, etc.).  
✔ Recommend insulin dosages based on blood glucose levels.  
✔ Provide interactive visualizations for better patient insights.  

---

## 📊 Mathematical Model  

### 1️⃣ **Diabetes Prediction Model**  
The model is trained on biomarkers to classify **diabetes risk** using a logistic regression formula:  
![alt text](image.png)
Where:  
- \( X_1, X_2, ... X_n \) = Features (Glucose, HbA1c, GAD antibodies, etc.)  
- \( \beta_0 \) = Intercept  
- \( \beta_1, \beta_2, ... \beta_n \) = Coefficients  

If \( P(Diabetes) > 0.5 \), the patient is **classified as diabetic**.  

### 2️⃣ **Insulin Recommendation Formula**  
The insulin dosage is calculated using the **correction factor and carbohydrate ratio**:

![alt text](image2.png)

Where:  
- **Target Glucose** = Ideal blood glucose level (e.g., 100 mg/dL)  
- **Insulin Sensitivity Factor (ISF)** = Reduction in glucose per unit of insulin  
- **Insulin-to-Carb Ratio (ICR)** = Carbohydrates covered by 1 unit of insulin  

Example Calculation:  
- If Blood Glucose = 250 mg/dL  
- Target Glucose = 100 mg/dL  
- ISF = 50  
- Carbohydrates = 60g  
- ICR = 10  

Then:
![alt text](image-1.png)

---

## ✨ Features  
✅ **AI-Powered Diabetes Prediction**  
✅ **Personalized Insulin Recommendations**  
✅ **Real-Time Visualizations**  
✅ **User-Friendly Web Interface**  

---

## 🛠 Tech Stack  
🔹 **Machine Learning**: Scikit-learn, XGBoost, Random Forest  
🔹 **Data Handling**: Pandas, NumPy  
🔹 **Backend**: Python, Flask  
🔹 **Visualization**: Matplotlib, Seaborn  
 

---

## 📥 Installation  

### Prerequisites  
Ensure **Python 3.7+** is installed, then run:  

```bash
python model.ipynb

