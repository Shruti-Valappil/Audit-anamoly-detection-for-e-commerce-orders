# E-Commerce Audit Anomaly Dashboard (Olist Dataset)

This project identifies high-risk anomalies in an e-commerce dataset to simulate internal audit support for a Business Intelligence role. Using the Brazilian Olist dataset, I applied data cleaning and anomaly detection in Python, then visualized the results in Tableau.

## Objectives
- Detect transaction anomalies that may indicate fraud, pricing errors, or operational issues
- Create an interactive audit dashboard to support internal investigations

## Key Anomalies Flagged
1. **High-Quantity Orders** – Possible bulk misuse or reseller behavior
2. **Overpriced Products** – Prices >3× category median
3. **Frequent 1-Star Reviewers** – Potential refund abusers
4. **Suspicious Payments** – $0 or overpaid orders
5. **Late Deliveries + Bad Reviews** – Service failures tied to poor customer feedback

## Tools Used
- **Python (Pandas)** for ETL and anomaly detection
- **Tableau** for audit visualization
- **Jupyter Notebook** for preprocessing

## Dataset
Brazilian E-Commerce Public Dataset by [Olist (Kaggle)](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

## Outcome
An audit-ready dashboard that highlights key risks in order, payment, product, and review data—aligned with real-world internal audit analysis.
