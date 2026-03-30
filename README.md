# Credit_Card_Fraud_Detection-
Data analysis project: Credit card fraud detection using Python, SQL, and visualizations

## Project Overview
This project analyzes credit card transactions to detect potential fraud using Python, SQL, and data visualization. The goal is to identify high-risk transactions using a combination of transaction features and create a **fraud risk scoring system**.



## Dataset
The dataset contains the following columns:
- `transaction_id` – Unique transaction identifier
- `amount` – Transaction amount
- `transaction_hour` – Hour of transaction
- `merchant_category` – Type of merchant
- `foreign_transaction` – 1 if foreign, 0 otherwise
- `location_mismatch` – 1 if location differs from usual
- `device_trust_score` – Trust score of device used
- `velocity_last_24h` – Number of transactions in last 24 hours
- `cardholder_age` – Age of cardholder
- `is_fraud` – 1 if fraudulent, 0 if not



## Tools & Skills
- Python (Pandas, Matplotlib, Seaborn)
- SQL (CASE statements for fraud scoring)
- GitHub (portfolio and project sharing)
- Data Analysis & Visualization
- Fraud Detection & Risk Scoring


## Workflow

### Step 1: Data Exploration
- Checked for missing values and distribution of fraud
- Observed class imbalance: fraud is rare (~1–2%)

### Step 2: Pattern Analysis
- **Amount:** Fraud transactions tend to be higher
- **Velocity:** Fraud occurs in multiple transactions quickly
- **Foreign Transaction:** Foreign transactions have higher fraud rates
- **Device Trust Score:** Higher risk for some device trust levels
- **Location Mismatch:** Unusual locations more likely fraud

### Step 3: Fraud Scoring
- Created a **fraud_score** by combining risk indicators
- Each rule assigned points: high amount, high velocity, foreign transaction, device trust score, location mismatch
- Sorted transactions by fraud_score to identify highest-risk

### Step 4: SQL Implementation
- Fraud scoring translated into **SQL CASE statements**
- Enables **database-level risk scoring**

### Step 5: Visualization
- Countplot: Fraud vs Non-Fraud transactions
- Histogram: Transaction amounts by fraud
- Fraud Score distribution
- Correlation Heatmap for numeric features
- Scatter plot: Amount vs Fraud Score
- Fraud by Hour of Day

---

## Key Insights
- Fraud transactions have **higher amounts and velocity**
- Foreign transactions have a **much higher fraud rate**
- Combining multiple risk indicators improves **detection accuracy**
- Visualizations confirm patterns and support the scoring system

---

## Project Structure
