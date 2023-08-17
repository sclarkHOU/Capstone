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
![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/9e85a1b6-3b2c-4cec-b53b-98baaf7d76a6)

While only account for 32% of the products in the dataset it had a 69% reorder rate

Lastly, the longer a customer spent looking for and adding items to their cart the chance of reorders dropped. Producted recommendations early into the shopping experience is key
![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/f5cc5bd4-4d1c-4f53-a8d7-22494940a8a7)

## Apriori & Association Rules
The primary objective of utilizing the Apriori algorithm and association rules was to unravel hidden relationships between products and to gain insights into customer purchasing behavior and understand which products tend to be bought together. This approach allows GreenGrocer to offer a seamless and personalized shopping experience to our online customers. By deciphering the relationships between organic products often chosen together, we can provide tailored product recommendations and enhance the virtual shopping journey. These insights not only allow us to tailor recommendations but also deepened our comprehension of our customers' organic preferences, solidifying our commitment to delivering quality and convenience.

![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/1c743d7d-ef17-4152-8030-9c9bbf93071e)

## Modeling
- **Decision Tree**
  - F1-score = **0.81**
- **XGBoostClassifier**
  - Final Model
  - F1-Score = **0.84**
  - AUC-PR: **0.89**
    - The Dataset was highly imbalanced so to validate performance I looked at the Precision-Recall Curve. The AUC-PR score of 89% indicates that our XGB model is effective at identifying reorders by customers. It strikes a balance between correctly identifying reorders and avoiding misclassification.
      
 ![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/3bea1691-8710-477a-9d0b-a20fe228d163)
 
  - Feature Importance
    
    We took those feature importances from our XGBoost Model and ran them into a Logistic Regression to gain insights from the features

- **Logistic Regression**
  F1-Score = **0.82**

## Conclusions
Based on the analysis here are actionable recommendations:

**1. Promote Organic Produce:**
- Targeted marketing campaigns on organic products
- Highlight the benefits of organic items to attract and retain customers
  
**2. Encourage Frequent Purchases:**
- Implement Loyalty programs & Subscription options
- Personalize recommendations based on purchase history/frequent purchases
  
**3. Leverage Basket Size:**
- Implement strategies to encourage customers to add more items to carts 
- Bundle related products
- Special deals for bulk purchases
  
**4. Enhance Product Placement:**
- Products added later to the cart have a lower chance of being reordered. Explore ways to streamline the add-to-cart process and ensure that customers find what they need quickly
- Optimize the user interface for easier shopping
- Implement "quick add" or one-click reordering features

In conclusion, by implementing these recommendations, GreenGrocer can enhance customer satisfaction, increase customer retention, and drive higher reorder rates, ultimately leading to improved business performance and growth.

## Future Steps
- Collect more data on Organic products and shoppers.
- Use Apriori and Association rule results to build a recommendation system.
- With the right computational resources I would like to explore alternative ways to handle class imbalance and engineer more features.
- Apply Deep Learning models to extract better insights from the data.
- Continuously monitor the impact of these recommendations and Use A/B testing to evaluate the effectiveness of the different strategies.

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

├── Association_Rule.ipynb

├── 
