# 📊 Credit Risk Modelling – ML + Streamlit Web App

### 🔗 **Live App:** [https://rml-project-credit-risk-model.streamlit.app/](https://rml-project-credit-risk-model.streamlit.app/)

A fully functional **Machine Learning–based Credit Risk Prediction System** built using **Python, Logistic Regression, Streamlit**, and a custom credit scoring mechanism.
This project predicts **default probability**, generates a **credit score**, and classifies users into risk categories using real-time inputs.

---

## ✅ What I Built in This Project (My Work)

### **🔹 1. End-to-End Machine Learning Pipeline**

* Collected and cleaned credit data
* Performed feature engineering (Loan-to-Income, DPD, utilisation, etc.)
* Encoded categorical features
* Applied MinMax scaling on numerical columns
* Trained a **Logistic Regression model**
* Tuned the model to achieve high accuracy and stability
* Saved model, scaler, and metadata using **joblib**

---

### **🔹 2. Designed a Custom Credit Scoring System**

I created a custom scoring mechanism:

* Converts probability of default into a **300–900 score range**
* Maps score to human-friendly rating:

  * **Excellent**
  * **Good**
  * **Average**
  * **Poor**

---

### **🔹 3. Built a Complete Streamlit Web App (Frontend + Backend)**

* Designed a clean UI with 12+ interactive inputs
* Automatically calculates **Loan-to-Income ratio**
* Shows model results in real time:

  * Default Probability
  * Credit Score
  * Rating
* Added dropdowns for residence type, loan type & purpose
* Connected UI to ML model via `prediction_helper.py`
* Ensured smooth end-to-end inference

---

### **🔹 4. Project Deployment**

* Packaged the model and app
* Created `requirements.txt`
* Deployed the app on **Streamlit Cloud**
* Published the live link for public access

---

## 🚀 Features of the Application

* Real-time default prediction
* Automated credit score generation
* Transparent risk rating
* clean UI built using Streamlit
* End-to-end ML workflow from raw data → model → deployment

---

## 📂 Project Structure

```
📁 Credit-Risk-Model/
│── main.py                  # Streamlit UI
│── prediction_helper.py     # Preprocessing & prediction
│── requirements.txt         # Dependencies
│── artifacts/
│     └── model_data.joblib  # Trained model + scaler + metadata
│── README.md                # Documentation
```

---

## ▶️ Run This Project Locally

### **1. Clone the repo**

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
```

### **2. Install libraries**

```bash
pip install -r requirements.txt
```

### **3. Run the app**

```bash
streamlit run main.py
```

---

## 🧠 Model Details

* **Algorithm:** Logistic Regression
* **Frameworks:** scikit-learn, pandas, numpy
* **Scaling:** MinMaxScaler
* **Custom Score Formula:**

  ```
  credit_score = 300 + (1 - default_probability) * 600
  ```

---

## 📊 Rating Logic

| Score Range | Rating    |
| ----------- | --------- |
| 750–900     | Excellent |
| 650–749     | Good      |
| 500–649     | Average   |
| 300–499     | Poor      |

---

## 🌐 Live Demo

🔗 **Try your own inputs:**
👉 [https://rml-project-credit-risk-model.streamlit.app/](https://rml-project-credit-risk-model.streamlit.app/)

---

