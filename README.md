# Conagra-Brands--Business-Analytics
Analyzed key drivers of real vs. alternative meat sales for Conagra Brands using feature engineering and machine learning; identified product, packaging, and availability factors impacting revenue.

# Conagra Brands: Real vs. Alternative Meat Sales Analysis

## Team Members
- Samarth Verma  
- Hiral Yadav  
- Vikramaditya Sriramachandra  
- Harsha Gurram  
- Kathyayani Chenimineni  
- Shriya Dubey  
- Pratham Khubchandani  

---

## Project Overview
This project analyzes why real meat products significantly outperform alternative meats in sales. By studying factors like packaging, cooking instructions, regional availability, and product popularity, we identify drivers of purchasing behavior and offer strategic recommendations to increase alternative meat revenue for Conagra Brands.

---

## Hypothesis
"If we create similar purchase experiences for real and alternative meat products, revenue from alternative meats will increase."

---

## Methodology

### Data Preparation
- Grouped data by Product UPC to create product-level features  
- Engineered new variables capturing geographic effects  
- Removed multicollinear variables and non-significant features using Chi-Square and correlation tests  
- Standardized numeric data and encoded categorical variables  
- Train-test split applied to ensure model validity  

### Modeling
- Forward Selection Regression to identify ranked drivers  
- Random Forest Regression with hyperparameter tuning  
  - Final model performance: **R² ≈ 0.81**

---

## Key Features Driving Sales

| Feature                    | Real Meat Importance | Alternative Meat Importance |
|---------------------------|----------------------|-----------------------------|
| ACV Weighted Distribution | 0.715                | 0.9836                      |
| Popularity                | 0.0778               | 0.0154                      |
| Price per Unit            | 0.0704               | 0.001                       |
| Cooking Info (Uncooked)   | 0.0342               | -                           |
| Packaging (Vacuum Packed) | 0.0194               | -                           |

---

## Business Recommendations

- Create alternative meat products that mimic real meat cooking instructions  
- Package alternative meat similarly to real meat while highlighting health benefits  
- Expand geographic availability to increase shelf presence  
- Offer product quantities and formats comparable to real meat SKUs  

---

## Limitations

- Lower observation count in some alternative meat segments may limit generalizability  
- Correlation-based insights; further experimentation is needed to establish causality  
