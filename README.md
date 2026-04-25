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


<img width="586" height="288" alt="heatmap" src="https://github.com/user-attachments/assets/dfbc0981-3968-42fc-9c59-a79036a2067c" />

---


<img width="461" height="286" alt="dow" src="https://github.com/user-attachments/assets/6f5cde05-3368-41b5-bd8c-8452f747345f" />


---


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

<img width="643" height="330" alt="aisle-high-reorder" src="https://github.com/user-attachments/assets/46b9d4d6-86da-4a49-bb1e-57670f1932d3" />

---


<img width="630" height="334" alt="aisle-low-reorder" src="https://github.com/user-attachments/assets/efd973fc-6e23-457d-935b-783ab37f1092" />

---


<img width="649" height="317" alt="popular-aisles" src="https://github.com/user-attachments/assets/9ec7096c-f54d-49e7-b45c-c981ed804675" />





## Machine Learning Models
- XGBoost Classifier
- Artificial Neural Network (ANN)

Features include:
- Product-level features
- User-level behavior features
- Aisle & department encoding
- User-product interaction features

Evaluation metric: ROC-AUC

- Artificial Neural Network (ANN)

  
  <img width="394" height="188" alt="NN Architecture" src="https://github.com/user-attachments/assets/0c3cd3d0-1b75-4f89-97b4-6575c409e61f" />

  ---

  
<img width="296" height="152" alt="NN-Report" src="https://github.com/user-attachments/assets/8631e999-4343-453f-b062-c06cb79ad3ce" />

---


<img width="491" height="254" alt="NN-Performance" src="https://github.com/user-attachments/assets/77a6a54f-4d38-456b-b0ba-02e83a531385" />

---

- XGBoost Classifier


<img width="306" height="157" alt="XGBoost-Report" src="https://github.com/user-attachments/assets/2de56341-62ad-449e-8ab2-213419cacbcc" />

---

<img width="503" height="256" alt="XGBoost Performance" src="https://github.com/user-attachments/assets/a593235a-c96a-41c4-b1c3-12207ba82882" />




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


