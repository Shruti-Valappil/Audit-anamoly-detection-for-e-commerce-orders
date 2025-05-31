# 🧾 Audit Anomaly Detection for E-Commerce Orders

This project identifies and visualizes anomalies in customer order behavior using data from the Brazilian e-commerce platform Olist. It is designed as an internal audit analytics project to uncover issues in logistics, pricing, and customer satisfaction that may go unnoticed in day-to-day operations.

## 📁 Dataset

The merged dataset includes key tables from the Olist database:
- Orders
- Order Items
- Products
- Customers
- Payments
- Reviews
- Sellers
- Product Category Translations

## 🔍 Anomalies Detected

The following five anomalies were flagged:

1. **Late Deliveries**
   - Orders where the delivered date exceeds the estimated delivery date.
2. **High Freight Charges Relative to Price**
   - Orders where freight cost is greater than the product price.
3. **Price Outliers**
   - Products priced significantly above or below the IQR (Interquartile Range).
4. **Low Review Score with High Price**
   - Expensive products (`> 75th percentile`) with poor customer ratings (`≤ 2`).
5. **Duplicate Order IDs**
   - Multiple rows with the same `order_id`, suggesting possible duplication or mismatched items.

Each anomaly is flagged as a boolean column and also summarized in a new column: `anomaly_type`.

## ⚙️ Technologies Used

- **Python** (Pandas, NumPy)
- **Jupyter Notebook**
- **Tableau** (for dashboard visualization)
- **CSV** export for Tableau integration
