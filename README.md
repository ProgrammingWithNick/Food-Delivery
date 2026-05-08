# 🍽️ Zomato Restaurant Data Analysis

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.5.0-red.svg)](https://pandas.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> 📊 A comprehensive data analysis project on Zomato restaurant dataset to uncover insights about restaurant ratings, pricing trends, cuisine preferences, and customer behavior across Indian cities.

---

## 📌 Table of Contents
- [Overview](#-overview)
- [Dataset](#-dataset)
- [Tools & Libraries](#-tools--libraries)
- [Data Preprocessing](#-data-preprocessing)
- [Key Visualizations](#-key-visualizations)
- [Insights & Findings](#-insights--findings)
- [Business Recommendations](#-business-recommendations)
- [Project Structure](#-project-structure)
- [How to Run](#-how-to-run)
- [Future Scope](#-future-scope)
- [Author](#-author)

---

## 📖 Overview

This project performs an **exploratory data analysis (EDA)** on a large-scale Zomato restaurant dataset containing **117,000+ restaurants** across multiple Indian cities. The goal is to identify patterns and relationships between various features such as:

- 🏙️ City & Locality
- 🍛 Cuisine Type
- 💰 Average Cost for Two
- ⭐ Ratings & Votes
- 🚚 Delivery Time
- 🎟️ Discount Percent
- 📦 Order Type (Dine-In / Delivery / Takeaway)

The insights derived can help restaurant owners, food delivery platforms, and customers make data-driven decisions.

---

## 📁 Dataset

- **Source**: Zomato Restaurant Data (synthetic/real-world aggregated)
- **Rows**: 117,000+
- **Columns**: 16

### Feature Description

| Feature Name          | Type        | Description |
|----------------------|-------------|-------------|
| `restaurant_id`      | Numerical   | Unique identifier for each restaurant |
| `restaurant_name`    | Categorical | Name of the restaurant |
| `cuisine_type`       | Categorical | Type of cuisine served |
| `city`               | Categorical | City where restaurant is located |
| `locality`           | Categorical | Specific locality within city |
| `average_cost_for_two` | Numerical | Average cost for two people (₹) |
| `rating`             | Numerical | Average customer rating (out of 5) |
| `votes`              | Numerical | Number of user votes/ratings |
| `delivery_time_min`  | Numerical | Average delivery time in minutes |
| `discount_percent`   | Numerical | Discount percentage offered |
| `menu_items_count`   | Numerical | Number of items on menu |
| `monthly_orders`     | Numerical | Average monthly orders |
| `review_count`       | Numerical | Number of written reviews |
| `distance_km`        | Numerical | Delivery distance in km |
| `establishment_year` | Numerical | Year restaurant was established |
| `order_type`         | Categorical | Dine-In / Delivery / Takeaway |

---

## 🛠️ Tools & Libraries

| Library | Purpose |
|---------|---------|
| 🐍 **NumPy** | Numerical operations |
| 🐼 **Pandas** | Data manipulation & analysis |
| 📊 **Matplotlib** | Basic plotting & visualization |
| 🎨 **Seaborn** | Statistical data visualization |
| 🔧 **Scikit-learn** | Preprocessing & modeling (optional) |

---

## 🧹 Data Preprocessing

The following preprocessing steps were performed to ensure data quality:

1. ✅ **Handling Missing Values** – Dropped rows with critical nulls, imputed others with median/mode.
2. ✅ **Duplicate Removal** – Checked and removed duplicate restaurant entries.
3. ✅ **Data Type Conversion** – Ensured numerical columns were properly typed.
4. ✅ **Outlier Treatment** – Capped extreme values in `average_cost_for_two` and `delivery_time_min`.
5. ✅ **Feature Scaling** – Applied normalization for certain numerical features in modeling phase.
6. ✅ **Categorical Encoding** – Used one-hot encoding for categorical variables like `cuisine_type` and `city`.

---

## 📈 Key Visualizations

| Chart Type | Purpose |
|------------|---------|
| 📊 **Bar Chart** | Compare average ratings across cuisines and cities |
| 📉 **Histogram** | Distribution of ratings, cost, and delivery time |
| 🥧 **Pie Chart** | Proportion of order types (Dine-In vs Delivery vs Takeaway) |
| 📈 **Line Chart** | Trend of monthly orders over different discount brackets |
| 🔥 **Heatmap** | Correlation between numerical features |
| 📦 **Box Plot** | Detect outliers in cost and ratings by cuisine |

---

## 💡 Insights & Findings

### 🍛 Cuisine Analysis
- **North Indian**, **Chinese**, and **Street Food** are the most common cuisines.
- **Mediterranean** and **Seafood** restaurants tend to have **higher average ratings** (above 4.0).

### 💰 Pricing Trends
- Metropolitan cities like **Mumbai, Bangalore, Delhi** have significantly higher `average_cost_for_two` (₹1500–₹2000).
- Smaller cities average around ₹800–₹1200 for two people.

### ⭐ Ratings & Delivery Time
- Weak **negative correlation** between `delivery_time_min` and `rating`.
- Restaurants with delivery time >75 minutes often have **lower ratings**.

### 🎟️ Discount & Orders
- Discounts of **20–30%** positively impact `monthly_orders` and `votes`.
- Very high discounts (50%) on low-rated restaurants **do not** significantly boost orders.

### 🍽️ Order Type
- **Dine-In** restaurants have **slightly higher average ratings** compared to Delivery or Takeaway.
- Suggests that ambiance and service quality contribute to satisfaction.

### 🏙️ Top Localities
- **Koramangala (Bangalore)**, **Connaught Place (Delhi)**, and **HSR Layout (Bangalore)** have the highest concentration of top-rated restaurants.

---

## 🎯 Business Recommendations

| Recommendation | Rationale |
|----------------|-----------|
| 🍽️ Open in high-density localities like Koramangala or Connaught Place | Higher footfall and rating potential |
| 🍛 Offer popular cuisines (North Indian, Chinese) with regional specialties | Broader customer appeal |
| 💰 Price between ₹800–₹1500 for two | Optimal price range for good ratings |
| 🎟️ Offer introductory discounts of 20–30% | Boosts initial orders and votes |
| 🚚 Keep delivery time under 45 minutes | Maintains positive customer experience |
| 🍴 Focus on Dine-In quality initially | Builds strong rating foundation |

---

📂 Project Structure

zomato-data-analysis/
│
├── data/
│   └── zomato.csv              # Raw dataset
│
├── notebooks/
│   └── Untitled.ipynb          # Jupyter notebook with full analysis
