# Amazon-Alexa-Review-Using-Sentiment-Analysis

This dataset consists of a nearly 3000 Amazon customer reviews (input text), star ratings, date of review, variant and feedback of various amazon Alexa products like Alexa Echo, Echo dots, Alexa Firesticks etc. for learning how to train Machine for sentiment analysis.

We try to predict the ratings given by the customers with the reviews(text data), predicting if the reviews will be able to predict the ratings for the products.

Initially the relationship is observed between each individual column by plotting plots through seaborn and matplotlib.

Data cleansing of review column (text data) is done in order to remove stop words,punctuations and not relevant characters from the text so as to take into account only valuable text data which will help us understand the insights.

After cleaning the data , the text data is tokenized and word2Vec is trained with the review words.

Recurrent Neural Network is used with 1 Dense Layer,and an LSTM layer since our data is sequential(text data). Embedding Layer is trained with the Word2vec words

The features are reviews data(tokens) and the target data is ratings , 20 epocs are run with the batch size of 1000 for training the RNN.

We run binary cross-entropy and categorical Cross Entropy and we see that the Binary Cross entropy predicts well.

This Notebook is divided into below parts:

1) Data Analysis
2) Data Cleansing
3) Word Cloud
4) Training the Word2Vec with our dictionary words
4) Data Modelling
6) Predicting the model
