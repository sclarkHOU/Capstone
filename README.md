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
  
***
## Data Analysis
Organic Produce Fresh Products dominate carts. By making sure to have the produce department stocked increase the probability of reorders
![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/738c6a17-78d5-481b-8d2e-15fec0beee01)


![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/07c16a2e-ce9a-40f8-9cca-975da03e7c93)
![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/9e85a1b6-3b2c-4cec-b53b-98baaf7d76a6)

While only account for 32% of the products in the dataset it had a 69% reorder rate

Lastly, the longer a customer spent looking for and adding items to their cart the chance of reorders dropped. Producted recommendations early into the shopping experience is key
![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/df5a9e05-af07-4884-b01f-b9dfe961127a)

** **
## Apriori & Association Rules
The primary objective of utilizing the Apriori algorithm and association rules was to unravel hidden relationships between products and to gain insights into customer purchasing behavior and understand which products tend to be bought together. This approach allows GreenGrocer to offer a seamless and personalized shopping experience to our online customers. By deciphering the relationships between organic products often chosen together, we can provide tailored product recommendations and enhance the virtual shopping journey. These insights not only allow us to tailor recommendations but also deepened our comprehension of our customers' organic preferences, solidifying our commitment to delivering quality and convenience.

![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/1c743d7d-ef17-4152-8030-9c9bbf93071e)

** **
## Modeling
The Instacart dataset contains historical order information, including product details, user behavior, and order characteristics. Our goal is to use a predictive model to analyze which features influence a customer's likelihood to reorder organic products. By examining the model's coefficients, we can gain insights into which features have the most significant impact on the prediction.

- **Decision Tree**
  - F1-score = **0.81**
- **XGBoostClassifier**
  - Final Model
  - F1-Score = **0.84**

    I took the top feature importances from my XGBoost Model and ran them into a Logistic Regression to gain insights from the features

- **Logistic Regression**
  F1-Score = **0.82**

** **
## Conclusions
Based on the analysis here are actionable recommendations:

**1. Promotions & Marketing:**
- Targeted marketing campaigns on Organic produce
  
**2. Encourage Frequent Purchases:**
- Personalize recommendations based on purchase history, frequent purchases, and similar products purchased by other customers
  
**3. Customer Retention:**
- Offer Subscription and/or Loyalty Rewards programs

**4. Enhance Product Placement:**
- Implement "quick add" or one-click reordering features for faster checkout

In conclusion, by implementing these recommendations, GreenGrocer can enhance customer satisfaction, increase customer retention, and drive higher reorder rates, ultimately leading to improved business performance and growth.

** **
## Future Steps
- Use Apriori and Association rule results to build a recommendation system.
- With the right computational resources I would like to explore alternative ways to handle class imbalance and engineer more features.
- Apply Deep Learning models to extract better insights from the data.

** **
## For More Information
If you have any questions, please contact me:
- **Email:** stuartclark281@gmail.com
- **Linkedin:** https://www.linkedin.com/in/stuart-clark-185034123/

** **
### Repository Contents
├── data

├── images

├── Association_Rules.ipynb

├── Final_Model.ipynb

├── Organic_Market_Basket_Analysis.pdf

├── Organic_Market_Basket_Analysis.ipynb

├── README.m
