# 🛒 E-Commerce Behaviour & Revenue Analysis

> A deep-dive exploratory data analysis of a multi-table e-commerce dataset — uncovering conversion bottlenecks, customer segments, product performance, and city-level opportunities.

🌐 **[View Project Website →]https://vyomvy.github.io/ecommerce-user-conversion-analysis/**

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Analysis Sections](#analysis-sections)
- [Visualisations](#visualisations)
- [Tech Stack](#tech-stack)
- [How to Run](#how-to-run)

---

## Project Overview

This project analyses an e-commerce platform's transactional and behavioural data to answer questions like:

- Where are users dropping off in the purchase funnel?
- Which cities and customers drive the most revenue?
- What products have high traffic but low conversions?
- How long does it take users to go from signup to first order?

The analysis spans **8,594 users**, **19,611 orders**, **2,000 products** across **10 categories** and **12 brands**.

---

## Dataset

Six CSV files were loaded and merged into a master DataFrame:

| File | Description |
|---|---|
| `users.csv` | User demographics, signup date, city |
| `orders.csv` | Order IDs, dates, status, total amount |
| `order_items.csv` | Line items per order |
| `products.csv` | Product names, categories, brands |
| `reviews.csv` | Ratings and review dates |
| `events.csv` | Behavioural events (view, cart, purchase) |

> `events` was kept separate from the main merge to avoid row explosion from the many-to-many relationship.

---

## Analysis Sections

1. **Revenue Analysis** — Total revenue, monthly trends, AOV
2. **Customer Segmentation** — Top customers, repeat buyers, top 10% revenue share
3. **Conversion Funnel** — View → Cart → Purchase drop-off analysis
4. **Signup to First Order** — Time-to-convert distribution and user journey split
5. **Product Performance** — High-value low-rating products, repeat purchases
6. **High Views, Low Conversion** — Products with traffic but no sales
7. **City-Level Insights** — High revenue / low user cities; high user / low engagement cities

---

## Visualisations

All charts are saved in the `images/` folder:

| File | Description |
|---|---|
| `images/conversion funnel.png` | Overall View → Cart → Purchase funnel |
| `images/high user low engagement.png` | Cities with large user base but low activity |
| `images/high value low rating.png` | High-revenue, low-rated categories |
| `images/signup to first order.png` | Days-to-first-order histogram |

---

## Tech Stack

- **Python 3** (Google Colab)
- `pandas` — data wrangling and merging
- `matplotlib` — all visualisations
- **Data source**: Synthetic e-commerce dataset (CSV files)

---

## How to Run

1. Clone this repository
2. Upload the dataset CSVs to your Google Drive under `MyDrive/ecommerce_dataset/`
3. Open `ecommerce_analysis.ipynb` in Google Colab
4. Run all cells in order

```bash
git clone https://github.com/vyomvy/ecommerce-user-conversion-analysis

---

*Analysis period: Jan 2024 – Oct 2025 (Nov 2025 excluded due to partial data)*
