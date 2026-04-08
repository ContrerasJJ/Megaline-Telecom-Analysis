# 📘 Megaline Telecom: User Behavior & Plan Profitability Analysis  

_Data Analysis • A/B Testing • Statistical Evaluation • Python • Pandas • Seaborn_

---

## 🔍 Project Summary  

Megaline, a telecom operator, offers customers two mobile plans — **Surf** and **Ultimate**.  
The company wants to understand **which plan generates more revenue** and **how users behave differently** across calls, messages, and internet usage.

This project analyzes customer behavior, evaluates plan profitability, and uses **statistical hypothesis testing** to determine whether the revenue difference between plans is statistically significant.

---

## 🎯 Objective  

- Compare customer usage patterns across Surf and Ultimate  
- Calculate monthly revenue per user  
- Analyze excessive usage (calls, texts, data) and overage charges  
- Statistically test whether one plan earns more than the other  
- Provide clear business recommendations to Megaline  

---

## 🛠️ Tools & Skills Used  

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- SciPy (t-test)  
- Exploratory Data Analysis (EDA)  
- Data Cleaning & Feature Engineering  
- Statistical Analysis & Hypothesis Testing  

---

## 🚀 Project Workflow  

### 1️⃣ Data Preparation  

- Loaded multiple datasets: calls, messages, internet, and user info  
- Merged them into a single monthly user-level dataset  
- Handled missing values and corrected data types  
- Calculated monthly totals for call minutes, number of messages, and internet usage (MB/GB)  

### 2️⃣ Exploratory Data Analysis (EDA)  

- Analyzed how much users call, text, and use data on each plan  
- Visualized distributions and usage patterns  
- Compared Surf vs. Ultimate users on:  
  - Call duration  
  - Number of SMS  
  - Internet usage  

### 3️⃣ Revenue Modeling  

For each user and month, I computed total revenue based on the tariff rules:

- Fixed monthly fee  
- Included limits for minutes, messages, and data  
- Overage charges when users exceeded their limits  

This produced **monthly revenue per user**, which became the main metric for comparison.

---

## 🧪 Statistical Hypothesis Testing  

- **H₀ (null):** There is **no difference** in average monthly revenue between Surf and Ultimate plans  
- **H₁ (alternative):** The average monthly revenue **differs** between the plans  
- Test: **Two-sided t-test**  
- Significance level: **α = 0.01**  

The test returned:

- **p-value = 3.63 × 10⁻¹⁶**

Since **p ≪ 0.01**, the result is **highly significant**.

---

## 📈 Key Insights  

- Internet usage is the **largest driver of revenue**  
- Surf users exceed plan limits **more frequently**, leading to overage charges  
- Ultimate users pay a **higher base fee** but go over limits less often  
- Revenue distributions for the two plans differ noticeably  
- **Conclusion from the test:**  
  - We **reject H₀** → the average monthly revenue between Surf and Ultimate users **differs significantly**  

---

## 🏁 Final Results & Business Impact  

- **Higher-earning plan:**  
  - Ultimate appears to be more profitable overall because of its higher base fee and stable revenue per user  

- **Statistical Significance:**  
  - **p-value = 3.63 × 10⁻¹⁶ < 0.01 → Reject H₀**  
  - The revenue difference between plans is **not due to chance**  

- **Business Recommendations:**  
  - Encourage heavy internet users to upgrade to **Ultimate**  
  - Offer targeted **add-on data packages** for Surf users who frequently exceed limits  
  - Use usage patterns to **segment customers** and personalize offers  
  - Consider marketing campaigns that move high-usage Surf customers to Ultimate to stabilize and grow revenue  

---

## 📦 Repository Structure  

```text
Megaline-Telecom-Analysis/
│── notebook-2.ipynb       # main analysis notebook
│── megaline_internet.csv  # sample dataset (internet usage)
│── README.md              # project documentation


## Conclusion

In this project, I analyzed customer behavior and revenue patterns for Megaline Telecom to identify opportunities for optimizing tariff plans.

Key outcomes:
- Identified usage patterns across customer segments to determine which plans generate the highest revenue
- Applied statistical hypothesis testing to validate differences in plan performance
- Uncovered insights showing how high-usage customers can be strategically targeted for plan upgrades

Business Impact:
- Recommended transitioning high-usage “Surf” users to the “Ultimate” plan to increase revenue
- Suggested targeted add-on packages to reduce churn and improve customer retention
- Demonstrated how data-driven segmentation can support personalized marketing strategies

This project highlights my ability to:
- Perform end-to-end exploratory data analysis using Python
- Apply statistical methods to real-world business problems
- Translate data insights into actionable business decisions

I’m excited to apply these skills in a Data Analyst or Data Scientist role to help organizations make smarter, data-driven decisions.
