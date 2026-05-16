# 🛒 Olist E-Commerce Data Analysis

![Python](https://img.shields.io/badge/Python-3.10-blue)
![SQL](https://img.shields.io/badge/SQL-SQLite-orange)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

> **Analyzing 100,000+ real orders from Olist — Brazil's largest e-commerce platform (2016–2018) — to uncover revenue trends, delivery bottlenecks, and customer behavior using Python and SQL.**

---

## 📌 Table of Contents
- [Project Overview](#project-overview)
- [Business Questions](#business-questions)
- [Dataset](#dataset)
- [Tools Used](#tools-used)
- [Project Structure](#project-structure)
- [Key Findings](#key-findings)
- [Business Recommendations](#business-recommendations)
- [Charts](#charts)
- [How to Run](#how-to-run)

---

## 📖 Project Overview

Olist is Brazil's largest department store marketplace connecting small businesses to customers. This project performs a full end-to-end data analysis on their publicly available dataset covering **2 years of real transactions (2016–2018).**

The analysis covers:
- Revenue trends and growth story
- Product category performance
- Delivery performance across Brazilian states
- Impact of late deliveries on customer reviews
- RFM Customer Segmentation

---

## ❓ Business Questions

| # | Question |
|---|---|
| 1 | What is Olist's total revenue and monthly growth trend? |
| 2 | Which product categories drive the most revenue? |
| 3 | How does delivery performance vary across Brazilian states? |
| 4 | Does late delivery directly impact customer review scores? |
| 5 | Who are the most valuable customers? (RFM Analysis) |

---

## 📦 Dataset

**Brazilian E-Commerce Public Dataset by Olist**
- 100,000+ orders across 9 relational tables
- Date range: September 2016 – October 2018
- Contains orders, customers, payments, products, sellers, reviews and geolocation data

🔗 [Download Dataset from Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Python | Data cleaning and analysis |
| Pandas | Data manipulation |
| Matplotlib & Seaborn | Data visualization |
| SQL (SQLite) | Business queries |
| Jupyter Notebook | Development environment |

---

## 📁 Project Structure

    olist-ecommerce-analysis/
    ├── notebooks/
    │   └── 01_data_exploration.ipynb
    ├── visuals/
    │   ├── monthly_revenue.png
    │   ├── top_categories.png
    │   ├── delivery_time_by_state.png
    │   ├── delivery_vs_reviews.png
    │   ├── orders_by_state.png
    │   ├── customer_segments.png
    │   ├── segment_value.png
    │   └── review_distribution.png
    ├── README.md
    ├── .gitignore
    └── LICENSE

## 📊 Key Findings

### 💰 Revenue
- Total revenue: **$15.4M** over 2 years
- **10x growth** from January to November 2017
- Black Friday 2017 was the biggest month at **$1.15M**
- Revenue stabilized at **~$1M/month** in 2018

### 🛍️ Product Categories
- **Bed & Bath** is the #1 category at **$1.69M**
- **Computers & Accessories** has fewer orders but highest value per order
- **Sports & Leisure** has high order volume but low revenue per order

### 🚚 Delivery Performance
- São Paulo delivers in just **8.8 days** (fastest)
- Northern states like Roraima wait **29+ days** (3x slower)
- **8% of orders** are delivered late
- Late deliveries average **2.57 stars** vs **4.29 stars** for on-time

### 👥 Customer Segments (RFM Analysis)
| Segment | Customers | Avg Spend |
|---|---|---|
| Champions | 6,493 | $312 |
| Loyal Customers | 27,292 | $134 |
| At Risk | 22,229 | $167 |
| Can't Lose Them | 8,671 | $241 |
| New Customers | 14,984 | $163 |
| Lost | 6,315 | $56 |

### ⭐ Customer Satisfaction
- **79%** of customers gave 4-5 stars
- **10%** gave 1 star — main driver is late delivery

---

## 💡 Business Recommendations

1. **Fix Northern State Logistics** — Open fulfillment centers in AM, PA, RR to reduce delivery time from 29 days to under 15 days
2. **Win Back Can't Lose Them Segment** — 8,671 high value customers inactive for 1+ year. A targeted campaign could recover **~$2M in revenue**
3. **Convert New Customers** — 14,984 customers bought once recently. A follow up offer within 30 days could convert them to loyal customers
4. **Reward Champions** — Create a VIP loyalty program for 6,493 top customers with early access and free shipping
5. **Reduce Late Deliveries** — Bring late delivery rate down from 8% to under 3% to significantly improve review scores

---

## 📈 Charts

### Monthly Revenue Trend
![Monthly Revenue](visuals/monthly_revenue.png)

### Top 10 Product Categories
![Top Categories](visuals/top_categories.png)

### Delivery Time by State
![Delivery Time](visuals/delivery_time_by_state.png)

### Late Delivery vs Review Score
![Delivery vs Reviews](visuals/delivery_vs_reviews.png)

### Customer Segments
![Customer Segments](visuals/customer_segments.png)

### Average Spend per Segment
![Segment Value](visuals/segment_value.png)

---

## ▶️ How to Run

1. Clone this repository:
```bash
git clone https://github.com/PayalSingh07/olist-ecommerce-analysis.git
```

2. Install required libraries:
```bash
pip install pandas matplotlib seaborn jupyter
```

3. Download the dataset from Kaggle and place CSV files in a `data/` folder

4. Open Jupyter Notebook:
```bash
jupyter notebook
```

5. Run `notebooks/01_data_exploration.ipynb` from top to bottom

---

## 👤 Author
**Payal Singh**
- 🔗 [LinkedIn](https://www.linkedin.com/in/payal-s-368aa0276/)
- 🐙 [GitHub](https://github.com/PayalSingh07/olist-ecommerce-analysis)

---

⭐ If you found this project helpful, please give it a star!
