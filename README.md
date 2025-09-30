# Customer Segmentation: E-Commerce Clothing Company

![Python](https://img.shields.io/badge/language-Python-blue)
![Jupyter Notebook](https://img.shields.io/badge/output-Jupyter%20Notebook-orange)

## Overview

This repository contains a customer segmentation analysis for an e-commerce clothing company, developed as a final project for the Machine Learning course. The goal is to cluster customers to identify target groups and tailor product promotions effectively. 

The dataset contains customer demographic and purchase data. After removing irrelevant or high-cardinality features, and encoding categorical variables, K-Means clustering is applied to segment customers.

---

## Repository Structure

- `2A.tsv` → raw dataset of clothing company customers
- `customer_clustering.ipynb` → main notebook containing EDA, preprocessing, K-Means clustering, and persona analysis

---

## Methodology

1. **Data Preprocessing**
   - Dropped irrelevant columns (e.g., Customer ID, Item Purchased, Size, Color, Payment Method)
   - Encoded categorical variables using LabelEncoder, OrdinalEncoder, and OneHotEncoder
   - Grouped locations into broader regions to reduce complexity

3. **Clustering**
   - K-Means clustering applied with the optimal number of clusters determined via silhouette score and the elbow method
   - Two clusters identified as the most meaningful segmentation

5. **Persona Analysis**
   - Compared clusters on numerical features (Purchase Amount, Previous Purchases) and categorical distributions
   - Characterized clusters as **Premium Shoppers** and **Budget Shoppers** to guide promotion strategies

---

## Key Insights

- Two clear customer segments emerged: **Premium Shoppers** (higher spending per purchase) and **Budget Shoppers** (lower spending per purchase).
- Clustering primarily reflects spending behavior; other categorical features showed minimal differences.
- The segmentation enables targeted promotions: premium offers for high-spending customers and discounts or bundles for price-sensitive customers.
- Preprocessing and encoding ensure the data is clean and structured for clustering.

---

## Presentation Video

[Customer Segmentation Analysis – Video Presentation](https://drive.google.com/file/d/1LOYaykReHVPdNqa_T7OmoFaqJu4HzvXU/view?usp=sharing)

---

## References

* Python libraries: pandas, scikit-learn, matplotlib, seaborn

---

## Author

Syalista Galuh Nadira
