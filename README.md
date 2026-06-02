# 📊 Ecommerce Sales Dashboard — Power BI

An interactive **Ecommerce Sales Dashboard** built with **Power BI**, **Excel**, and **DAX** to analyze sales performance, customer behavior, payment trends, and profit across categories and Indian states.

---

## 🖼️ Dashboard Preview

![Ecommerce Sales Dashboard](dashboard_preview.png)

> *Built with Power BI Desktop | Data Source: Excel CSV Files*
>
> ## 📁 Project Structure

```
Power_BI_Sales_Dashboard/
│
├── Orders.csv          # Customer order data (Order ID, Date, Customer, State, City)
├── Details.csv         # Order details (Amount, Profit, Quantity, Category, Sub-Category, Payment Mode)
├── Sales_Dashboard.pbix  # Power BI report file
└── README.md

## 📂 Dataset Description

### `Orders.csv` — 501 rows
| Column        | Description                          |
|---------------|--------------------------------------|
| Order ID      | Unique identifier for each order (e.g., B-25681) |
| Order Date    | Date the order was placed (DD-MM-YYYY) |
| CustomerName  | Name of the customer                 |
| State         | Indian state where order was placed  |
| City          | City of delivery                     |

### `Details.csv`
| Column       | Description                              |
|--------------|------------------------------------------|
| Order ID     | Foreign key linking to Orders.csv        |
| Amount       | Total sale amount (₹)                    |
| Profit       | Profit earned on the order (₹)           |
| Quantity     | Number of items ordered                  |
| Category     | Product category (Electronics, Furniture, Clothing) |
| Sub-Category | Product sub-category (Printers, Saree, Bookcases, etc.) |
| PaymentMode  | Payment method used (COD, UPI, Credit Card, Debit Card, EMI) |
