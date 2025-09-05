

# Bank Loan Data Analysis

## About the Project

This project is an **end-to-end data analysis of bank loan applications** aimed at understanding customer behavior, financial risk, and portfolio health.

Banks operate in a high-risk environment where every loan decision affects profitability and credit exposure. By systematically analyzing historical loan data, we can:

* Track loan performance and repayment patterns
* Identify **Good vs Bad Loans**
* Understand borrower characteristics (employment, income, home ownership, loan purpose)
* Detect **seasonality and regional trends** in lending
* Support data-driven credit policies

The dataset provided is large:

* **Full dataset:** 38,000+ loan records (uploaded but not previewable on GitHub)
* **Sample dataset:** \~1,500 rows for quick testing, reproducibility, and public preview

This ensures anyone can explore the analysis easily without needing to download the massive file.

---

## Problem Statement

### **Business Requirement Document (BRD 1): KPI Summary**

The first goal was to compute key banking metrics that provide an **at-a-glance understanding of lending activities**:

* **Loan Applications** → Total and Month-to-Date (MTD) counts
* **Funded Amounts** → Total funds disbursed and MTD breakdown
* **Payments Received** → Total repayments collected and MTD tracking
* **Portfolio Health** →

  * *Average Interest Rate* → benchmark lending cost
  * *Average Debt-to-Income (DTI) Ratio* → borrowers’ repayment capacity
* **Loan Quality** → Segmentation into *Good vs Bad Loans*, capturing:

  * Application %
  * Counts
  * Funded amounts
  * Repayments

These KPIs form the **core health dashboard for bank management**.

---

### **Business Requirement Document (BRD 2): Visualization Overview**

The second goal was to build **clear, business-facing visuals** to uncover patterns in the loan portfolio:

* **Monthly Trends by Issue Date** → Detecting seasonal peaks and troughs in lending
* **Regional Analysis by State** → Identifying high-volume and high-risk geographies
* **Loan Term Analysis** → Comparing borrower preference between short-term (36 months) vs long-term (60 months) loans
* **Employment Length Analysis** → Measuring how job stability influences loan approval and repayment
* **Loan Purpose Breakdown** → Understanding the primary drivers behind loan demand (e.g., debt consolidation, credit card repayment, home improvement)
* **Home Ownership Analysis** → Studying how home ownership status affects loan disbursement and repayment patterns

These visualizations transform raw data into **business intelligence**, giving decision-makers both a macro and micro view of portfolio dynamics.

---

## Repository Structure

```
Bank-Loan-Analysis/
│── data/
│   ├── bank_loan_data_sample.csv   # ~1,500 rows for testing
│   ├── bank_loan_data_full.csv     # 38,000+ rows (not previewable on GitHub)
│   └── README.md                   # explains datasets
│
│── images/
│   ├── loan_trends.png
│   ├── loan_purpose.png
│   ├── home_ownership.png
│   └── ...
│
│── src/
│   ├── analysis.py                 # script version of notebook
│
│── BankLoanAnalysis.ipynb          # main Jupyter Notebook
│── requirements.txt
│── README.md                       # this file
│── LICENSE (optional)
```

---

##  Tech Stack

* **Python (3.x)**
* **Jupyter Notebook (Anaconda environment)**
* **Libraries Used**:

  * `pandas` → data cleaning & transformations
  * `numpy` → numerical operations
  * `matplotlib` & `seaborn` → visual storytelling and dashboard-style plots

---

## Key Insights & Business Value

* 📌 **Seasonality** → Loan disbursements showed consistent monthly spikes, indicating consumer borrowing behavior linked to certain periods.
* 📌 **Loan Purpose** → Debt consolidation dominated the portfolio, highlighting customer reliance on loans for financial restructuring.
* 📌 **Employment Length** → Borrowers with longer work experience exhibited lower default tendencies, validating employment as a key risk factor.
* 📌 **Home Ownership** → Borrowers with mortgages had a unique risk-return profile compared to those owning or renting homes.
* 📌 **Good vs Bad Loans** → Segmentation provided a **direct measure of portfolio risk**, helping in predictive credit modeling.
* 📌 **Regional Disparities** → Certain states contributed disproportionately to loan applications, suggesting targeted credit policies are required.

Together, these findings help banks **optimize approval policies, monitor risks, and strengthen long-term portfolio health**.

---

##  Conclusion

This project demonstrates how **data analysis transforms raw banking data into actionable insights**. By combining KPIs, borrower segmentation, and visualization, we:

* Created a **comprehensive loan portfolio dashboard**
* Identified **key borrower attributes affecting repayment**
* Highlighted **macro trends (seasonality, geography, purpose)**
* Distinguished **Good vs Bad Loans for better credit strategy**

The framework can be extended to build **predictive models** for loan default probability, automate risk scoring, and design **data-driven lending strategies**.

