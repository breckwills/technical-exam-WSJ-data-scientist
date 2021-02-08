  Welcome to the WSJ Data Science technical test for the membership team. Please submit answers in the form of a Jupyter notebook, in either R or Python. Please email zipped files to john.wiley@dowjones.com within three days of receiving the exam.

## Scenario

  A hypothetical investing blog wants to improve their paywall performance. Currently the paywall monitors some traffic variables to trigger a paywall for users, but they would like to improve the targeting with a predictive model. The goal of this exercise is to examine the propensity dataset provided and create a model that will be able to predict an user's likelihood of subscribing. The final result should be able to inform a new paywall strategy for this blog.

**Notes: 
Each row in `propensity_data.csv` represents a single page view.
Conversion rates on specific days or times can be highly correlated for all visitors due the content being published.
**

## Data 

| Column Name     | Description       |
| --------------- | ----------------- |
| pageID | unique ID for each article a user views
| paywall | whether the article was locked or open
| time | date and time of user's visit
| daysSinceFirstSeen | number of days since first article visit
| section | section of the article read on visit
| visitNum | visit count of the article read
| pageNum | page count of the article read
| registered | binary of user's logged in status (registration is free and not a subscription)
| edu | binary of whether a user is a college student or not
| mobile | binary of whether a user is on a mobile phone
| mac | binary of whether a user is on an Apple device
| converted | binary of whether user subscribed after page view


## Questions

  1. What is the base rate of conversion for locked versus open pages?
  
  2. How many article views does the blog currently have locked?
  
  3. Choose 3 variables and show how does conversion rate differs by each one. Which is the strongest indicator of a conversion?
  
  5. Build a model to score a user's likelihood of subscribing.
  
        a. Why did you choose this particular model algorithm?
        
        b. Show the importance of the variables that you chose to include in the model.
        
        c. Show the strength of the model.
        
        d. Graph the distribution of likelihood of subscribing scores.
        
  6. What paywall decision would you make based off these findings?
