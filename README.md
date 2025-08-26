

# 📊 Customer Churn EDA & Business Insights  

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![PowerBI](https://img.shields.io/badge/PowerBI-Dashboard-yellow)
![License](https://img.shields.io/badge/License-MIT-green)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adityamishra-22/customer-churn-eda-business-insights/blob/main/telco_churn_notebook_.ipynb)

---

## 📖 Project Overview  
This project performs **Exploratory Data Analysis (EDA)** on a Telco customer dataset to uncover factors influencing customer churn.  

### **Goals**
- Clean and prepare raw churn data.
- Engineer new features for deeper insights.
- Perform EDA to identify **high-risk churn segments**.
- Export a **dashboard-ready dataset** for Power BI / Tableau.
- Build **interactive Power BI dashboards** for churn insights.

---

## 🚀 Quickstart  

1. **Clone the repo**  
   
   git clone https://github.com/adityamishra-22/customer-churn-eda-business-insights.git
   cd customer-churn-eda-business-insights


2. **Open the notebook** in **Jupyter** or **Google Colab** → [Open in Colab](https://colab.research.google.com/github/adityamishra-22/customer-churn-eda-business-insights/blob/main/telco_churn_notebook_.ipynb)
3. **Run all cells** → outputs:

   * `telco_clean_DA.csv` → cleaned dataset
   * KPI metrics & churn insights
4. **Open Power BI file** → `Telco_Churn_Dashboard.pbix` → explore interactive visuals.

---

## 📂 Dataset Info

**Source:** Telco Customer Churn dataset (public domain)

| Column              | Description                                    |
| ------------------- | ---------------------------------------------- |
| customerID          | Unique ID for each customer                    |
| gender              | Male/Female                                    |
| SeniorCitizen       | 1 = Senior, 0 = Non-Senior                     |
| Partner, Dependents | Relationship info                              |
| tenure              | Months since becoming customer                 |
| Contract            | Month-to-month / One year / Two year           |
| PaymentMethod       | E-check, Auto-pay, Credit card, etc.           |
| MonthlyCharges      | Monthly billing amount                         |
| TotalCharges        | Total lifetime charges                         |
| Churn               | Yes/No → Whether the customer left the service |

---

## 🧮 KPIs Computed

| KPI Metric             | Formula / Definition                            |
| ---------------------- | ----------------------------------------------- |
| Overall Churn %        | Churned Customers ÷ Total Customers × 100       |
| Early-Tenure Churn %   | Churn where Tenure < 12 ÷ Total Tenure<12 × 100 |
| Contract Churn %       | Churn per Contract Type × 100                   |
| Payment Method Churn % | Churn per Payment Method × 100                  |
| High Spender Flag      | MonthlyCharges > Mean(MonthlyCharges)           |

---

## 📊 Key Insights

* **Month-to-month contracts** → highest churn rate (\~42%).
* **Electronic Check** users churn \~2× more than **Auto-Pay** users (\~45% vs <20%).
* **Tenure < 12 months** → \~3× higher churn risk vs long-tenure customers.
* **High monthly charges** → positively correlated with churn probability.

---

## 🖥️ Power BI Dashboard

An **interactive Power BI dashboard** was built using the cleaned dataset for better visualization:

**Key Features:**

* Overall Churn Rate KPI
* Churn by Contract Type
* Churn by Payment Method
* Churn Trend by Tenure
* High Spender & Month-to-Month Churn KPIs

**Screenshots:**

| Overall View                                 | 
| -------------------------------------------- | 
| <img width="1413" height="787" alt="Screenshot 2025-08-26 192841" src="https://github.com/user-attachments/assets/f16a538c-d5e0-435c-b028-80ad70200d67" />| 

> *Interactive `.pbix` file and static PDF snapshots available in the repo.*

---

## 📝 Business Actions

| Insight                              | Recommended Action                      |
| ------------------------------------ | --------------------------------------- |
| Month-to-month contract = high churn | Incentivize yearly plans with discounts |
| Electronic Check users churn more    | Push auto-pay adoption campaigns        |
| Tenure < 12 months churn more        | Retention offers in first 3–6 months    |
| High-Charge customers churn more     | Tiered pricing or loyalty discounts     |

---

## 🛠️ Tools & Libraries

* **Python**: pandas, numpy, matplotlib, seaborn
* **Jupyter Notebook / Colab**
* **Power BI**: interactive dashboards

---

## 📈 Next Steps

* Add churn prediction models (ML).
* Introduce confidence intervals for churn KPIs.
* Automate monthly churn reporting in Power BI Service.

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 🙌 Acknowledgements

* **Dataset**: Telco Customer Churn (Kaggle)
* **Visualization Inspiration**: Power BI Community


