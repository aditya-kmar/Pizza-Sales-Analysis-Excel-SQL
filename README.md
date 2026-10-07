# 🍕 Pizza Sales Analysis Dashboard

An interactive **Pizza Sales Analysis Dashboard** built using **Excel and SQL** to analyze sales performance, customer ordering patterns, revenue, order trends, pizza categories, pizza sizes, and top-performing pizzas.

The dashboard provides a clear view of overall business performance and helps identify the best-selling products and peak ordering periods.

---

## 📊 Dashboard Preview

Pizza Sales Dashboard<img width="1397" height="761" alt="dashboard png" src="https://github.com/user-attachments/assets/62881094-c0f2-4805-ad35-c731913624de" />


---

## 🎯 Project Objectives

- Analyze overall pizza sales performance
- Track total revenue, orders, quantity sold, and AOV
- Identify daily and hourly order trends
- Analyze sales performance by pizza category
- Analyze sales contribution by pizza size
- Identify top-performing pizzas by total orders
- Generate actionable business insights from sales data

---

## 🛠️ Tools & Technologies

- **Microsoft Excel**
  - Data Cleaning
  - Data Analysis
  - Pivot Tables
  - Charts & Dashboard
  - Slicers / Filters
- **SQL**
  - Data Aggregation
  - GROUP BY
  - ORDER BY
  - CASE Statements
  - Date & Time Analysis
  - Percentage Calculations
  - Ranking & Filtering

---

## 📌 Key Performance Indicators

| KPI | Value |
|---|---:|
| 💰 Total Revenue | ₹817,860.05 |
| 🧾 Total Orders | 21,350 |
| 🍕 Quantity Sold | 49,574 |
| 💵 Average Order Value | ₹38.31 |

---

## 📈 Dashboard Analysis

### 1. Daily Order Trend

The daily order analysis shows that:

- **Friday** recorded the highest number of orders with **3,538**
- **Thursday** followed with **3,239 orders**
- **Sunday** recorded the lowest orders with **2,624**
- Overall, order volume remains relatively consistent throughout the week.

### 2. Hourly Order Trend

The hourly analysis shows clear peak ordering periods:

- **12 PM** is the busiest hour with **2,529 orders**
- **1 PM** recorded **2,455 orders**
- Another strong period occurs around **5–6 PM**
- Orders decline significantly after **8 PM**
- **11 PM** has very low activity with only **28 orders**

**Business Insight:**  
The business should focus staffing, preparation, and promotions around lunch hours and the evening peak period.

---

## 🍕 Pizza Category Analysis

Sales contribution by pizza category:

| Category | Sales Contribution |
|---|---:|
| Classic | 26.91% |
| Supreme | 25.46% |
| Chicken | 23.96% |
| Veggie | 23.68% |

### Key Insight

- **Classic pizzas** contribute the highest share of sales at **26.91%**
- **Supreme pizzas** are the second-largest contributor at **25.46%**
- Chicken and Veggie categories have relatively similar contributions.
- The sales distribution is fairly balanced across all four categories.

---

## 📏 Pizza Size Analysis

| Pizza Size | Sales Contribution |
|---|---:|
| Large | 45.89% |
| Medium | 30.49% |
| Regular | 21.77% |
| X-Large | 1.72% |
| XX-Large | 0.12% |

### Key Insight

- **Large pizzas dominate sales**, contributing **45.89%**
- Medium pizzas account for **30.49%**
- Large + Medium pizzas together contribute more than **76%** of total sales.
- X-Large and XX-Large pizzas have very low demand.

**Business Insight:**  
Inventory planning and promotional offers should primarily focus on Large and Medium pizzas.

---

## 🏆 Top 5 Pizzas by Total Orders

| Rank | Pizza | Orders |
|---|---|---:|
| 🥇 1 | The Classic Deluxe Pizza | 2,453 |
| 🥈 2 | The Barbecue Chicken Pizza | 2,432 |
| 🥉 3 | The Hawaiian Pizza | 2,422 |
| 4 | The Pepperoni Pizza | 2,418 |
| 5 | The Thai Chicken Pizza | 2,371 |

### Key Insight

**The Classic Deluxe Pizza** is the best-performing pizza with **2,453 orders**, closely followed by Barbecue Chicken and Hawaiian pizzas.

The top 5 pizzas have relatively close order volumes, indicating strong demand across multiple popular products rather than dependence on a single pizza.

---

## 📦 Pizza Quantity by Category

| Category | Quantity Sold |
|---|---:|
| Classic | 14,888 |
| Supreme | 11,987 |
| Veggie | 11,649 |
| Chicken | 11,050 |

### Key Insight

Classic pizzas have the highest quantity sold with **14,888 pizzas**, making them the strongest category in terms of volume.

---

## 💡 Business Insights

Based on the analysis, the following insights were identified:

1. 🍕 **Classic pizzas are the strongest category**, contributing **26.91%** of total sales.
2. 📏 **Large pizzas are the most preferred size**, accounting for **45.89%** of sales.
3. 🕛 **Lunch hours are the busiest**, with **12 PM recording the highest orders**.
4. 🌆 Evening hours also show strong demand, especially around **5–6 PM**.
5. 📅 **Friday is the busiest day** with **3,538 orders**.
6. 🌙 Orders drop significantly during late-night hours.
7. 🏆 **The Classic Deluxe Pizza** is the top-selling pizza by total orders.
8. 📊 Sales are relatively well distributed across Classic, Supreme, Chicken, and Veggie categories.
9. 📦 Large and Medium pizzas together account for more than **76% of sales**, making them the key sizes for inventory planning.
10. 💰 The dashboard records total revenue of **₹817K+** from **21K+ orders**.

---

## 🔍 SQL Analysis

SQL was used to perform data analysis and extract meaningful insights, including:

- Total Revenue
- Total Orders
- Total Quantity Sold
- Average Order Value
- Daily Order Trends
- Hourly Order Trends
- Category-wise Sales
- Size-wise Sales
- Top 5 Pizzas
- Percentage Contribution
- Aggregated Sales Analysis

Example:

```sql
SELECT 
    pizza_category,
    SUM(quantity) AS total_pizza_sold
FROM pizza
GROUP BY pizza_category
ORDER BY total_pizza_sold DESC;
