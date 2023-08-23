<h1 align="center">  Organic Market Basket Analysis </h1>

![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/c5b6605e-e28a-4f2a-b185-0f44366785c5)

## Business Overview
The organic grocery market is experiencing rapid growth, driven by increasing consumer awareness of health and sustainability. Today the global Organic food market is worth $176 billion and is estimated to grow at a CAGR of 12.1%, earning revenue of around $553 billion by the end of 2033.

With increasing concerns about the use of pesticides, GMOs, and other harmful additives in conventional food products, more people are turning to organic food for a healthier and sustainable diets. 

With the demand for organic products and online shopping on the rise, GreenGrocer wants to strategically position itself to tap into this expanding market by introducing an Organic Grocery Delivery Service. GreenGrocer wants to continue to elevate the customer experience, I have been tasked with finding key factors for predicting customer reorders to optimize marketing strategies and identify frequently purchased items for improved product recommendations and cross-selling opportunities for GreenGrocer. 

## Data Overview
The dataset comes from 3 million grocery orders from more than 200,000 Instacart users. The data was filtered down to only focus on Organic Products. The dataset includes information on the following:
- 5000 Organic products
- 190,000 users who have purchased Organic products
- 2.3 million orders containing Organic products
  
***
## Data Analysis

#### While organic items only account for 32% of the products in the dataset it had a 69% reorder rate.

![image](https://github.com/sclarkHOU/Organic-Market-Basket-Analysis/assets/56837718/e2bffc22-94df-4fcb-a8fd-55f3170ecd68)

#### Organic Produce Fresh Products dominate carts. By making sure to have the produce department stocked increase the probability of reorders.

![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/738c6a17-78d5-481b-8d2e-15fec0beee01)

#### Lastly, Products that are added to the cart initially are more likely to be reordered again compared to the ones added later. Customers tend to first order all the products they buy frequently and then look out for the new products available.

![image](https://github.com/sclarkHOU/Organic-Market-Basket-Analysis/assets/56837718/b9c21a23-52b2-418d-9616-e97cd0417dbc)

** **
## Apriori & Association Rules
The primary objective of utilizing the Apriori algorithm and association rules was to unravel hidden relationships between products and to gain insights into customer purchasing behavior and understand which products tend to be bought together. This approach allows GreenGrocer to offer a seamless and personalized shopping experience to our online customers. By deciphering the relationships between organic products often chosen together, I can provide tailored product recommendations and enhance the virtual shopping journey. These insights not only allow me to tailor customer recommendations but also deepened the comprehension of our customers' organic preferences, solidifying GreenGrocer's commitment to delivering quality and convenience.

![image](https://github.com/sclarkHOU/Organic_Market_Basket_Analysis/assets/56837718/1c743d7d-ef17-4152-8030-9c9bbf93071e)

** **
## Modeling
The Instacart dataset contains historical order information, including product details, user behavior, and order characteristics. My goal is to use a predictive model to analyze which features influence a customer's likelihood to reorder organic products. By examining the model's coefficients, I can gain insights into which features have the most significant impact on the prediction.

I started with a decision tree to understand the relationship between features but due to my imbalanced data I transitioned to XGBoost for improved predictive power. Lastly I utilized logistic regression to interpret and quantify the impact of features.

Because of the imbalance in my data I not only wanted to identify positive instances but wanted to minimize instances where my model predicted a customer will reorder organic products but they do not. Leading to incorrect allocation of resources towards customers who are not likely to reorder organic products. I also wanted to minimize instances where my model suggested a customer does not reorder organic products but they do. Leading to missed opportunities to promote organic products to customers who are actually interested in them.

In a pursuit to find a balance between these two instances I used an F1-Score as my metric.

- **Decision Tree**
  - Basline Model
  - F1-score = **81%**
    
- **XGBoostClassifier**
  - Final Model
  - F1-Score = **84%**

- **Logistic Regression**
  - Interpret feature importances
  - F1-Score = **82%**

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
- Explore alternative ways to handle class imbalance and engineer more features.
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

├── Organic Market Basket Analysis Presentation.pdf

├── Organic_Market_Basket_Analysis.ipynb

├── README.md
