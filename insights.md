This report summarizes insights from a comprehensive EDA on the Olist Brazilian E-Commerce dataset. It highlights customer behavior, product performance, revenue trends, and operational patterns, along with data quality considerations.

# Dataset: 
Olist Brazilian E-Commerce

# Objective: 
The goal of this exploratory data analysis (EDA) is to understand pricing behavior, customer reviews, payment preferences, product characteristics, and time-based trends in the Olist Brazilian e-commerce dataset.

# Key Findings & Summary (Report)

### 1. Price & Freight Value Analysis
- Order Price Distribution:
Order prices are heavily right-skewed, with most orders concentrated at the lower price range and a small number of very high-value orders acting as outliers.
- Price Boxplot:
The majority of order prices lie within a relatively narrow range, while a large number of extreme outliers indicate occasional high-priced purchases.
- Freight Value Distribution:
Freight charges are generally low for most orders, with a small set of orders incurring significantly higher shipping costs.

*This suggests that shipping is usually affordable but can increase substantially for certain products or locations.*

### 2. Review Score Analysis
- Review Score Distribution:
The dataset is dominated by 5-star reviews, followed by 4-star reviews. Lower ratings (1–3 stars) appear less frequently but are still present in meaningful numbers.

- Delivery Delay vs Review Score:
Orders with higher delivery delays tend to receive lower review scores, particularly 1-star reviews. This highlights delivery performance as a key driver of customer satisfaction.

### 3. Payment Type Insights
- Payment Method Usage:
	- Credit card is the most commonly used payment method.
	- Boleto is the second most popular option.
	- Voucher and debit card payments are relatively rare.
- Price Distribution by Payment Type:
Voucher and debit card payments show more variability and outliers, while credit card payments dominate across most price ranges.

### 4. Product Category Insights
- Top Product Categories:
Categories such as cama_mesa_banho, esporte_lazer, moveis_decoracao, beleza_saude, and informatica_acessorios appear most frequently and generate significant revenue.
- Revenue Concentration:
A small number of product categories contribute a disproportionately large share of total revenue, indicating category-level concentration.


### 5. Price vs Review Score
- The relationship between price and review score shows high variance.
- Due to missing review data for some orders, conclusions are limited.
- There is no strong evidence that higher-priced products consistently receive higher ratings.

### 6. Correlation Analysis (Numerical Features)
- Strong Positive Correlations:
	Product weight ↔ product price
	Product weight ↔ product height
	Product width ↔ product length

- Weak Negative Correlations:
	Delivery delay days show very weak or negative correlation with price and product dimensions.
	Larger or heavier products are not necessarily delivered more slowly.


### 7. Time-Based Trends
- Order Volume Over Time:
- The number of orders increases gradually over time, with clear seasonal spikes, especially during holiday periods.
- A sharp decline is observed near October 2018, corresponding to the end of the dataset.

- Revenue Trends:
- Peaks during holiday seasons
- Drops in early months
- Recovers mid-year before declining toward the dataset’s end

*This indicates strong seasonality in customer purchasing behavior.*

### 8. Customer & Geographic Analysis
- Customer Behavior:
All customers in the dataset are one-time buyers, with no repeat purchases observed during the available time period.

- Top States by Order Volume:
	- São Paulo (SP) has the highest number of orders
	- Followed by Rio de Janeiro (RJ) and Minas Gerais (MG)

*Order volume is highly concentrated in a few major states.*

# Key Takeaways
- Prices and freight values are highly skewed with significant outliers.
- Delivery delays have a clear negative impact on customer reviews.
- Credit cards dominate payment behavior.
- Revenue is concentrated in a small number of product categories.
- Strong seasonal patterns affect both orders and revenue.
- No repeat customer behavior is observed in this dataset.
