<h1 align="center">Fake News Classifier</h1>

![-1x-1](https://github.com/Jacobtrombley/images-in-readme/assets/124385220/13e8b824-1bd3-47e4-9830-57cb212719d1)

Is all news real news? Can we trust all the news on social media and from various media outlets? How will we be able to detect fake news? The answer is with Python and Machine Learning!

## What is fake news?
Fake news includes pieves of news that may be false and is generally spread through social media and other onlien media sources. This technique is often used to impose certain ideas on the public and is ofte achieved with political agendas. These news itemas may contain both false and exaggerted claims which may end up being viralized by algorithms. Useres may also get caught in echo chambers of fake news on many common social media platforms. 

## Project Aim 
The aim of the project is to use the dataset containing varying news articles which are either real or fake to train a model. This model will be trained to decipher between real and fake news articles. In order to do this a [TD-IDF Vectorizer](#TFID) and Passive Agressive Classifier will be used. The models performance will be evaluated with the accuracy and a confusion matrix. 

## The Dataset 
The dataset used in this project called news.csv which comtaines news articles along with labels on if the news is FAKE or REAL. The dataset has a shape of 7796x4, the first column identifies the news, the second contains the titles, the third contains the text, and the fourth labels the news as REAL or FAKE. 

<a id="TFID"></a>
## What is a TfidfVectorizer?
- TF-IDF is an abbreviation for Term Frequency Inverse Document Frequency
- This is an algorith to transform text into a meaningful representation of numbers which is used to fit machine learning algorithm for prediction 
- TF-IDF considers the overall documents of weight of words
- TF-IDF is a measure of origionality of a word by comparing the number of times a word appears in a doc with the number of docs the word appears in
- TF-IDF = TF(t,d)xIDF(t)
  ![IMG_A2A14A03BE0C-1](https://github.com/Jacobtrombley/images-in-readme/assets/124385220/1fad8d62-4389-48c4-b0cb-fe30a7fdf00b)

- Term Frequency (TF): the number of times a word appears in a document (higher value means a term appears more often than others and therefore the document is a good match when the term is part of the search terms)
- Inverse Document Frequency (IDF): a measure of how significant a term is in the entire collection (words that occur many times in a document but also many times in others may be irrelevant)

## What is a PassiveAggressiveClassifer?
These are online learning algorithms that remains passive for a correct classification outcome and turns aggressive in the event of a miscalculation, updating, and adjusting. Unlike most other algorithms this one does not converge as its purpose is to make updates that correst the loss causing very little change in the norm of the weight vector. 


