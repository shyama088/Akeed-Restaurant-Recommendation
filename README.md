# Akeed-Restaurant-Recommendation
Akeed is a delivery service app in Oman. Akeed’s vision is to be the delivery and
discovery platform for everything people need instantly. Akeed approaches the dimensions of
food delivery by taking the order, routing it to a restaurant, picking up the order and delivering it
to the customer.

1. ****Business Problem****

The objective of this challenge is to build a recommendation engine to predict what restaurants
customers are most likely to order from given the customer location, restaurant information, and
the customer order history.

Predict if the customer will make an order (target variable = 1) or will not make an order (target
variable = 0) from a given restaurant given the customer’s location, restaurant information and
order history of the customer

![image](https://user-images.githubusercontent.com/59326106/133022222-275cef97-a3c9-4954-a119-320f236e7e74.png)

2. **ML formulation of the business problem**

For a given customer at a given location number and restaurant, predict if the customer will order from the restaurant or not.
The goal is to make customized recommendations to the customer. Therefore it is a
recommendation. It can also be seen as a classification problem (if the user will order or not
order from a restaurant

3. **Business constraints**

![image](https://user-images.githubusercontent.com/59326106/133022343-7c4c48b4-a650-4db9-b6f8-5a8d861cead7.png)

Considering the above table, let’s assume that in the original data, customer C1(Alice) has
ordered from R1 (KFC) but not from R3 (McDonald’s). The target value of C1(Alice) for R3
(McDonald’s) was predicted to be 1. Hence R3 (McDonalds) will be recommended to C1 (Alice)
the next time. In this case, R3(McDonald’s) is recommended because of R1 (KFC). Letting the
customer know this, will increase the trust of the customer in the recommendation system
Hence some form of interpretability is required

4. **Datasets**

*  Orders
*  Vendors (Restaurant)
*  Train customers
*  Train location (location of the customers)
*  Test customers
*  Test customers (location of the customers)


5. **Performance metric**

The error metric is the F1 score, which ranges from 0 (total failure) to 1 (perfect score). Hence,
the closer your score is to 1, the better your model.

1. **F1 Score:** A performance score that combines both precision and recall. It is a harmonic mean of
these two variables. The formula is given as 2*Precision*Recall/(Precision + Recall)
2. **Precision:** This is an indicator of the number of items correctly identified as positive out of the
total items identified as positive. The formula is given as TP/(TP+FP)
3. **Recall / Sensitivity / True Positive Rate (TPR):** This is an indicator of the number of items
correctly identified as positive out of total actual positives. The formula is given as TP/(TP+FN)
where:
TP=True Positive FP=False Positive
TN=True Negative FN=False Negative

**Link :** https://zindi.africa/competitions/akeed-restaurant-recommendation-challenge
