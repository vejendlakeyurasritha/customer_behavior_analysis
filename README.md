
# Customer Shopping Behavior Analysis

An end-to-end data analytics project focused on understanding customer shopping patterns, purchasing behavior, product performance, discount usage, subscription trends, and revenue using **Python, MySQL, and Power BI**.

The project analyzes **3,900 purchase records across 18 columns** to uncover business insights and support data-driven decision-making.

---

## 📌 Project Overview

Understanding customer purchasing behavior helps businesses evaluate product performance, customer preferences, and revenue trends. This project uses data cleaning, SQL-based analysis, and business intelligence reporting to explore customer shopping behavior.

### 🎯 Objectives

- Clean and prepare customer shopping data for analysis.
- Analyze revenue across customer demographics and age groups.
- Evaluate subscription status and purchasing patterns.
- Identify products with high average ratings and discount usage.
- Examine customer segments and repeat-purchase behavior.
- Compare average purchase amounts across shipping types.
- Present key findings through a Power BI dashboard.
- Provide actionable business recommendations.

## 🛠️ Tools and Technologies

| Tool | Purpose |
|---|---|
| **Python** | Data cleaning, preprocessing, feature creation, and missing-value handling using pandas |
| **MySQL** | SQL queries and analysis of customer behavior, revenue, products, discounts, and subscriptions |
| **Power BI** | Dashboard reporting and data visualization |

## 📂 Dataset Overview

The dataset contains **3,900 purchase records and 18 columns** covering customer demographics, purchase details, and shopping behavior.

### Key Features

- **Customer Information:** Age, Gender, Location, Subscription Status
- **Purchase Details:** Item Purchased, Category, Purchase Amount (USD), Season, Size, Color
- **Shopping Behavior:** Discount Applied, Previous Purchases, Purchase Frequency
- **Customer Feedback:** Review Rating
- **Shipping Information:** Shipping Type

### Data Preparation

1. Imported the dataset using pandas.
2. Standardized column names to `snake_case`.
3. Created an `age_group` column.
4. Created a `purchase_frequency_days` column.
5. Imputed **37 missing review ratings** using the median rating within each category.
6. Dropped the `Promo Code Used` column.
7. Connected the prepared dataset to MySQL for SQL analysis.

## 🔍 Analysis Performed

### 1. Revenue Analysis
- Compared revenue by gender.
- Analyzed revenue across different age groups.
- Examined average purchase amounts and overall revenue metrics.

### 2. Subscription Analysis
- Compared subscribers and non-subscribers by customer count, average spending, and total revenue.

### 3. Discount Analysis
- Identified high-spending records involving discounts.
- Ranked products based on discount usage.
- Examined discount patterns to identify opportunities for reviewing discount policies.

### 4. Product Performance
- Identified the top five products by average review rating.
- Compared product counts across categories.
- Examined repeat-purchase patterns.

### 5. Shipping Analysis
- Compared average purchase amounts for standard and express shipping.

### 6. Customer Segmentation
- Analyzed **Loyal, Returning, and New** customer segments.

## 📊 Key Findings

All monetary values are reported in USD, as documented in the project report.

### Overall Metrics

| Metric | Value |
|---|---:|
| Total purchase records | 3,900 |
| Average purchase amount | $59.76 |
| Average review rating | 3.75 |
| Subscription status — Yes | 27% |
| Subscription status — No | 73% |

### Revenue by Gender

| Gender | Revenue |
|---|---:|
| Female | $75,191 |
| Male | $157,890 |

### Subscribers vs. Non-Subscribers

| Metric | Subscribers | Non-Subscribers |
|---|---:|---:|
| Customers | 1,053 | 2,847 |
| Average spend | $59.49 | $59.87 |
| Total revenue | $62,645.00 | $170,436.00 |

### Top 5 Products by Average Rating

| Product | Average Rating |
|---|---:|
| Gloves | 3.86 |
| Sandals | 3.84 |
| Boots | 3.82 |
| Hat | 3.80 |
| Skirt | 3.78 |

### Average Purchase Amount by Shipping Type

| Shipping Type | Average Purchase Amount |
|---|---:|
| Standard Shipping | $58.46 |
| Express Shipping | $60.48 |

### Products with the Highest Discount Usage

| Product | Purchases Using Discounts |
|---|---:|
| Hat | 50.00% |
| Sneakers | 49.66% |
| Coat | 49.07% |
| Sweater | 48.17% |
| Pants | 47.37% |

### Customer Segmentation

| Segment | Customers |
|---|---:|
| Loyal | 3,116 |
| Returning | 701 |
| New | 83 |

### Revenue by Age Group

| Age Group | Revenue |
|---|---:|
| Young Adult | $62,143 |
| Middle-aged | $59,197 |
| Adult | $55,978 |
| Senior | $55,763 |

### Repeat Purchase Analysis

- **958 customers** had more than five purchases.
- **2,518 customers** did not have more than five purchases.

## 📈 Power BI Dashboard

![Customer Shopping Behavior Dashboard](dashboard.png)

The Power BI report presents key metrics and analytical findings, including:

- Revenue by age group
- Revenue by category
- Total customer count
- Average purchase amount
- Average review rating
- Subscription status

**Dashboard File:** `customer_analysis.pbix`

## 💡 Business Recommendations

1. **Encourage subscriptions:** Promote exclusive subscription benefits to encourage customer sign-ups.
2. **Reward repeat customers:** Use loyalty initiatives to recognize repeat purchasing behavior.
3. **Review discount policies:** Evaluate discount usage while balancing sales objectives and profit margins.
4. **Promote highly rated products:** Use product ratings and purchase counts to guide marketing campaigns.
5. **Target relevant customer groups:** Consider higher-revenue age groups and express-shipping customers when planning campaigns.

*These are recommendations for consideration; their business impact has not been measured in this analysis.*

## ⚠️ Limitations

- The analysis is based on the provided transactional dataset.
- No additional inferred or estimated data is included beyond the reported SQL results.
- Monetary values are retained in USD.
- Missing review ratings were imputed using the median rating within each category, which may influence rating summaries.


## 📁 Project Structure

- `Customer_shopping_analysis.ipynb` — Python notebook for data cleaning, preprocessing, feature engineering, and analysis.
- `customer_analysis_sql.sql` — MySQL queries for business analysis.
- `customer_analysis.pbix` — Power BI dashboard.
- `customer_shopping_behavior.csv` — Source dataset.
- `Customer Shopping Behavior.pdf` — Project report.
- `README.md` — Project documentation.

## 🚀 How to View the Dashboard

1. Clone or download this repository.
2. Open `customer_analysis.pbix` using Microsoft Power BI Desktop.
3. Explore the report visuals and business metrics.

To reproduce the complete analysis, the corresponding Python code, source dataset, and MySQL queries must also be available.

## 🧠 Skills Demonstrated

- Data cleaning and preprocessing using Python
- Exploratory data analysis
- Feature creation and missing-value handling with pandas
- SQL querying and business analysis using MySQL
- Customer segmentation and purchasing behavior analysis
- Revenue and product performance analysis
- Power BI dashboard development and data visualization
- Translating analytical findings into business recommendations

---

**Project:** Customer Shopping Behavior Analysis  
**Technologies:** Python | MySQL | Power BI  
**Dataset:** 3,900 purchase records | 18 columns
