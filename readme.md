# Customer Churn Prediction & Retention Analytics

An end-to-end Machine Learning web application designed to predict customer churn, identify key risk factors, and help businesses proactively retain valuable customers. 

🔗 **Live App:** [View Streamlit Application](https://customerchurnprediction-zkbeoitb8v2dkq45n7wnto.streamlit.app/)

---

## About the Project
Customer churn is one of the most critical metrics for subscription and service-based businesses. Acquiring new customers is significantly more expensive than retaining existing ones. 

This project tackles the churn problem by:
- Analyzing historical customer demographics, account details, and usage behavior.
- Training a robust predictive model to flag customers at high risk of leaving.
- Providing an interactive web interface where users can input customer details and instantly generate real-time churn predictions along with actionable risk insights.

---

## Tech Stack & Libraries
- **Language:** Python
- **Machine Learning & Modeling:** Scikit-Learn, Pandas, NumPy
- **Web App & Deployment:** Streamlit Cloud
- **Data Visualization:** Matplotlib / Seaborn

---

## Key Features
- **Real-Time Predictions:** Enter customer attributes (such as tenure, monthly charges, contract type, and services used) into the sidebar controls and instantly see whether the customer is likely to churn.
- **Interactive UI:** Clean, responsive, and intuitive dashboard built with Streamlit.
- **Actionable Insights:** Understand the core drivers behind customer attrition to shape targeted retention campaigns.

---

## How to Run Locally

If you'd like to run this project on your local machine, follow these simple steps:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Shaikh-Mazher01/Customer_Churn_Prediction.git](https://github.com/Shaikh-Mazher01/Customer_Churn_Prediction.git)
   cd Customer_Churn_Prediction

2. **Install the required dependencies:**
   ```bash
   pip install -r requirements.txt

3. **Launch the Streamlit app:**
   ```bash
   streamlit run app.py

## Project Structure
```text
Customer_Churn_Prediction/
├── App
│   └── app.py                   # Main Streamlit application script
├── Models
│   └── logistic_model.pkl       # Trained Logistic Regression model
│   └── rf_model.pkl             # Trained Random Forest model
├── notebook
│   └── Customer_Churn_Prediction.ipynb              # Notebook
├── .gitignore       
├── requirements.txt             # Project dependencies
└── README.md                    # Project documentation
```

---

## 🤖 Models Used
- **Logistic Regression:** 
  - Baseline interpretable model.
  - High recall, making it excellent at catching true churn customers.
- **Random Forest:** 
  - Powerful ensemble model.
  - Capable of capturing complex, non-linear relationships with balanced performance across metrics.

---

## 🔍 Model Explainability (SHAP)
To ensure transparency and trust in the predictions, **SHAP** was integrated to decode model decisions:
- Explains individual customer predictions.
- Identifies global feature importance across the dataset.
- Highlights exact drivers behind a customer's churn risk.

### **Key Insights from SHAP:**
- 📉 **Low tenure** $\rightarrow$ Higher churn risk.
- 📉 **Month-to-month contracts** $\rightarrow$ Strongest churn driver.
- 📈 **Higher monthly charges** $\rightarrow$ Increased churn probability.
- ❌ **Lack of core services** (online security, tech support) $\rightarrow$ Higher vulnerability.

---

## 💼 Business Recommendations
Translating model insights into actionable business strategies:
- **Encourage Long-Term Commitment:** Introduce discounts or incentives to shift customers from month-to-month to annual contracts.
- **Service Bundling:** Promote add-on services (like tech support and security packages) to increase platform stickiness.
- **Proactive Retention:** Focus retention offers and loyalty discounts on high-paying customers before they show cancellation intent.
- **New Customer Onboarding:** Build targeted engagement workflows for new users who are still within their low-tenure window.

---
