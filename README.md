# Instacart Next-Basket Recommender System

This project implements a next-basket recommender system for Instacart using advanced data science techniques. The primary goal is to enhance user retention, drive additional sales, and foster strategic partnerships through predictive analytics and personalized marketing.

---

## Overview

Instacart's historical purchasing data was leveraged to:
- **Predict next-basket recommendations:** Using the TIFU-KNN algorithm, users are provided personalized product suggestions to streamline shopping and boost engagement.
- **Identify high-potential users for targeted marketing campaigns:** A Decision Tree model was used to identify users likely to purchase specific products or shop in certain departments, enabling strategic partnerships with manufacturers and retailers.

---

## Features

1. **TIFU-KNN Recommendation Model**
   - Captures temporal user behavior and collaborative patterns for accurate predictions.
   - Achieved a **recall of 0.37**, significantly outperforming baseline models.
   - Supports personalized and relevant product recommendations to enhance the user experience.

2. **Decision Tree Model**
   - Identifies users with high purchasing potential in specific categories (e.g., snacks).
   - Enables personalized promotions and strategic partnerships with manufacturers.
   - Projected **$1.2 million in revenue growth** from personalized marketing campaigns.

3. **Comprehensive Data Pipeline**
   - Processed and analyzed **32 million rows** of transactional data.
   - Merged datasets from products, orders, departments, and aisles to build a robust foundation for analysis.
   - Incorporated category-level insights to refine predictive capabilities.

---

## Dataset

The project uses the publicly available [Instacart Kaggle Dataset](https://www.kaggle.com/c/instacart-market-basket-analysis), containing:
- **32 million+ rows** of transactional data.
- **206,000 unique users**.
- **50,000 unique products** across 21 departments and 134 aisles.

### Data Preprocessing
- Merged datasets to create a unified, structured view of user behavior.
- Excluded users with fewer than 3 orders to focus on active shoppers.
- Applied temporal decay to model evolving user preferences effectively.

---

## Models

### TIFU-KNN (Temporal-Item-Frequency-Based User KNN)
- Combines temporal dynamics and collaborative filtering.
- Incorporates time-decayed weights to emphasize recent purchases.
- Builds user vectors with both product-level and category-level preferences.

### Decision Tree
- Predicts user likelihood to purchase specific products or shop in specific departments.
- Features include order history, product preferences, and department-level trends.
- Facilitates personalized marketing strategies for manufacturers like PepsiCo.

---

## Results

1. **TIFU-KNN:**
   - Recall: **0.37** (compared to 0.11 for the baseline model).
   - Improved user engagement by recommending relevant items for cross-selling.

2. **Decision Tree:**
   - Identified snack-purchasing patterns to support targeted advertising.
   - Simplified feature engineering and explainable decision-making.

---

## Future Enhancements
- Incorporate additional features such as user demographics, time of purchase, and store location.
- Expand recommendation capabilities to include recipe suggestions and meal planning.
- Improve model scalability to handle larger datasets and real-time predictions.

---
## References
- Instacart Paper(TIFU-KNN) [Paper](https://arxiv.org/pdf/2006.00556)
