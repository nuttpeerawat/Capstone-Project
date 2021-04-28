# Capstone-Project 

## Contents: 
- Problem Statement 
- Executive Summary 
- Data Dictionary p.s. There are some problem when I try to upload data to github, so I upload dataset that I used in this link: https://drive.google.com/drive/folders/1NwWdB3tUeRM_ICN8fbEjuQwUo2D3o4Ao?usp=sharing 
- Conclusions and Recommendations 
------------------------------------------------------------------------ 
## Problem Statement 

Since the pandemic of covid 19 many people have decreased their visits to restaurants and have turned to online food delivery services for their daily meals and many delivery apps recommend users restaurants based on their location which it may not meet the preferences of the customer enough. This project aims to increase the number of users of food delivery apps by creating a restaurant recommendation system based on their preferences. 

------------------------------------------------------------------------ 
## Data Dictionary 
| Feature           | Type         | Description                                | 
| :---------------: | :----------: | -----------------------------------------: | 
|busines categories | object       | categories of restaurant       | 
|business city        | object         | city of restaurants | 
|business id      | object        | id of the restaurant  | 
|business latitude        | float        | latitude of restaurant             | 
|business longitude        | float        | longitude of restaurant             | 
|business name         | object          | restaurant name | 
|business_review_count | int          | total review of that restaurant | 
|business stars      | int          | restaurant star              | 
|date     | object          | review date             | 
|review id          | int          | reviewer id | 
|review average stars | float       | average rating of all reviewer give to all restaurant | 
|stars       | float        | business stars/rating              | 
|text      | object          | review text            | 
|user_id           | object       | ID of user                            | 
|categories       | object       | categories of restaurant                           | 
|dominant_topic         | object       | dominant topic of each review that got doing from topic modeling                            | 
|topic_keywords        | object       | keyword of review text that got from doing topic modeling                            | 
------------------------------------------------------------------------ 
## Conclusions and Recommendations 

In this project I have created 3 recommendation system which are location based recommendation system, content based recommendation system and collaborative recommendation system 
- For location-based recommendation system I done by calculating distance between location from latitude and longitude data, to use this recommendation system a user can input their latitude and longitude location then it will find nearest 5 high rating restaurants (4-5 stars) near user location and also return the distance it meters. 
- For content-based recommendation system I done by do the topic modeling in review text from user to get the keyword from each restaurant then combined with the categories of restaurant after that use count vectorizer and cosine similarity to get similar restaurants. To use this model the user has to input restaurant name and it will return top 10 restaurants based on content of the restaurant 
- For collaborative recommendation system I done by use each user rating for each restaurant then use singular value decomposition and cosine similarity to get similar restaurants. To use this model user has to input restaurant name and it will return top 10 restaurants based on the rating. 

## Limitation And Future Improvement 
- This project use dataset from yelp in 2005 to 2013 which is outdated so it would be better if use dataset that upto date. In terms of what can be done to improve these models in the future: 
-  1. Do sentiment analysis in review text 
-  2. Do evaluation on the model 
-  3. Incorporate Neural Network and Deep Learning Concepts into collaborative filtering recommendation system.
