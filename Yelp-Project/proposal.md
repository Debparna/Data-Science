## Topic

**Sentiment Analysis On Yelp Reviews to Compare Reviews with Health Rating of Resturants**

We will perform sentiment analysis on yelp reviews related to the health and cleanliness of a restaurant. We will then use this analysis to give the restaurant a health rating and compare to the official health inspection rating to provide an accuracy score. 


## Summary 

The problem that we are trying to address is that health inspections are not always up to date, as there are many restaurants in big cities and it takes a lot of human capital, resources and money to physically conduct these inspections. Each year, millions of people cycle through and post yelp reviews of their experiences at restaurants. This information has the potential to help improve City’s health inspection efforts. Our topic is to analyze the safety and health of Yelp restaurant reviews using sentiment analysis and diction to assign a health rating of the restaurant. Then we will compare the health rating to City inspection ratings to determine the ‘accuracy’ or differences between City inspections and customer experiences. This data analysis will provide a more accurate picture of the conditions of the health of resturants and, by an addition of this feature, Yelp can help provide better recommendations to their users. It can be a convenient and up-to-date method for users to take into account the health quality of the restaurant while choosing one. 

## Questions to Consider

1. What are the overall sentiments of Yelp reviews for a restaurant? We will classify the reviews into positive and negative to help us rate the health of the restaurant.
2. According to Yelp, what are the complaints of a restaurant. How many of the yelp complaints are about the health risks of the restaurant? Categorize these into low, moderate, high risk. This data will be meaningful to the users of Yelp (they can immediately see how ‘risky’ eating at that restaurant is.
3. How do these health risks align with health inspection data? Are they the same? Is there a relation between yelp complaints of health risks and City inspection ratings? If so what is the relationship? This data will be meaningful to the City. City can see how aligned its ratings are with customers, and consider inspecting the specific things that customers have been complaining about.
4. What is the percentage of restaurants with incorrect or outdated health ratings? This can help prove that since yelp reviews are up to date and more realistic, they can be used as a more accurate health metric for restaurants. 


## Data Sources

1. Yelp Dataset

We will be using the yelp dataset to get review data from review.json. We will be parsing the json file to get the text of the customer reviews. The reviews will be separated if they are related to health comments on the restaurant. We will check each review against a word bank we create which contains popular health related words (e.g. hygiene, clean, dirty, etc.). We will then perform a sentiment analysis on the separated reviews to classify each review into health categories (low/moderate/high risk).

2. Health Inspection/Rating API (by city/county)

Once we have our own health rating for each restaurant based on the sentiment analysis of the yelp reviews, we will be using the official Health Inspection APIs for the relevant counties to compare our ratings to those. Each county has its own API for the health ratings of the restaurants in the county. We can use this as a metric for accuracy of the health rating according to actual reviews of the hygiene of the restaurant. 

## Challenges

This project will prove to be a challenge due to the fact we will be using various API’s and combining them together to create a metric that determines the health and safety ratings of a restaurant. Creating the metric through sentiment analysis will prove to be challenging since we will have to determine what features in a post influence this rating, and how each feature would be weighted in grading the metric fairly. The sentiment analysis might be one of the larger challenges, as this can get tricky in detecting negative traits that are not false positives. The next challenge would be in analyzing whether this aligns with City health inspection ratings, and what it would mean for the metric/customer reviews if it doesn’t.

## Skills

In this project, we are aiming to use many of the data science techniques we learned in this class such as data wrangling, cleaning and visualization of the results. We are performing sentiment analysis on the yelp dataset and as a result we will be performing statistical methods of classification and regression on the data to obtain these results. Since the data set is in json format, we will be implementing json parsing and data aggregation. We will also be using website API querying and searching for the official health inspection data, which are some of the techniques we learned in this class. We will use this additional data to compare our sentiment analysis results and for this we will be use algorithms to compare datasets and perform data analysis to draw conclusions from  the dataset. 

## Authors
1. Sarah Rahman
2. Debparna Pratiher
3. Zuhair Bhatti
4. Kavitha Dhanukodi



