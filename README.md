# Organic Market Basket Analysis
![image](https://github.com/sclarkHOU/Capstone/assets/56837718/d3657590-160b-46bb-bf26-f7a5f2e23f94)

## Business Overview
The organic grocery market is experiencing rapid growth, driven by increasing consumer awareness of health and sustainability. Today the global Organic food market is worth $176 billion and is estimated to grow at a CAGR of 12.1%, earning revenue of around $553 billion by the end of 2033.

With the demand for organic products and online shopping on the rise, GreenGrocer wants to strategically position itself to tap into this expanding market by introducing an Organic Grocery Delivery Service.GreenGrocer wants to continue to elevate the customer experience and has tasked us to find key factors for predicting customer reorders to optimize marketing strategies and identify frequently purchased items for improved product recommendations and cross-selling opportunities. 

## Data Overview
The dataset comes from 3 million grocery orders from more than 200,000 Instacart users. The data was filtered down to only focus on Organic Products. The dataset includes information on the following:
- 5000 Organic products
- 190,000 users who have purchased Organic products
- 2.3 million orders containing Organic products

## Data Analysis
- Key Findings

## Modeling
- Decision Tree Classifier
  - Baseline Model - The model was overfitting
  - Train F1-Score: 1.0
- Decision Tree with a max_depth=7
  - F1-score = 0.81 on both Test and Train data
- Logistic Regression
  - Used the top features from the Decision Tree Classifier to get Coefficents and Odds Ratios for those Features
  - F1-Score = 79% on both Test and Train data
- XGBoostClassifier
  - Final Model
  - F1-Score = 0.82 for both Train and Test data
- Apriori Algorithm
  - Text
    - Text

## Conclusions
- Text
- 
## For More Information
If you have any questions, please contact me:
- **Email:** stuartclark281@gmail.com
- **Linkedin:** https://www.linkedin.com/in/stuart-clark-185034123/

### Repository Contents
├── data

├── images

├── README.md

├── Organic Market Basket Analysis.ipynb

├── Model.ipynb

├── Association Rule/Aprior Model.ipynb

├── 
