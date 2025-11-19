Here is a clean, professional **README.md** you can directly add to your GitHub repo for this credit-risk Streamlit project:

---

# 📊 Credit Risk Modelling – Streamlit App

A machine-learning powered web application that predicts **default probability**, generates a **credit score**, and assigns a **risk rating** based on customer financial and behavioural features.
This project uses **Logistic Regression**, feature scaling, and a fully deployed **Streamlit UI**.

---

## 🚀 Features

* ⚡ **Real-time risk predictions** using a trained ML model
* 📈 **Default probability** shown in percentage
* ⭐ **Credit score (300–900)** generated dynamically
* 🏷️ **Rating levels:** Poor / Average / Good / Excellent
* 🎛️ Clean UI with interactive input fields
* 🧩 Encodes categorical variables and scales numerical features
* 🎒 Model and scaler are loaded from `artifacts/model_data.joblib`

---

## 🛠️ Tech Stack

* **Python 3.10+**
* **Streamlit** for UI
* **scikit-learn** for ML
* **pandas, numpy** for preprocessing
* **joblib** for model loading
* **xgboost** (used in training pipeline)

---

## 📂 Project Structure

```
📁 your-project/
│── main.py                  # Streamlit UI application
│── prediction_helper.py     # Preprocessing + prediction pipeline
│── requirements.txt         # Dependencies
│── artifacts/
│     └── model_data.joblib  # Trained model, scaler & metadata
│── README.md                # Project documentation
```

---

## ▶️ How to Run the Project Locally

### **1. Clone the repo**

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### **2. Install dependencies**

Make sure you have Python installed.

```bash
pip install -r requirements.txt
```

### **3. Run the Streamlit app**

```bash
streamlit run main.py
```

The app will open in your browser at:
👉 `http://localhost:8501`

---

## 🧠 Model Details

The ML model is trained using:

* Logistic Regression
* MinMaxScaler for selected numerical columns
* Encoded categorical variables
* Custom credit score calculation formula:

  ```
  credit_score = 300 + (1 - default_probability) * 600
  ```

Ratings are based on:

* 300–499 → **Poor**
* 500–649 → **Average**
* 650–749 → **Good**
* 750–900 → **Excellent**

---

## 🖥️ UI Inputs

The app collects:

* Age
* Income
* Loan Amount
* Loan Tenure
* Avg DPD
* Delinquency Ratio
* Credit Utilization
* No. of Open Accounts
* Residence Type
* Loan Type
* Loan Purpose

The backend prepares a dataframe → scales features → predicts → outputs results.

---


