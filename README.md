# Twitter Sentiment Analysis on LuxWorld and Travel2Earn and Move2Earn

[![](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=darkgreen)](https://www.python.org)  [![](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=TensorFlow&logoColor=white)](https://www.tensorflow.org) [![](https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/stable/) [![](https://img.shields.io/badge/SciPy-654FF0?style=for-the-badge&logo=SciPy&logoColor=white)](https://www.scipy.org) [![](https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org) [![](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)  [![](https://img.shields.io/badge/Plotly-239120?style=for-the-badge&logo=plotly&logoColor=white)](https://plotly.com) [![](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=Keras&logoColor=white)](https://keras.io) [![](https://img.shields.io/badge/conda-342B029.svg?&style=for-the-badge&logo=anaconda&logoColor=white)](https://www.anaconda.com)

![Twitter Sentiment Analysis](https://user-images.githubusercontent.com/76781033/210329609-171d0e0c-3a91-4c64-aed7-12e37f4b19cb.png)

## TABLE OF CONTENTS

* [Problem Statement](#problem-statement)
* [Objectives](#objectives)
* [Tools and Packages](#tools)
* [Data Scraping and Collection](#data-scraping-and-collection)
* [Data Pre-Processing](#data-preprocessing)
* [Data Modeling](#data-modeling)
* [Data Visualization](#data-visualization)
* [Results](#results)
* [Conclusion](#conclusion)
* [References](#references)
* [Challenges and Future Work](#challenges-and-futurework)

## PROBLEM STATEMENT

Are you wondering how people are feeling about your brand on Twitter? By monitoring the sentiment of tweets in real time, you can gain insights into what people think and feel about your brand, product, or service through __different tweets__ and __comments__. This guarantees that the companies understand the behavior of the customers and make changes based on the __sentiment__ and therefore bring __benefits__ to the companies. 

## OBJECTIVES
<li> To extract information from tweets (between October and December, 2022) related to Luxworld, travel-to-earn, move-to-earn and see it is either positive or negative, or neutral. </li> 
<li> To explore conversations and topics that occur most in the collected tweets. </li> 
<li> To visualize the trends in sentiments of Twitter users. </li> 

## TOOLS

<table style="width:100%">
  <tr>
    <th>Task</th>
    <th>Technique</th> 
    <th>Tools/Packages Used</th>
  </tr>
  <tr>
    <td>Data Scraping and Collection</td>
    <td>Tweet extraction from Twitter </td> 
    <td>snscrape</td>
  </tr>
  <tr>
    <td>Data Pre-processing</td>
    <td>Removed Twitter handles, punctuation, stopwords, lemmatization</td> 
    <td>re, nltk,pandas</td>
  </tr>
  <tr>
    <td>Text Analytics</td>
    <td>Sentiment analysis</td> 
    <td>TextBlob</td>
  </tr>
  <tr>
    <td>Data Visualization</td>
    <td>Multi-attribute plots</td> 
    <td>matplotlib, seaborn, wordcloud</td>
  </tr>
   <tr>
    <td>Data Modeling</td>
    <td>Unsupervised LDA</td> 
    <td>sklearn </td>
  </tr>
  <tr>
    <td>Environments & Platforms</td>
    <td> </td> 
    <td>Jupyter Notebook, Twitter</td>
  </tr>
</table><br>

## Data Scraping and Collection

<li> Package: snscrape</li>
<li>Language: English</li>
<li>Keywords: luxworld, Travel2Earn, Move2Earn</li>
<li>Timeframe: October 1, 2022 to September 26, 2022</li>
<li>Number of tweets collected = 14.829 tweets</li>

## DATA PREPROCESSING

<b> Data Cleaning </b> 

<li> Removed Twitter Handles (@user) using library re </li>
<li> Removed punctuation and stopwords using string.punctuation and nltk </li> 
<li> Lemmatization of Tweets using nltk.WordNetLemmatizer() </li> <br> 

## Data Modeling
<h4> Sentiment Analysis </h4>

Sentiment analysis is a supervised machine learning problem with different types of analysis. We considered a fine-grained sentiment classification with three levels of sentiments - positive, neutral, negative. We used TextBlob -  a simple library which supports complex analysis and operations on textual data. TextBlob returns polarity and subjectivity of a sentence. Polarity lies between [-1,1], -1 defines a negative sentiment and 1 defines a positive sentiment. Negation words reverse the polarity. TextBlob has semantic labels that help with fine-grained analysis. 

## DATA VISUALIZATION 
<h4> Distribution of Sentiments </h4>
<img src="https://github.com/emmanguyen0602/LuxWorld-Twitter-Sentiment-Analysis/blob/main/Images/countplot%20sensitive.png" style="width:1000px;height:500px;"> 
<hr>

<h4> Wordcloud Visualization </h4>
<img src="https://github.com/emmanguyen0602/LuxWorld-Twitter-Sentiment-Analysis/blob/main/Images/Screenshot_4.png" style="width:1000px;height:500px;"> 
<hr>
<img src="https://github.com/emmanguyen0602/LuxWorld-Twitter-Sentiment-Analysis/blob/main/Images/trend%20wordcloud.png" style="width:1000px;height:500px;"> 
<hr>

<h4> Countplot Most Occurring Words </h4>
<img src="https://github.com/emmanguyen0602/LuxWorld-Twitter-Sentiment-Analysis/blob/main/Images/top%20occuring%20words.png" style="width:1000px;height:500px;"> 
<hr> 
<img src="https://github.com/emmanguyen0602/LuxWorld-Twitter-Sentiment-Analysis/blob/main/Images/top%20occuring%20words%20neg.png" style="width:1000px;height:500px;"> 
<hr> 

<h4> Trendline of Tweets Over Time </h4>
<img src="https://github.com/emmanguyen0602/LuxWorld-Twitter-Sentiment-Analysis/blob/main/Images/trendline.png" style="width:1000px;height:500px;"> 
<hr>

## RESULTS 

* After performing __exploratory data analysis__, it could be seen that there is a comparatively more number of positive and neutral tweets compared to negative sentiments. 
* With the use of __word clouds__, it could be seen that positive words such as airdrop, presale, luck, d2e, m2e were used most frequently in LuxWorld tweets whereas some of the words used in negative tweets are game, token, time, amp, market etc.
* And for T2E and M2e bar graphs and WordClouds, besides words move to earn and crypto, NFT, app, web3, rewards, utilities etc are positive words and game, StepN, earn etc are negative words.
* October had the lowest number of tweets as compared to November and October about Luxworld's tweets. Especially, the number of positive tweets got peak on around 27-* 29/11 - the presale started and 11-13/10. The tweets in December was quite stable though not too high.


## CONCLUSION 
This study focused on analysing for positive and negative sentiments from Twitter tweets about LuxWorld, Travel to earn and Move to earn and distribution of tweet over time. 


## REFERENCES 

https://github.com/rashidesai24/Analyzing-Twitter-Trends-On-COVID-19-Vaccinations
https://github.com/emmanguyen0602/Sentiment_Analysis



## CHALLENGES AND FUTUREWORK 
<b> Challenges </b>:Tweet scraping cost large time.
<h4> Future Work </h4>
<li> Extract tweets from organization and indivisual </li>
<li> Explore the hidden topic using Unsupervided LDA </li>


