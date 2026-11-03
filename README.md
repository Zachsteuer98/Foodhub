# FoodHub order analysis

A portfolio case study of restaurant demand, customer ratings, order cost, and delivery performance using 1,898 FoodHub orders.

### Context

The number of restaurants in New York is increasing day by day. Lots of students and busy professionals rely on those restaurants due to their hectic lifestyles. Online food delivery service is a great option for them. It provides them with good food from their favorite restaurants. A food aggregator company FoodHub offers access to multiple restaurants through a single smartphone app.

The app allows the restaurants to receive a direct online order from a customer. The app assigns a delivery person from the company to pick up the order after it is confirmed by the restaurant. The delivery person then uses the map to reach the restaurant and waits for the food package. Once the food package is handed over to the delivery person, he/she confirms the pick-up in the app and travels to the customer's location to deliver the food. The delivery person confirms the drop-off in the app after delivering the food package to the customer. The customer can rate the order in the app. The food aggregator earns money by collecting a fixed margin of the delivery order from the restaurants.

### Objective

The food aggregator company has stored the data of the different orders made by the registered customers in their online portal. They want to analyze the data to get a fair idea about the demand of different restaurants which will help them in enhancing their customer experience. Suppose you are hired as a Data Scientist in this company and the Data Science team has shared some of the key questions that need to be answered. Perform the data analysis to find answers to these questions that will help the company to improve the business.

### Data Description

The data contains the different data related to a food order. The detailed data dictionary is given below.

### Data Dictionary

* order_id: Unique ID of the order
* customer_id: ID of the customer who ordered the food
* restaurant_name: Name of the restaurant
* cuisine_type: Cuisine ordered by the customer
* cost_of_the_order: Cost of the order
* day_of_the_week: Indicates whether the order is placed on a weekday or weekend (The weekday is from Monday to Friday and the weekend is Saturday and Sunday)
* rating: Rating given by the customer out of 5
* food_preparation_time: Time (in minutes) taken by the restaurant to prepare the food. This is calculated by taking the difference between the timestamps of the restaurant's order confirmation and the delivery person's pick-up confirmation.
* delivery_time: Time (in minutes) taken by the delivery person to deliver the food package. This is calculated by taking the difference between the timestamps of the delivery person's pick-up confirmation and drop-off information

## Analysis process

The presentation follows the analysis from the original project: profile the dataset and rating completeness; examine restaurant, cuisine, cost, rating, preparation-time, and delivery-time distributions; compare demand and service measures across categories; answer the business questions; then summarize findings and recommendations.

Charts include frequency bars, cost and time histograms and boxplots, cuisine-by-day and prep-by-delivery heatmaps, cuisine price comparisons, prep time by rating, and delivery-time comparisons by day and cuisine.

## Conclusions:
*  The analysis reveals clear patterns in customer demand, pricing behavior, and operational performance. In general more orders are being placed on Weekends vs the Weekday. and the majority of orders are being made for American, Japanese, Italian, and Chinese cuisines. Orders are being placed with mostly the same small group of restaurants, with just 21 out of 178 restaurants generating the majority of the platforms activity.

Prices tend to be less per dish with popular cusines, likely being influenced by the food being inexpensive and easy to share. It is also apparent that there is a strong niche of restaurants that recieve less demand but have pricier food options such as vietnamese, and French food.

From an Operational standpoint, Foodhub is extremely reliable when it comes to delivery times. With only 10.54% of deliveries taking more than 60 minutes. The majority of orders are being prepared + delivered in 45-60 minute time window. This could also contribute to why there are no 1-3 star ratings. I found this very odd, more research should go into why low rating reviews are not being recieved in this size dataset.

Overall, Foodhub is generating the majority of its revenue from the top 5 most popular cuisines. their delivery times are extremely reliable, niche restaurants are an area to grow demand during the weekday due ideal marketing conditions, and there are clear areas for improvement and operational efficiency.

## Recommendations:

*  Reduce additional fees during weekday delivery to incentize customers to order food during the slower days of the week.

* Promote Niche restaurants during the week given that it's likely 1-2 person orders are their strength vs on weekends promoting top cuisines and family/group order options with restaurant providers.

* There is a large amount of restaurants of Foodhub that don't recieve orders yet work with the service. Diving deeper into why these restaurants don't recieve orders is imperitive. I feel the likely solution is to promote less frequented restaurants on weekdays when customers are likely to be coming home from work and don't want to cook a meal. Incentizing regular customers with promotions to feed with these restaurants could build up their reputation and bring in more business for Foodhub and their supporting restaurants.

* On the Foodhub app, their front end team should be filtering the top 5 categories so they are easy to find.

## Open the presentation

Open [`foodhub_dashboard.html`](foodhub_dashboard.html) in a modern browser. The standalone page includes the full dataset, interactive filters, and CSV export; it requires no server or package installation. Use **Print / Save PDF** to create a static copy.