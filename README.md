# Organic Market Basket Analysis
![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/c5b6605e-e28a-4f2a-b185-0f44366785c5)



## Business Overview
The organic grocery market is experiencing rapid growth, driven by increasing consumer awareness of health and sustainability. Today the global Organic food market is worth $176 billion and is estimated to grow at a CAGR of 12.1%, earning revenue of around $553 billion by the end of 2033.

With the demand for organic products and online shopping on the rise, GreenGrocer wants to strategically position itself to tap into this expanding market by introducing an Organic Grocery Delivery Service.GreenGrocer wants to continue to elevate the customer experience and has tasked us to find key factors for predicting customer reorders to optimize marketing strategies and identify frequently purchased items for improved product recommendations and cross-selling opportunities. 

## Data Overview
The dataset comes from 3 million grocery orders from more than 200,000 Instacart users. The data was filtered down to only focus on Organic Products. The dataset includes information on the following:
- 5000 Organic products
- 190,000 users who have purchased Organic products
- 2.3 million orders containing Organic products

## Data Analysis
Organic Produce Fresh Products dominate carts. By making sure to have the produce department stocked increase the probability of reorders
![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/aa3194e6-2df6-4026-b519-6345c0efdf48)

![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/07c16a2e-ce9a-40f8-9cca-975da03e7c93)

While only account for 32% of the products in the dataset it had a 67% reorder rate
![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/9e85a1b6-3b2c-4cec-b53b-98baaf7d76a6)

Lastly, the longer a customer spent looking for and adding items to their cart the chance of reorders dropped. Producted recommendations early into the shopping experience is key
![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/f5cc5bd4-4d1c-4f53-a8d7-22494940a8a7)

## Modeling
- Decision Tree
  - F1-score = 0.81 on both Test and Train data
    
- XGBoostClassifier
  - Final Model
  - F1-Score = 0.83
  - AUC-PR: 0.89
 ![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/3bea1691-8710-477a-9d0b-a20fe228d163)

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
