# FoodHub Order Analysis

Exploratory data analysis of ~1,900 food-delivery orders placed through **FoodHub**,
a food-aggregator app operating in New York City. The analysis explores customer
demand, cuisine popularity, order cost, food-preparation and delivery times, and
customer ratings, and estimates the revenue the aggregator earns across all orders.

## Overview

The dataset contains one row per order with nine fields: order ID, customer ID,
restaurant name, cuisine type, order cost, day of the week, rating, food-preparation
time, and delivery time.

The notebook works through:

- **Data cleaning** — data types, missing values, and unrated orders
- **Univariate analysis** — distributions of cost, prep time, delivery time, cuisine, and ratings
- **Multivariate analysis** — relationships between cuisine, cost, timing, and ratings
- **Business metrics** — top restaurants, most popular weekend cuisines, promotional-offer
  eligibility, and net revenue
- **Conclusions & recommendations**

## Key findings

- American cuisine is the most ordered; **Shake Shack** is the single most-ordered restaurant.
- Orders spike on weekends, and weekend deliveries are *faster* than weekday deliveries
  (~22.5 min vs ~28.3 min).
- Most orders are under $20, and ~90% are delivered within 60 minutes of being placed.
- Ratings show little correlation with cost, prep time, or delivery time.

## Tech stack

Python · pandas · NumPy · matplotlib · seaborn · Jupyter

## Getting started

```bash
pip install -r requirements.txt
jupyter notebook FDS_Project.ipynb
```

## Dataset

The dataset is **not included** in this repository. To try it yourself, download the
**FoodHub order data** from [Kaggle](https://www.kaggle.com/datasets/andrewtoh78/foodhub-order)
and place it at `data/foodhub_order.csv`.

## Repository layout

```
├── FDS_Project.ipynb      # main analysis notebook
├── data/
│   └── foodhub_order.csv  # order-level dataset (not tracked in git)
├── requirements.txt
└── README.md
```
