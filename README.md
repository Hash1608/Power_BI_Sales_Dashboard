## Ecommerce Sales Dashboard

An interactive **Ecommerce Sales Dashboard** built with **Power BI**, **Excel**, and **DAX** to analyze sales performance, customer behavior, payment trends, and profit across categories and Indian states.

---

## Dashboard Preview

![Ecommerce Sales Dashboard](dashboard_preview.png)

> *Built with Power BI Desktop | Data Source: Excel CSV Files*
>
> ##  Project Structure

```
Power_BI_Sales_Dashboard/
│
├── Orders.csv          # Customer order data (Order ID, Date, Customer, State, City)
├── Details.csv         # Order details (Amount, Profit, Quantity, Category, Sub-Category, Payment Mode)
├── Sales_Dashboard.pbix  # Power BI report file
└── README.md

##  Dataset Description

### `Orders.csv` — 501 rows
| Column        | Description                          |
|---------------|--------------------------------------|
| Order ID      | Unique identifier for each order (e.g., B-25681) |
| Order Date    | Date the order was placed (DD-MM-YYYY) |
| CustomerName  | Name of the customer                 |
| State         | Indian state where order was placed  |
| City          | City of delivery                     |

### `Details.csv`— 1501 rows
| Column       | Description                              |
|--------------|------------------------------------------|
| Order ID     | Foreign key linking to Orders.csv        |
| Amount       | Total sale amount (₹)                    |
| Profit       | Profit earned on the order (₹)           |
| Quantity     | Number of items ordered                  |
| Category     | Product category (Electronics, Furniture, Clothing) |
| Sub-Category | Product sub-category (Printers, Saree, Bookcases, etc.) |
| PaymentMode  | Payment method used (COD, UPI, Credit Card, Debit Card, EMI) |

##  Dashboard Features & KPIs

###  Key Metrics (KPI Cards)
| Metric           | Value  |
|------------------|--------|
| Sum of Profit    | 37K    |
| Sum of Amount    | 438K   |
| Sum of Quantity  | 5,615  |
| Sum of AVG       | 121K   |

###  Visualizations

| Visual | Description |
|--------|-------------|
| **Total Sales by State** | Horizontal bar chart — Maharashtra leads with ₹102K, followed by Madhya Pradesh (₹87K) |
| **Category Performance** | Donut chart — Clothing (62.62%), Electronics (20.55%), Furniture (16.83%) |
| **Profit by Month** | Line chart — Monthly profit trend showing peaks in Jan–Feb and Nov, dips mid-year |
| **Top 6 Customers** | Bar chart — Harivansh leads at ₹9.9K, followed by Madhav (₹9.4K) |
| **Mode of Payments** | Pie chart — COD is most preferred (43.74%), followed by UPI (20.61%) |
| **Sales by Sub-Category** | Bar chart — Printers top at ₹8.6K, Bookcases at ₹6.5K |

###  Filters & Slicers
- **Quarter Slicer** — Filter data by Qtr 1, Qtr 2, Qtr 3, Qtr 4
- **Month Dropdown** — Drill down to a specific month

## Tools & Technologies
ToolUsagePower BI DesktopDashboard creation and data visualizationMicrosoft ExcelData storage and preprocessing (CSV format)DAX (Data Analysis Expressions)Custom calculated measures and KPIsPower QueryData transformation and relationship modeling

##  DAX Measures Used

```dax
-- Total Profit
Sum of Profit = SUM(Details[Profit])

-- Total Sales Amount
Sum of Amount = SUM(Details[Amount])

-- Total Quantity Sold
Sum of Quantity = SUM(Details[Quantity])

-- Average Order Value
Sum of AVG = AVERAGE(Details[Amount])

  Order ID  ─────────────────  Order ID

##  How to Use

1. **Clone the repository**
   ```bash
   git clone https://github.com/Hash1608/Power_BI_Sales_Dashboard.git
   ```

2. **Open in Power BI Desktop**
   - Launch Power BI Desktop
   - Open `Sales_Dashboard.pbix`

3. **Refresh Data Source** (if needed)
   - Go to `Home → Transform Data → Data Source Settings`
   - Update the file paths to point to `Orders.csv` and `Details.csv`

4. **Explore the Dashboard**
   - Use the **Quarter** and **Month** slicers to filter data interactively
   - Hover over charts for detailed tooltips
  
   - ## 💡 Key Insights

- 🏆 **Maharashtra** is the highest revenue-generating state (₹102K)
- 👗 **Clothing** dominates sales with over 62% of total category share
- 💳 **Cash on Delivery (COD)** is the most preferred payment method (43.74%)
- 📉 Profit dipped into negative territory during **June–September** months
- 🖨️ **Printers** are the top-selling sub-category by revenue (₹8.6K)
- 👤 **Harivansh** is the top customer by purchase value (₹9.9K)


## 👤 Author

**Hash1608**
- GitHub: [@Hash1608](https://github.com/Hash1608)
