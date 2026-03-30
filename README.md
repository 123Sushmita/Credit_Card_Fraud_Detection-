# Credit Card Fraud Detection

**Project Overview**  
Analyze credit card transactions to detect potential fraud using **Python**, **SQL**, and **Tableau**. The goal is to identify high-risk transactions and create a fraud scoring system.

---

## Project Objectives
- Explore patterns in fraudulent vs. non-fraudulent transactions  
- Detect high-risk transactions using multiple features  
- Visualize insights to support proactive decision-making  

---

## Dataset
**Location:** `data/creditcardFraud.csv`  

Columns:

| Column Name           | Description |
|-----------------------|-------------|
| transaction_id        | Unique transaction identifier |
| amount                | Transaction amount |
| transaction_hour      | Hour of transaction (0–23) |
| merchant_category     | Type of merchant |
| foreign_transaction   | 1 if foreign transaction, 0 otherwise |
| location_mismatch     | 1 if location differs from usual, 0 otherwise |
| device_trust_score    | Trust score of the device used |
| velocity_last_24h     | Number of transactions in last 24 hours |
| cardholder_age        | Age of cardholder |
| is_fraud              | 1 if fraudulent, 0 otherwise |

---

## Project Structure

Credit_Card_Fraud_Detection/
├─ data/               # Dataset
├─ notebooks/          # Python / Colab notebooks
├─ sql/                # SQL queries
├─ visualizations/     # Tableau screenshots
├─ README.md           # Documentation



---

## Python Analysis
**Notebook:** `notebooks/Credit_Card_Fraud_Analysis.ipynb`  

Key Steps:  
1. Data cleaning & exploration  
2. Fraud pattern analysis  
3. Feature-based fraud scoring  
4. Visualizations with **Matplotlib** & **Seaborn**  

---

## SQL Analysis
**File:** `sql/creditcardanalysis.sql`  

- Fraud scoring implemented using `CASE` statements  
- Aggregate queries for insights:  
  - Total vs fraudulent transactions  
  - Fraud percentages  
  - Analysis by merchant, hour, device score  

---

## Tableau Visualizations
**Folder:** `visualizations/`  

Examples:  
- Fraud vs Non-Fraud Count  
- Fraud by Transaction Amount  
- Fraud by Cardholder Age  
- Fraud by Hour of Day  
- Device Trust Score vs Fraud  
- Fraud by Merchant Category  
- Heatmap: Fraud by Hour vs Merchant Category  
- Velocity Last 24 Hours vs Fraud  

---

## Key Insights
- Fraud transactions often have **higher amounts** and **higher velocity**  
- **Foreign transactions** have a higher fraud probability  
- Low **device trust scores** and **location mismatches** increase risk  
- Combining multiple features improves fraud detection accuracy  
- Visualizations support actionable insights  

---

## Tools & Skills
- **Python:** Pandas, Matplotlib, Seaborn  
- **SQL:** Aggregation, CASE statements, fraud scoring  
- **Tableau:** Dashboards, binning, visual analysis  
- **GitHub:** Version control and portfolio sharing  
- **Data Analysis:** Pattern recognition, risk scoring, visualization




