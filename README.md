# 🌦️ Weather Prediction using Naive Bayes

This project involves predicting whether it will rain tomorrow using the **WeatherAUS dataset** and a **Naive Bayes Classifier**. It covers data preprocessing, label encoding, model training, and evaluation using scikit-learn.

---

## 📁 Dataset

- **File**: `weatherAUS.xlsx`
- **Target Variable**: `RainTomorrow` (Yes/No)
- **Description**: Contains daily weather observations across Australian weather stations with features like:
  - Location
  - MinTemp, MaxTemp
  - Rainfall
  - WindGustSpeed
  - Humidity
  - Pressure
  - Cloud
  - RainToday
  - RainTomorrow

---

## 🛠️ Tools and Libraries Used

- Python  
- Pandas  
- NumPy  
- Seaborn  
- Matplotlib  
- Scikit-learn  

---

## 🧼 Data Preprocessing

- Checked for missing values
- Imputed missing **numerical** values using the **mean**
- Imputed missing **categorical** values using the **most frequent** strategy
- Encoded categorical columns using **LabelEncoder**
- Dropped irrelevant columns like `Date`

---

## 🧠 Model Building

- Used all features except `RainTomorrow` and `Date` as input variables
- Target variable: `RainTomorrow`
- Performed **80/20 Train-Test Split**
- Trained the model using **Gaussian Naive Bayes (GaussianNB)** from scikit-learn
- Evaluated model performance using **accuracy score**

---

## ✅ Output

The model predicts whether it will rain tomorrow based on past weather conditions.

**Sample Output:** Accuracy: 0.90  
*Note: Accuracy may vary depending on random data split.*

---
