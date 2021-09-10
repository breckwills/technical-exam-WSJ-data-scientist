  Welcome to the WSJ Data Science technical test for the membership team. This exam is designed to give you an opportunity to demonstrate your ability to work with structured datasets. You should not spend more than an hour working on it. Focus on clarity over completeness. If you don't have time to answer a certain question, describe how you would approach solving it instead.

  Please submit answers in either R or Python (Jupyter notebooks preferred). Email zipped files to breck.wills@dowjones.com.

## Scenario

  A hypothetical investing blog wants to improve their paywall performance. The publisher would like to use a predictive model to identify which types of traffic are most likely to convert. Examine the dataset provided and create a model that will be able to predict the likelihood of a user subscribing on a specific article.

**Notes: 
Each row in `propensity_data.csv` represents a single page view.
**
Conversion rates on specific days or times can be highly correlated for all visitors due the content being published. 
**
Assume a one-to-one relationship between page views and conversions (i.e. a conversion will only be attributed to a single page view).
**
## Data 

| Column Name     | Description       |
| --------------- | ----------------- |
| pageID | unique ID for each instance of a reader viewing an article
| paywall | whether the article was locked or open
| time | date and time the page view occurred
| daysSinceFirstSeen | number of days between when the article was read and when the user first visited
| section | section of the article read
| visitNum | visit count of the article read (e.g. if 2, this is their second visit in last 28 days)
| pageNum | page count of the article read (e.g. if 2, this is their second page view in their current visit)
| registered | binary of user's logged in status (registration is free and not a subscription)
| edu | binary of whether a user is visiting from an edu domain (`1` = "edu domain")
| mobile | binary of whether a user is on a mobile phone (`1` = "mobile phone")
| mac | binary describing whether a user is on an Apple device (`1` = "Apple device")
| converted | binary describing whether the user subscribed immediately after the page view (`1` = "subscribed")


## Questions

  1. What is the base rate of conversion for locked versus open pages?
  
  2. What percent of article views are paywalled?
  
  3. Create a model predicting which page views result in a conversion.
  
        a. Which variables are the strongest predictors of conversion?
        
        b. What measures would you use to assess the performance of this model?
        
  4. What recommendations, if any, would you make to the publisher based on your findings?    
        
  5. Create two visualizations that back up your recommendations.
