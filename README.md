# 🍽️ Zomato Restaurant Data Analysis

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.5.0-red.svg)](https://pandas.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> 📊 A comprehensive Exploratory Data Analysis (EDA) project on the Zomato restaurant dataset to uncover insights about restaurant ratings, pricing trends, cuisine preferences, and customer behavior across Indian cities.

---

# 📌 Table of Contents

- [📖 Overview](#-overview)
- [📁 Dataset](#-dataset)
- [🛠️ Tools & Libraries](#️-tools--libraries)
- [🧹 Data Preprocessing](#-data-preprocessing)
- [📈 Key Visualizations](#-key-visualizations)
- [💡 Insights & Findings](#-insights--findings)
- [🎯 Business Recommendations](#-business-recommendations)
- [📂 Project Structure](#-project-structure)
- [▶️ How to Run](#️-how-to-run)
- [🚀 Future Scope](#-future-scope)
- [👨‍💻 Author](#-author)
- [📜 License](#-license)

---

# 📖 Overview

This project performs an **Exploratory Data Analysis (EDA)** on a large-scale Zomato restaurant dataset containing **117,000+ restaurants** across multiple Indian cities.

The main objective of this project is to analyze restaurant trends and discover meaningful insights related to:

- 🏙️ City & locality distribution
- 🍛 Popular cuisine types
- 💰 Restaurant pricing trends
- ⭐ Customer ratings & reviews
- 🚚 Delivery performance
- 🎟️ Discounts & monthly orders
- 📦 Order preferences (Dine-In / Delivery / Takeaway)

The analysis helps restaurant owners, food delivery platforms, and customers make better data-driven decisions.

---

# 📁 Dataset

- **Dataset Name:** Zomato Restaurant Dataset
- **Total Rows:** 117,000+
- **Total Columns:** 16
- **File Format:** CSV

## 📋 Features Description

| Feature Name | Type | Description |
|---|---|---|
| `restaurant_id` | Numerical | Unique restaurant identifier |
| `restaurant_name` | Categorical | Restaurant name |
| `cuisine_type` | Categorical | Type of cuisine served |
| `city` | Categorical | City location |
| `locality` | Categorical | Area/locality within city |
| `average_cost_for_two` | Numerical | Average cost for two people |
| `rating` | Numerical | Restaurant rating (out of 5) |
| `votes` | Numerical | Number of customer votes |
| `delivery_time_min` | Numerical | Average delivery time |
| `discount_percent` | Numerical | Discount percentage |
| `menu_items_count` | Numerical | Total menu items |
| `monthly_orders` | Numerical | Average monthly orders |
| `review_count` | Numerical | Number of written reviews |
| `distance_km` | Numerical | Delivery distance |
| `establishment_year` | Numerical | Restaurant establishment year |
| `order_type` | Categorical | Dine-In / Delivery / Takeaway |

---

# 🛠️ Tools & Libraries

| Tool / Library | Purpose |
|---|---|
| 🐍 Python | Programming language |
| 🐼 Pandas | Data analysis & manipulation |
| 🔢 NumPy | Numerical computations |
| 📊 Matplotlib | Data visualization |
| 🎨 Seaborn | Statistical visualization |
| 📓 Jupyter Notebook | Interactive analysis environment |
| 🤖 Scikit-learn | Data preprocessing & modeling |

---

# 🧹 Data Preprocessing

The following preprocessing steps were performed:

1. ✅ Handling missing values
2. ✅ Removing duplicate records
3. ✅ Correcting data types
4. ✅ Outlier detection & treatment
5. ✅ Feature scaling (optional)
6. ✅ Encoding categorical variables
7. ✅ Data cleaning and formatting

---

# 📈 Key Visualizations

| Visualization | Purpose |
|---|---|
| 📊 Bar Charts | Compare ratings and cuisines |
| 📉 Histograms | Analyze distributions |
| 🥧 Pie Charts | Order type distribution |
| 📈 Line Charts | Monthly order trends |
| 🔥 Heatmaps | Correlation analysis |
| 📦 Box Plots | Detect outliers |

---

# 💡 Insights & Findings

## 🍛 Cuisine Analysis

- North Indian and Chinese cuisines are the most popular.
- Mediterranean and Seafood restaurants tend to receive higher ratings.

## 💰 Pricing Trends

- Metro cities like Mumbai, Delhi, and Bangalore have higher average dining costs.
- Smaller cities maintain more affordable pricing.

## ⭐ Ratings & Delivery Time

- Restaurants with faster delivery usually receive better ratings.
- Delivery times above 75 minutes negatively impact customer satisfaction.

## 🎟️ Discounts & Orders

- Discounts between 20–30% increase customer orders significantly.
- Extremely high discounts do not guarantee better engagement.

## 🍽️ Order Preferences

- Dine-In restaurants generally receive slightly higher ratings.
- Better service quality and ambiance influence ratings positively.

---

# 🎯 Business Recommendations

| Recommendation | Reason |
|---|---|
| 🍽️ Open restaurants in high-demand localities | Better visibility and customer reach |
| 🍛 Focus on popular cuisines | Higher customer engagement |
| 💰 Maintain balanced pricing | Improves customer retention |
| 🎟️ Offer moderate discounts | Increases order volume |
| 🚚 Reduce delivery time | Enhances customer experience |
| ⭐ Improve dine-in experience | Boosts restaurant ratings |

---

# 📂 Project Structure

```txt
zomato-data-analysis/
│
├── data/
│   └── zomato.csv                  # Raw dataset
│
├── notebooks/
│   └── zomato_analysis.ipynb       # Jupyter notebook with analysis
│
├── images/
│   └── charts/                     # Saved visualizations
│
├── requirements.txt                # Project dependencies
│
├── README.md                       # Project documentation
│
└── LICENSE                         # MIT license
```

---

# ▶️ How to Run

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/ProgrammingWithNick/Food-Delivery.git
```

## 2️⃣ Navigate to the Project Folder

```bash
cd Food-Delivery
```

## 3️⃣ Install Required Libraries

```bash
pip install -r requirements.txt
```

## 4️⃣ Open Jupyter Notebook

```bash
jupyter notebook
```

## 5️⃣ Run the Notebook

Open:

```bash
notebooks/zomato_analysis.ipynb
```

Run all cells to view the complete analysis and visualizations.

---

# 🚀 Future Scope

- 🤖 Machine Learning-based restaurant rating prediction
- 📍 Location-wise recommendation system
- 📈 Interactive dashboards using Power BI or Tableau
- 🌐 Web deployment using Streamlit
- 📊 Real-time restaurant analytics

---

# 👨‍💻 Author

**Nikhil Khavdu**

- 🎓 MCA Student
- 💻 Full Stack Developer
- 🚀 Passionate about Data Analytics, AI, and Web Development

---

# 📜 License

This project is licensed under the **MIT License**.

Feel free to use, modify, and share this project for learning and educational purposes.
