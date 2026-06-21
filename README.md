#  iPhone Sales Analysis — Exploratory Data Analysis

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-EDA-green?logo=pandas)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

A data analysis project exploring iPhone product listings, pricing, ratings, and discount patterns using Python.

---

##  Project Overview

This project analyzes an iPhone product dataset scraped from an e-commerce platform (Flipkart) to answer key business questions around pricing, customer ratings, and discount strategies.

**Domain:** E-commerce / Consumer Electronics  
**Type:** Exploratory Data Analysis (EDA)  
**Tools:** Python, Pandas, Matplotlib, Seaborn

---

##  Key Questions Answered

1. Which iPhone models have the highest customer ratings?
2. Which models have received the most customer reviews?
3. Is there a relationship between Sale Price and Number of Ratings?
4. Does a higher Discount Percentage lead to more customer ratings?
5. What are the specifications of the cheapest and most expensive iPhones?

---

##  Key Findings

| Finding | Result |
|---|---|
| Highest rated iPhone | iPhone 11 Pro Max — 4.7 ⭐ (1,078 ratings) |
| Price vs Ratings correlation | **-0.70** — Lower priced iPhones get more ratings |
| Discount vs Ratings correlation | Positive — Higher discounts attract more buyers |
| Most reviewed model | iPhone 11 series dominates review count |

###  Insights

- **Lower-priced iPhones are rated more often** — this reflects India's price-sensitive market where budget models see higher sales volumes and therefore more reviews.
- **A -0.70 correlation** between Sale Price and Number of Ratings is a strong negative relationship — the most affordable models get the most customer engagement.
- **Discount percentage positively correlates** with rating count, suggesting promotional pricing drives purchase volume.

---

##  Project Structure

```
iphone-sales-analysis/
│
├── iPhone_Sales_Analysis.ipynb   ← Main analysis notebook
├── apple_products.csv            ← Dataset (source: Kaggle)
├── requirements.txt              ← Python dependencies
└── README.md                     ← Project documentation
```

---

##  Dataset

- **Source:** [Apple Products Data — Kaggle](https://www.kaggle.com/datasets/komalkhetlani/apple-products-data)
- **Records:** iPhone product listings from Flipkart
- **Key Columns:**

| Column | Description |
|---|---|
| Product Name | iPhone model name |
| Sale Price | Current selling price  |
| MRP | Original price before discount  |
| Discount Percentage | % discount offered |
| Star Rating | Average customer star rating |
| Number Of Ratings | Total ratings count |
| Number Of Reviews | Total written reviews |
| RAM | RAM specification |
| ROM | Storage specification (extracted) |
| Color | Color variant (extracted) |

---

##  Steps Performed

### 1. Data Cleaning
- Dropped irrelevant columns (`Product URL`, `Brand`, `UPC`)
- Extracted `Color` and `ROM` from the Product Name column using **Regex**
- Standardized product name formatting

### 2. Exploratory Analysis
- Checked for duplicates and missing values
- Generated descriptive statistics

### 3. Visualizations
- **Top 10 Highest-Rated iPhone Models** — Horizontal bar chart
- **Top 10 Most Reviewed iPhone Models** — Bar chart with value labels

### 4. Correlation Analysis
- **Sale Price vs Number of Ratings** — Linear regression plot (r = -0.70)
- **Discount Percentage vs Number of Ratings** — Linear regression plot

### 5. Price Extremes
- Identified cheapest and most expensive iPhones with full specifications

---

##  How to Run

```bash
# 1. Clone the repository
git clone https://github.com/faiz2517/iphone-sales-analysis.git
cd iphone-sales-analysis

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter Notebook
jupyter notebook iPhone_Sales_Analysis.ipynb
```

---

## Requirements

See `requirements.txt` for full list. Main libraries:
- `pandas` — data manipulation
- `numpy` — numerical operations
- `matplotlib` — plotting
- `seaborn` — statistical visualization

---

##  Author

**Md Faiz Ansari**  
Aspiring Data Analyst & Data Scientist  

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/md-faiz-ansari-00a3a8275/)
[![GitHub](https://img.shields.io/badge/GitHub-faiz2517-black?logo=github)](https://github.com/faiz2517)
[![mail](faizaaykhan8916@gmail.com)]
