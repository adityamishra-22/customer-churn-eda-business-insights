# customer-churn-eda-business-insights

## Project Overview
This project analyzes a Telco customer dataset to identify **factors driving customer churn**.  
It is designed as a **Data Analyst portfolio project**, focusing on **data cleaning, exploratory data analysis (EDA), feature engineering, and business insights**, without building any ML model.

---

## Dataset
- **Source:** [Telco Customer Churn Dataset](https://www.kaggle.com/blastchar/telco-customer-churn)  
- **Rows:** Each row represents a unique customer.  
- **Columns:** Demographics, services subscribed, account details, and churn flag (`Churn` = Yes/No).  

---

## Steps Performed
1. **Data Loading**  
   - Primary: GitHub RAW URL  
   - Fallback: Local CSV file in the same folder  

2. **Data Cleaning**  
   - Handle missing values (`TotalCharges` for tenure = 0)  
   - Convert numeric columns to correct datatypes  
   - Remove redundant or duplicate columns  

3. **Feature Engineering**  
   - **AverageCharges** = TotalCharges ÷ tenure  
   - **HighSpender** flag = MonthlyCharges > AverageCharges mean  
   - **ServicesMost** = Average number of services subscribed  

4. **Exploratory Data Analysis (EDA)**  
   - Churn by **Contract Type**  
   - Churn by **Payment Method**  
   - Churn vs **Tenure** and **MonthlyCharges**  
   - Churn vs **HighSpender** & **Service Usage**  
   - Correlation heatmaps for numeric features  

5. **Insights Generation**  
   - Key business insights about churn patterns printed in plain English.  

6. **Export**  
   - Clean dataset `telco_clean_DA.csv` ready for Power BI / Tableau dashboards.  

---

## Key Insights (Example)
- Month-to-month contract customers churn the most.  
- Electronic check users have higher churn than auto-pay customers.  
- Tenure < 12 months shows significantly higher churn.  
- High monthly charges correlate with higher churn risk.  
- Low service usage customers churn more than heavy users.  

---

## How to Run
1. Place the dataset CSV in the same folder as this notebook, or rely on the GitHub RAW URL.  
2. Open the notebook `telco_churn_notebook_.ipynb` in Jupyter/Colab.  
3. Click **Run All**.  
4. At the end, find `telco_clean_DA.csv` for dashboarding.  

---

## Next Steps
- Create **Power BI** or **Tableau** dashboards using the exported CSV.  
- Segment churn risk by **Contract + Tenure + PaymentMethod**.  
- Add **confidence intervals** to churn rates for business reporting.  

---

## Tools Used
- **Python:** pandas, numpy, matplotlib, seaborn  
- **Jupyter Notebook / Colab**  
- **Power BI / Tableau** (optional for visualization dashboards)  
