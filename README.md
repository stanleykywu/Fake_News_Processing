# Fake News Processing
Using Neural Network to process article title and determine if it is fake news

Data Source: https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset

# Pre-processing
The first step removed stop-words from each training title using nltk's stopword list. Then used keras' hashing trick to convert numpy array of strings to integer mapping component. Found most common words in data set and used these words to filter each title entry. Resized each title entry before feeding to model.

# Modeling
Used keras' sequential model with adam optimizer and sparse categorical crossentropy for loss. 
