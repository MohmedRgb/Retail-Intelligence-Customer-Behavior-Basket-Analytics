# Retail-Intelligence-Customer-Behavior-Basket-Analytics
## Overview
This project analyzes Instacart’s anonymized grocery orders dataset (~3M orders, 200K+ users) to discover customer purchasing behavior, product associations, and build predictive models for product reorders.


## Objectives
- Discover hidden product associations for cross-selling and upselling
- Perform customer segmentation for targeted marketing
- Analyze customer purchase behavior
- Build ML models to predict product reorders


## Dataset
The dataset contains:
- Orders data (3.4M+ orders)
- Products (49K+ products)
- Aisles (134 categories)
- Departments (21 categories)
- Order-product relationships (prior & train sets)


## Project Structure

├── Plots/
├── Data Description and Analysis.ipynb
├── Exploratory Data Analysis.ipynb
├── Customers Segmentation.ipynb
├── Market Basket Analysis.ipynb
├── Feature Extraction.ipynb
├── Data Preparation.ipynb
├── NN Model.ipynb
├── XGBoost Model.ipynb
└── README.md





## Key Insights
- Most orders are placed on weekends (Saturday & Sunday)
- Majority of users reorder weekly
- Organic products have higher reorder rates
- 85% of users purchase only ~10K products out of 49K
- Fruits and vegetables dominate customer purchases



## Market Basket Analysis
Applied Apriori algorithm to discover product associations using support, confidence, and lift metrics. Found strong associations between products like organic fruits and fresh produce.





## Machine Learning Models
- XGBoost Classifier
- Artificial Neural Network (ANN)

Features include:
- Product-level features
- User-level behavior features
- Aisle & department encoding
- User-product interaction features

Evaluation metric: ROC-AUC




## Results
- XGBoost slightly outperformed ANN in ROC-AUC score
- Feature importance showed strong influence of product popularity and user behavior




## Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- TensorFlow / Keras
- Mlxtend (Apriori)
- Matplotlib, Seaborn


## Future Work
- Implement collaborative filtering recommendation system
- Deploy model as a web app
- Real-time recommendation engine




## Conclusion
This project demonstrates how large-scale retail data can be leveraged to understand customer behavior, optimize product placement, and build predictive recommendation systems.


