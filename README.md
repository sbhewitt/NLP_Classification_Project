# Project 3 - Web APIs & NLP

**Problem Statement:**

Real estate market in Ames, Iowa is becoming increasingly competitive along with the rest of the nation. Our company is looking to determine what aspects of homes in recent home sales have the greatest and least influence on a property's sale price. We want to maximize a seller’s profits while minimizing turnaround time of sale

---
### Datasets

* [`books_cleaned_data.csv`](../data/books_cleaned_data.csv): r/books Subreddit ([source](https://www.reddit.com/r/books/))
* [`fantasy_cleaned_data.csv`](../data/fantasy_cleaned_data.csv): r/Fantasy Subreddit ([source](https://www.reddit.com/r/Fantasy/))
* [`total_cleaned_data.csv`](../data/total_cleaned_data.csv): r/books & r/Fantasy Subreddits

####  Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|**subreddit**|*object*|r/books & r/Fantasy Subreddits|Subreddit|
|**selftext**|*object*|r/books & r/Fantasy Subreddits|Selftext under reddit post|
|**title**|*object*|r/books & r/Fantasy Subreddits|Title of reddit post|
|**total_text**|*object*|r/books & r/Fantasy Subreddits|Title and selftext of reddit post|



Following columns were one hot encoded:
|**Neighborhood**|*object*|Ames Housing Data|Physical locations within Ames city limits|
|**Exter Qual**|*object*|Ames Housing Data|Quality of the material on the exterior|
|**Electrical**|*object*|Ames Housing Data|Electrical system|
|**Bsmt Qual**|*object*|Ames Housing Data|Height of the basement|
|**Bsmt Cond**|*object*|Ames Housing Data|General condition of the basement|
|**Bsmt Exposure**|*object*|Ames Housing Data|Refers to walkout or garden level walls|
|**Mas Vnr Type**|*object*|Ames Housing Data|Masonry veneer type|
|**HeatingQC**|*object*|Ames Housing Data|Heating quality and condition|
|**Garage Qual**|*object*|Ames Housing Data|Garage quality|
|**Garage Cond**|*object*|Ames Housing Data|Garage condition|
|**Year Built**|*int*|Ames Housing Data|Number of fireplaces|
|**Fireplace Qu**|*object*|Ames Housing Data|Fireplace quality|
|**Kitchen Qual**|*object*|Ames Housing Data|Kitchen quality|
|**Garage Finish**|*object*|Ames Housing Data|Interior finish of the garage|
|**Garage Type**|*object*|Ames Housing Data|Garage location|
|**Paved Drive**|*object*|Ames Housing Data|Paved driveway|

---
### Models
![plot](./images/3confusion_matrix.png)
CountVectorizer, Multinomial Naive Bayes, TfidVectorizer, and Logisit Regression have been run in 

---
### Conclusion and Recommendations

Overall Quality and Square Footage have the largest influences on sale price. Miscellaneous Features (ie Elevator, 2nd Garage, Tennis Court) have a significantly lower influence on sale price

**Recommendations:** Good kitchen quality has a larger range of sale prices. May be in a seller's best interest to limit renovations on kitchen and allocate funds to other areas of the home. Exterior quality does not need to be excellent, Good and Average quality have large ranges. Average basement quality have 

---