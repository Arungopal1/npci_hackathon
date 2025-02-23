# 🚀 UPI Fraud Detection System using LSTM & XGBoost  



## 📌 Overview  
**UPI Fraud Detection System** is an advanced AI-powered fraud detection solution that analyzes transaction patterns using **Deep Learning & Machine Learning**. It combines the power of **LSTM with Attention Mechanism** and **XGBoost** to deliver high-accuracy fraud predictions.  

🔹 **LSTM** learns sequential transaction behaviors 📈  
🔹 **XGBoost** analyzes structured fraud patterns 🚀  
🔹 **Ensemble Learning** combines both models for superior accuracy 🎯  

## 🎯 Key Features  
✅ **Automated Data Preprocessing & Feature Engineering**  
✅ **Class Imbalance Handling with SMOTE**  
✅ **Optimized XGBoost with Hyperparameter Tuning**  
✅ **LSTM with Attention for Sequential Data Analysis**  
✅ **Hybrid Ensemble Model (XGBoost + LSTM + Logistic Regression)**  
✅ **Performance Evaluation with Confusion Matrix, ROC, and PR Curves**  

---  

## 📂 Dataset Details  
- **Source**: Custom UPI transaction dataset in **JSON format**.  
- **Target Variable**: `"Fraud_Label"` (1 = Fraud, 0 = Legitimate).  
- **Preprocessing**:  
  - Missing values imputed with **median values**.  
  - **Categorical encoding** applied using **Label Encoding**.  
  - Highly correlated features removed.  
  - Data **normalized** using `StandardScaler()`.  

---  

## 🏗️ Model Architecture  

### **1️⃣ XGBoost Classifier**  
✔ **Gradient Boosted Trees** for structured fraud detection.  
✔ **RandomizedSearchCV** for hyperparameter tuning.  
✔ Outputs probability scores for fraud classification.  

### **2️⃣ LSTM with Attention**  
✔ **Bidirectional LSTM** for sequential pattern learning.  
✔ **Attention Mechanism** to focus on key transaction features.  
✔ Outputs fraud probabilities based on historical data.  

### **3️⃣ Ensemble Meta Model (Logistic Regression)**  
✔ **Combines XGBoost & LSTM outputs** for enhanced accuracy.  
✔ **Reduces false positives & false negatives**.  
✔ Final decision-making layer.  

---  

## 📊 Model Evaluation Metrics  

📌 **Confusion Matrix** 🔍  
Visual representation of model predictions vs actual labels.  

📌 **ROC Curve** 📈  
Shows True Positive Rate vs False Positive Rate.  

📌 **Precision-Recall Curve** 🎯  
Measures model's ability to detect fraud cases.  

✅ **Final Accuracy:** Displayed in the console.  

---  

## ⚙️ Installation & Setup  

### **Step 1: Clone the Repository**  
```bash
git clone https://github.com/yourusername/UPI-Fraud-Detection.git
cd UPI-Fraud-Detection
```

### **Step 2: Install Dependencies**  
```bash
pip install -r requirements.txt
```

### **Step 3: Run the Model**  
```bash
python fraud_detection.py
```

---  

## 📜 Outputs  

🔹 **Trained Models:**  
- ✅ `xgb_fraud_model.pkl` (XGBoost Model)  
- ✅ `lstm_fraud_model.keras` (LSTM Model)  
- ✅ `meta_model.pkl` (Final Ensemble Model)  

🔹 **Preprocessing Assets:**  
- 📌 `scaler.pkl` (Standard Scaler)  
- 📌 `label_encoders.pkl` (Label Encoders)  

🔹 **Performance Plots:**  
- 📊 Confusion Matrix  
- 📈 ROC Curve  
- 🎯 Precision-Recall Curve  

---  

## 🎨 Visualizations  

📌 **Confusion Matrix Example**  
![Confusion Matrix](https://github.com/Arungopal1/npci_hackathon/blob/main/src/Output%20images/confusionmatrix.png)  

📌 **ROC Curve Example**  
![ROC Curve](https://github.com/Arungopal1/npci_hackathon/blob/main/src/Output%20images/Roc%20curve.png)  

---  

## 💡 Future Improvements  

🚀 Implement **Real-Time Fraud Detection API**  
🔍 Integrate **Explainable AI (SHAP values)** for fraud justification  
📊 Improve dataset **feature engineering techniques**  
💾 **Deploy model as a REST API using FastAPI**  

---  
