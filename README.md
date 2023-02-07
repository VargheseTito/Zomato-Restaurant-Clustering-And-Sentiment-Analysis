
# Zomato Restaurant Clustering and Sentiment Analysis


![This is an image](https://cdn.businesstraveller.com/wp-content/uploads/fly-images/951047/zomato-infinity-dining-916x516.jpg)

Analyzed the sentiment of the Zomato customer reviews to find the best restaurant in the city.




## Problem Statement

Your task is to cluster the Zomato restaurants into different segments. Also, the data has valuable information around cuisine and costs which can be used in cost vs. benefit analysis Perform sentiment analysis. Also, use the metadata of reviewers to identify the critics in the industry.
## Project Description

In this Project, I have focused on Customer reviews and Restaurants and analyzed the sentiments of the reviews given by the customer in the data and also, clustered the zomato restaurants into different segments to get some useful insight in the form of Visualizations. 

The Analysis helped us to solve one of the business use cases that can directly help the customers in finding the Best restaurant in their locality and for the company to grow up and work in the fields they are currently lagging in.

![This is an image](https://media1.tenor.com/images/20a76877c457c73ee740e3994b8852e8/tenor.gif?itemid=17778952)

Challenges-

Handling and cleaning large amounts of review data using NLP techniques such as stopwords, lemmatization and vectorization using TF-IDF.

Choosing the right number of clusters using various methods.

Exploring different ML algorithms to find the model with the highest predictive power. 
## Demo



![This is an image](https://image.slidesharecdn.com/zomatomt5016-160407053633/95/zomato-transforming-the-global-restaurant-business-36-638.jpg?cb=1460008392)
## About the data

There are two data files

"Zomato restaurant reviews" has the Name of the Restaurant, Name of the customer, their review, rating, follower details, Time of Review, and the number of photos uploaded along with the review. This data has been mainly used for Sentiment analysis.

Restaurant: Name of the Restaurant
Reviewer: Name of the Reviewer
Review: Review Text
Rating: Rating Provided by Reviewer
MetaData: Reviewer Metadata - No. of Reviews and followers
Time: Date and Time of Review
Pictures: No. of pictures posted with the review
"Zomato Restaurant names and Metadata" has the details of the Name of the Restaurant, Link to order on their restaurant on Zomato, Average cost, Tags for the restaurants, Cuisines, and timings. This data has been mainly used for clustering.

Name: Name of Restaurants
Links: URL Links of Restaurants
Cost: Per person estimated Cost of dining
Collection: Tagging of Restaurants w.r.t. Zomato categories
Cuisines: Cuisines served by Restaurants
Timings: Restaurant Timings
## Steps Involved


Null values Treatment
The data set had null values out of which we replaced some with the mean of the feature some by zero and dropped some observations which were almost filled with null values.



Exploratory Data Analysis
We performed univariate and bivariate analyses. This process helped us figure out various aspects and relationships among variables. It gave us a better idea of which feature behaves in which manner.

Encoding of categorical columns
We used One Hot Encoding(converting to dummy variables) to produce binary integers of 0 and 1 to encode our categorical features because categorical features that are in string format cannot be understood by the machine and needs to be converted to the numerical format.

Standardization of features
Our main motive through this step was to scale our data into a uniform format that would allow us to utilize the data in a better way while performing fitting and applying different algorithms to it. The basic goal was to enforce a level of consistency or uniformity to certain practices or operations within the selected environment.

Fitting different models
For modeling, we tried various algorithms like:

Clustering
K means clustering
Hierarchical clustering
MultinomialNB
Logistic Regression
Decision Tree
Random Forest Classification
XGBoost Classification
LightGBM Classification

Tuning the hyperparameters for better recall
It is necessary to tune the hyperparameters of respective algorithms to improve accuracy and avoid overfitting when using tree-based models such as Random Forest Classifier and XGBoost classifier. The best set of hyperparameters was determined using a grid search algorithm.



Deciding number of cluster
Elbow Method 
From the above graph we selected the number of cluster(k) should be between 3 and 5

Performance Matrix
Clustering
Silhouette score 
It can be seen that the silhouette score for k=4 is the highest



## Conclusion

1. The Restaurant with the highest rating of nearly 4.8 and good reviews is the AB's Absolute Barbecues. On the contrary, the restaurant with worst reviews and rating is the Hotel Zara Hifi
with a rating less than 2.5.

2. The most expensive Cuisine is the Modern India cuisine which
cost around 2000 rupees and the least expensive item available at
a cost of 200 rupees is the Mithai

3. The collage-Hyatt Hyderbad Gachibowli is the most expensive restaurant available and the most affordable restaurant for the customers are the Amul and Mohammedia Shawarma.

4. The most popular cuisines available in the most of the restaurant is the North Indian and Chinese.

5. The most frequent working hours of the restaurant is between 11am to 11pm.

6. The billing amount of rupees 500 is the most frequent cost paid by the customers on their order.

7. Restaurant Clustering was done in with just two features Cost and Rating. Kmeans Clustering gave us optimal cluster value as 5 but we have done our clustering analysis based upon the principal component analysis because the similarities in the data points within the clusters were pretty great. We have got optimal clusters as 4 clusters in PCA.

8. Sentiment Analysis was done on the reviews and a model was trained in order to identify negative and positive sentiments. The best model for sentiment analysis we found out to be XGboost,LightGBM and Logistic Regression model.
## Recommendations

Ratings should be collected on a
category basis such as rating for
packaging, delivery, taste,
quality, quantity, service, etc.
This would help in targetting
specific fields that are lagging.
## Contribute

Tito Varghese | Data Science Trainee | Machine Learning |

https://www.linkedin.com/in/tito-varghese