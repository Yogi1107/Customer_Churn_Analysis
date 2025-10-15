---

#  churn-analysis-eda

## 📊 Executive Summary

This repository contains the Exploratory Data Analysis (EDA) of customer data aimed at identifying key factors and patterns driving **customer churn**. The analysis found that **26.54%** of the customer base is churning.

The primary risk factors for attrition are concentrated in **new and shorter-term customers**, **senior citizens**, and those on **flexible contracts** utilizing specific payment methods.

*(For a high-level overview of the final results, please refer to the **Summary PDF** included in this repository.)*

---

## 📈 Key Findings and Churn Drivers

### 1. Contract Type is the Most Significant Driver

The **Month-to-month contract** is the primary churn driver. The count of churned customers on this contract type is substantially higher than for others.

### 2. Tenure and Early Churn

* **High-Risk Period:** Churn is highest among customers with very **low tenure** (e.g., 1-10 months). The churn percentage is at its peak for customers with just 1-2 months of service.
* **Retention Improves Over Time:** As customer tenure increases (e.g., 50+ months), the likelihood of churn decreases sharply.

### 3. Senior Citizens are a High-Risk Demographic

The churn rate for **Senior Citizens** is significantly higher at **41.7%**, compared to **23.7%** for non-Senior Citizens.

### 4. Service Subscriptions and Retention Value

While most customers are subscribed to services, **customers without certain value-added services are more likely to leave.**

| Service (Lack of) | Churn Correlation | Insight |
| :--- | :--- | :--- |
| **Online Security** | Very High | Absence is strongly associated with high churn counts. |
| **Tech Support** | Very High | Absence is strongly associated with high churn counts. |
| **Online Backup** | High | Lack of service leads to increased churn volume. |
| **Device Protection** | High | Lack of service leads to increased churn volume. |
| **Streaming TV/Movies** | Medium | Lack of service correlates with a lower likelihood of retention. |

### 5. Payment Method Friction

The **Electronic check** payment method accounts for the largest number of churned customers. This suggests potential friction in the payment process or a preference for automated billing among loyal customers.

---

## 🛠️ Strategic Recommendations

Based on these data-driven insights, the following areas should be prioritized for churn mitigation:

1.  **Incentivize Longer Contracts:** Develop targeted campaigns to migrate **Month-to-month** customers to **One-year or Two-year contracts**.
2.  **Enhance Early Retention:** Focus retention efforts and special offers on customers in their **first year of service** to push them past the highest-risk period.
3.  **Improve Service Adoption:** Aggressively promote the value of high-retention services, particularly **Online Security** and **Tech Support**, to encourage broader adoption across the customer base.
4.  **Optimize Payment Methods:** Analyze and address any issues with the **Electronic check** payment process, and implement campaigns to encourage migration to automatic, reliable payment options (Credit card or Bank transfer).
5.  **Target Senior Citizens:** Develop specific outreach or specialized support for this demographic to address their disproportionately high churn rate.

---

## 💻 Repository Contents

| File | Description |
| :--- | :--- |
| `EDA_Customer_churn.ipynb` | The core Jupyter Notebook containing the full data loading, cleaning, exploratory data analysis (EDA), visualizations, and initial conclusions. |
| **`Telco-Customer-Churn.csv`** | **The raw data file used for the entire analysis.** |
| **`Summary.pdf`** | **A presentation or detailed summary document of the key findings (PDF format).** |
| `README.md` | This file, providing a summary of the project and key findings. |

---
