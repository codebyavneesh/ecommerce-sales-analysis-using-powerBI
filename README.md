# 🛒 E-Commerce Sales Analysis

A data analysis project focused on uncovering **sales trends and revenue patterns** in e-commerce data using Python, SQL, and Jupyter Notebook.

---

## 📁 Project Structure

```
ecommerce-sales-analysis/
│
├── ecommerce_sales_analysis.ipynb   # Main analysis notebook
├── dataset/                         # Raw source data (CSV files)
│   ├── customers.csv                # Customer details (id, name, city, etc.)
│   ├── orders.csv                   # Order records (id, product, quantity, price, date)
│   └── products.csv                 # Product catalogue (id, name, category, price)
├── exports/                         # Exported charts and result files
├── screenshots/                     # Visualizations and chart snapshots
└── README.md
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Python** | Data processing & analysis |
| **SQL** | Data querying & transformation |
| **Jupyter Notebook** | Interactive analysis environment |
| **Pandas** | Data manipulation |
| **Matplotlib / Seaborn** | Data visualization |

---

## 📊 Project Overview

This project analyzes e-commerce sales data to identify key revenue trends, seasonal patterns, and business performance metrics using SQL queries inside Python, with results visualized through Matplotlib charts.

**💵 Total Company Revenue: ₹5,37,510.00**

---

## 🗃️ Dataset

All source data is stored in the [`dataset/`](https://github.com/codebyavneesh/ecommerce-sales-analysis-using-python-mysql/tree/main/ecommerce-sales-analysis/datasets) folder. Three CSV files are used:

| File | Description | Columns |
|------|-------------|---------|
| `customers.csv` | Customer master data | `customer_id`, `customer_name`, `city`, `email`, `signup_date` |
| `orders.csv` | All order transactions | `order_id`, `customer_id`, `product_id`, `quantity`, `payment_method`, `order_date` |
| `products.csv` | Product catalogue | `product_id`, `product_name`, `category`, `price` |

> These three tables are loaded into SQL (via Python) and joined together to perform all the analysis below.

---

## 📈 Key Analysis & Outputs

### 1. 🏆 Top 10 Highest Selling Products
> Which products have the highest total quantity sold?

SQL fetches product-wise total quantity from orders, grouped and sorted descending — displayed as a **bar chart**.

![Top 10 Highest Selling Products](https://github.com/codebyavneesh/ecommerce-sales-analysis-using-python-mysql/blob/main/ecommerce-sales-analysis/screenshots/top_10_highest_selling_product.png)

---

### 2. 💰 Top 10 Highest Spenders
> Who are the customers spending the most overall?

Customer-level revenue aggregation using SQL JOIN across orders, products, and customers tables — visualized as a **bar chart**.

![Top 10 Highest Spenders](https://github.com/codebyavneesh/ecommerce-sales-analysis-using-python-mysql/blob/main/ecommerce-sales-analysis/screenshots/top_10_highest_spender.png)

---

### 3. 🧾 Top 10 Average Spenders
> Which customers have the highest average order value?

Average spend per customer calculated via SQL — highlights premium/high-value buyers — shown as a **bar chart**.

![Top 10 Average Spenders](https://github.com/codebyavneesh/ecommerce-sales-analysis-using-python-mysql/blob/main/ecommerce-sales-analysis/screenshots/top_10_average_spender.png)

---

### 4. 🏙️ Revenue of Each City
> Which cities contribute the most to total revenue?

City-wise revenue breakdown using SQL `GROUP BY` on customer location joined with order data — plotted as a **bar chart**.

![Revenue of Each City](https://github.com/codebyavneesh/ecommerce-sales-analysis-using-python-mysql/blob/main/ecommerce-sales-analysis/screenshots/revenue_of_each_city.png)

---

### 5. 📅 Monthly Trend Analysis
> How does revenue change month over month?

Time-series analysis using SQL date functions to extract monthly revenue — displayed as a **trend chart** to spot peak and slow seasons.

![Monthly Trend Analysis](https://github.com/codebyavneesh/ecommerce-sales-analysis-using-python-mysql/blob/main/ecommerce-sales-analysis/screenshots/monthly_trend_analysis.png)

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/ecommerce-sales-analysis.git
   cd ecommerce-sales-analysis
   ```

2. **Install dependencies**
   ```bash
   pip install pandas matplotlib seaborn jupyter
   ```

3. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook ecommerce_sales_analysis.ipynb
   ```

4. Run all cells from top to bottom.

---

## 📤 Exports

Processed chart files and CSVs are saved in the [`exports/`](https://github.com/codebyavneesh/ecommerce-sales-analysis-using-python-mysql/tree/main/ecommerce-sales-analysis/exports) folder for easy sharing and reference.

---

## 👤 Author

**Your Name**
- GitHub: [@codebyavneesh](https://github.com/codebyavneesh)
