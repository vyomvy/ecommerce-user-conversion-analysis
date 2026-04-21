# 🛒 E-Commerce Behavioral & Revenue Analysis

> A full-stack exploratory data analysis project uncovering conversion bottlenecks, customer segments, and growth opportunities in a synthetic Indian e-commerce dataset.

🌐 **[View Project Website →](https://your-website-link-here.com)**

---

## 📌 Overview

This project analyzes a multi-table e-commerce dataset — users, orders, products, reviews, and behavioral events — to answer one core question: **where is the business losing money, and where is it leaving it on the table?**

The analysis spans 8,594 users, 19,611 orders, 2,000 products across 10 categories and 12 brands — spanning data from early 2024 through October 2025.

---

## 📊 Key Findings at a Glance

| Metric | Value |
|---|---|
| Total Revenue (Completed + Shipped) | ₹47,23,771 |
| Average Order Value | ₹592.55 |
| Signup-to-Purchase Conversion Rate | 80.3% |
| Repeat Purchase Rate | 67.5% |
| Top 10% Customers → Revenue Share | 33.5% |
| Funnel: View → Purchase Drop-off | 92.8% |

---

## 🔍 Analysis Sections

### 1. Revenue & Order Overview
- Total revenue from completed and shipped orders: **₹47,23,771**
- ~40% of orders are cancelled or returned — a significant fulfillment/quality signal
- Monthly revenue is flat with no clear growth trend; festive months underperform

### 2. Customer Conversion Funnel
- 80.3% of registered users have placed at least one order — an exceptionally strong top-of-funnel
- Product page is the biggest drop-off point: **78.5% of viewers never add to cart**
- Only 7.2% of product views result in a purchase

  ![Conversion Funnel](conversion%20funnel.png)

### 3. Signup to First Order
- 63% of users placed their first order *before* account creation (guest-first flow)
- Of post-signup users, the average days-to-first-order is **~62 days**, but median is near 0 — long tail of late adopters skews it

  ![Signup to First Order](signup%20to%20first%20order.png)

### 4. High-Value, Low-Rating Products
- Electronics leads with **₹8,37,279** in high-value, low-rated revenue (avg rating 2.76/5)
- 9 out of 10 categories appear in this quadrant — a platform-wide quality issue, not isolated

  ![High Value Low Rating](high%20value%20low%20rating.png)

### 5. Geographic Insights: High Users, Low Engagement
- Multiple cities have large registered user bases but below-average browsing activity
- Re-engagement campaigns targeting these cities could convert already-acquired users

  ![High User Low Engagement](high%20user%20low%20engagement.png)

### 6. Other Analyses
- **Top 25 customers** place 7–10 orders each — natural ceiling on power-user frequency
- **Top 10 products** contribute only 2.4% of revenue → classic long-tail distribution
- **1,542 cities** generate high revenue from very few users — untapped high-value markets
- Products like *Nimbus Threat* and *Harbor Eye* have 40+ views but 2–3% conversion — listing/pricing friction

---

## 🗂️ Dataset Structure

```
ecommerce_dataset/
├── users.csv          # User profiles with signup date, city
├── orders.csv         # Order-level data with status and total amount
├── order_items.csv    # Line-item breakdown per order
├── products.csv       # Product catalogue with category and brand
├── reviews.csv        # Ratings linked to order + product
└── events.csv         # Behavioral events: view, cart, purchase
```

---

## 🛠️ Tech Stack

- **Python 3** — core analysis
- **Pandas** — data wrangling and merging
- **Matplotlib** — visualizations
- **Google Colab** — execution environment
- **Jupyter Notebook** — `.ipynb` format

---

## 🚀 How to Run

1. Clone the repository
2. Upload the dataset folder to your Google Drive at `MyDrive/ecommerce_dataset/`
3. Open `ecommerce_analysis.ipynb` in Google Colab
4. Run all cells top to bottom

```bash
git clone https://github.com/your-username/ecommerce-analysis.git
```

---

## 💡 Business Recommendations

- **Fix the product page** — the view→cart drop (78.5%) is the single biggest revenue leak
- **Launch a loyalty programme** for the top 10% of customers (859 users, 33.5% of revenue)
- **Investigate Electronics quality** — high revenue + low ratings = return/churn risk
- **Re-engage dormant city users** — large user base, low browsing in several metros
- **Target high-revenue low-user cities** — single buyers spending ₹40K+ signal untapped demand

---

## 📁 Project Structure

```
├── ecommerce_analysis.ipynb   # Main analysis notebook
├── conversion funnel.png
├── high user low engagement.png
├── high value low rating.png
├── signup to first order.png
└── README.md
```

---

## 👤 Author

Made with 📊 and Python.  
Connect on [LinkedIn](https://www.linkedin.com/in/your-profile) · [Project Website](https://your-website-link-here.com)
