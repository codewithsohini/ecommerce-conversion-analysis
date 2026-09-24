# E-Commerce Conversion & Customer Behavior Analysis

## Overview

This project analyzes **25,000 e-commerce sessions** to understand customer behavior, purchase conversion, cart abandonment, pricing, discounts, product ratings, and marketing channels.

The project follows a business-focused, hypothesis-driven analytics approach rather than simply producing a dashboard. Each major question is investigated using data analysis, visualization, and business interpretation.

## Business Problem

E-commerce businesses can receive substantial website traffic without converting all visitors into customers. Customers may browse products, spend time on the website, add products to their cart, and still leave without completing a purchase.

This project investigates which customer, behavioral, product, pricing, and acquisition factors are associated with purchase conversion and cart abandonment.

## Objectives

- Measure overall purchase conversion.
- Quantify cart abandonment.
- Examine whether website engagement is associated with purchase.
- Investigate the relationship between product price and cart abandonment.
- Examine whether discount levels are associated with conversion.
- Analyze the relationship between product ratings and repeat-customer behavior.
- Compare conversion rates across marketing channels.
- Translate findings into practical business recommendations.

## Dataset

The dataset contains:

- **25,000 sessions**
- **29 variables**
- **8,442 unique customers**
- Date coverage: **January 1, 2024 to December 30, 2024**

Important variables include:

- `customer_id`
- `session_id`
- `visit_date`
- `device_type`
- `user_type`
- `marketing_channel`
- `product_id`
- `product_category`
- `unit_price`
- `quantity`
- `discount_percent`
- `discount_amount`
- `revenue`
- `pages_viewed`
- `time_on_site_sec`
- `added_to_cart`
- `purchased`
- `cart_abandoned`
- `rating`
- `payment_method`
- `location`

## Project Workflow

1. Data loading
2. Data quality checking
3. Data cleaning
4. Feature engineering
5. Exploratory data analysis
6. Hypothesis-driven analysis
7. Visualization
8. Statistical testing
9. Business recommendations
10. Conclusion

## Hypotheses

### H1 — Engagement → Purchase
Customers with higher website engagement may be more likely to purchase.

### H2 — Cart Abandonment
A substantial proportion of customers who add products to their cart may fail to complete the purchase.

### H3 — Price → Abandonment
Higher-priced products may be associated with higher cart abandonment.

### H4 — Discount → Conversion
Different discount levels may be associated with different purchase conversion rates.

### H5 — Rating → Repeat Purchase
Product rating may be associated with repeat-customer behavior.

### H6 — Marketing Channel → Conversion
Purchase conversion rates may differ across marketing channels.

## Key Findings

- **16,117** sessions added a product to the cart.
- Among cart additions, **65.15% were abandoned** and **34.85% resulted in a purchase**.
- Website engagement showed only a **small difference** between purchasing and non-purchasing sessions.
- Cart abandonment rates were relatively similar across product price bands.
- Purchase conversion rates were also very similar across discount bands.
- Product rating showed a statistically significant association with repeat-customer status at the customer level.
- The chi-square test for rating vs repeat-customer status produced:
  - Chi-square statistic: **104.76**
  - p-value: **1.47 × 10⁻²²**
- Marketing-channel conversion rates ranged from approximately **21.66% to 23.60%**, indicating relatively small differences.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Google Colab / Jupyter Notebook

## Repository Structure

```text
ecommerce-conversion-analysis/
│
├── ecommerce_conversion_analysis.ipynb
├── requirements.txt
├── README.md
├── project_report.docx
└── data/
    └── dataset.csv
```

> The dataset itself may be excluded from the repository if its source or license does not permit redistribution.

## How to Run

### 1. Clone/download the project

Open the notebook in Google Colab or Jupyter Notebook.

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Load the dataset

Place the CSV file in the expected location and update the notebook's file path if necessary.

### 4. Run the notebook

Execute the notebook cells sequentially from data loading through the final business recommendations.

## Business Takeaways

The analysis indicates that cart abandonment is a major conversion challenge. Meanwhile, simply increasing discounts or targeting higher-priced products does not appear sufficient to explain conversion behavior in this dataset.

The strongest analytical signal identified was the association between product ratings and repeat-customer behavior. This suggests that customer feedback and product quality deserve attention alongside conversion optimization.

## Limitations

- The dataset is suitable for analytical practice and business exploration, but conclusions should be interpreted within the scope of the available data.
- Observational associations do not establish causation.
- Marketing-channel analysis does not account for acquisition cost or customer lifetime value.
- Cart abandonment identifies the size of the problem but does not by itself identify the causal reason for abandonment.
- The analysis does not use machine learning for prediction because the primary objective is descriptive and hypothesis-driven business analytics.

## Author

**Sohini Dutta**  
B.Sc. Data Science  
NSHM Knowledge Campus Kolkata
