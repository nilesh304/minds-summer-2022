# MINDS Summer 2022 Programming Challenge

### Sentiment Analysis on news articles from https://www.aljazeera.com/where/mozambique/
<br />

 
## How to run the File <br/>
1. Open the file in Jupyter notebook
2. Click on Cell > Run All 

## Web Scrapping to get Articles
1. Used request library to hit the links and get the HTML response <br/>
2. Used beautifulSoup to iterate through HTML response and get required data <br/>
3. The scraped data with required fields such as title, text, image and image caption and date is saved in **articles.json**

## Preprocessing Data
### Preprocessing is done in 3 steps:
1. Converting article to lower case <br/>
2. Removing Stopwords <br/>
3. Lemmatizing Article <br/>

## Sentiment Analysis
### I have applied two different Sentiment Analysis Libraries

1. SentimentIntensityAnalyzer from VADER
2. TextBlob <br/>


## Results <br/>
### 1.   SentimentIntensityAnalyzer from VADER

![vader](https://user-images.githubusercontent.com/22401616/172280922-d80c9d29-7b49-49e9-813e-ce28b45fd3af.png)

### Conclusion
#### &nbsp; &nbsp; &nbsp; 1. 4 / 10 news articles are positive
#### &nbsp; &nbsp; &nbsp; 2. 6 / 10 news articles are negative

<br/>
<hr/>

### 2.  TextBlob
![textblob](https://user-images.githubusercontent.com/22401616/172280954-7c1e5c1e-4314-4e4c-94e1-654a2d54603a.png)

### Conclusion
#### &nbsp; &nbsp; &nbsp; 1. 6 / 10 news articles are positive
#### &nbsp; &nbsp; &nbsp; 2. 4 / 10 news articles are negative

<hr>

### Based on the results we can observe that VADER is more efficent than TextBlob

Library | Positive | Negative
-- | ---- | ----
SentimentIntensityAnalyzer | 4 | 6
TextBlob | 6 | 4

