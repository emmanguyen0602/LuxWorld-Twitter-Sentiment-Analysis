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

## Problem Statement

Are you wondering how people are feeling about your brand on Twitter? By monitoring the sentiment of tweets in real time, you can gain insights into what people think and feel about your brand, product, or service through __different tweets__ and __comments__. This guarantees that the companies understand the behavior of the customers and make changes based on the __sentiment__ and therefore bring __benefits__ to the companies. 

## Objectives
<li> To extract information from tweets (between October and December, 2022) related to Luxworld, travel-to-earn, move-to-earn and see it is either positive or negative, or neutral. </li> 
<li> To explore conversations and topics that occur most in the collected tweets. </li> 
<li> To visualize the trends in sentiments of Twitter users. </li> 

## Tools

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

## DATA-PREPROCESSING

<b> Data Cleaning </b> 

<li> Removed Twitter Handles (@user) using library re </li>
<li> Removed punctuation and stopwords using string.punctuation and nltk </li> 
<li> Lemmatization of Tweets using nltk.WordNetLemmatizer() </li> <br> 

## Data Modeling


