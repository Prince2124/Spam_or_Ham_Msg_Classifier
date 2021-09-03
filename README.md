# Spam or Ham Message Classification
The purpose of this project is to understand how we can use machine learning algorithm to build SMS spam detection model. Particularly, we will build a binary classification model to detect whether a text message is spam or not. A lot of times they ask us to fill in forms and ask our personal information or Account number details which is really fishy or bound to be a fraud. The goal of this project is to use Data Science to accurately classify whether a message is spam or not.
# Data
The dataset we used to build our model is from the UIC repostiory. The link to the dataset is https://archive.ics.uci.edu/ml/datasets/sms+spam+collection. The dataset has 2 columns, the text messages and the label. The dataset contains 5572 text messages which are appropriately labelled ham and spam. The dataset is imbalanced in nature with 4825 instances of ham class and 747 instances of spam class.
# Data cleaning and preprocessing
The data is a bunch of text messages which are personal conversations as well as spam texts. So, we pre-processed the data by by performing the following steps:
A.The messages contained phone numbers, email addresses, http links, money symbols, and other numbers which is replace by with whitespace using Implemented regular expressions.
B.Converted the messages to lowercase.
C.Implemented stemming on words to bring them to their root form.
D.The important words are the tokens other than the stop words. So, we removed the stopwords from the messages as they do not act as the differentiating factor.
E.Then, implemented CountVectorizer for the data modeling process.
# Execution of the process
In the project has a jupyter notebook spam_classification.ipynb which is used for the implementation of this project.
# Screenshort of Confusion matricx of different classifire model
## A.Decision Tree Classifier
![Using_DecisionTreeClassifier](https://user-images.githubusercontent.com/59818604/132064774-63e05355-9bc8-4edc-9a83-fd93254ac768.png)
## B.Naive Bayes Classifier
![Using_NaiveBayesClassifier](https://user-images.githubusercontent.com/59818604/132064780-0149a202-a27e-46bb-9364-d8a7ec1733ed.png)
## C.SVM_Classifier
![Using_SVM_Classifier](https://user-images.githubusercontent.com/59818604/132064786-1d24b0eb-5c3a-43d0-8dd2-7e307723f2b2.png)

# Results
The results of the CountVectorizer data:
A.Using Naive bayes classifier Model>>>>>>>>>>>>>>>>Accuracy:98.5
B.Using Decision Tree Classifier(Entropy)>>>>>>>>>>>>>>>>Accuracy:98.1
C.Using SVM with linear Model>>>>>>>>>>>>>>>>Accuracy:98.5
# Reference
https://github.com/krishnaik06/SpamClassifier
