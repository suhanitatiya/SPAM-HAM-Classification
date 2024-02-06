
# SPAM/HAM Classification using NLP


Spam/ham classification, also known/email filtering/spam filtering, is a task that involves automatically categorizing emails into two categories: "spam" (unwanted messages) and "ham" (desired messages). 
Reasons: Reduction of Email Overload, Improved User Experience.


## Install and Import Libraries
Libraries installed and imported : numpy, pandas, matplotlib, seaborn.

To install libraries 

```bash
  !pip install numpy
  !pip install pandas

```
To import libraries 
```bash
 import numpy as np
 import pandas as pd

```

## Datasets
```bash
SMSspamcollection.tsv             

```


## Steps performed
Perform them one by one

```bash
Checking Null Values
Counting the Labels
Splitting data into test and train set

```






















## CountVectorizer
It is used to transform a given text into a vector on the basis of the frequency (count) of each word that occurs in the entire text.



## Fit the data to vectorizer 
```bash
Step1]  Build vocab.
Step2]  Count number of words.

```
## TfidfVectorizer

The TfidfVectorizer will tokenize documents, learn the vocabulary and inverse document frequency weightings, and allow you to encode new documents.

```bash
  vectorizer=TfidfVectorizer()
  X_train_tfidf=vectorizer.fit_transform(X_train)
```



## LinearSVC (support vector classifier)
The objective of a Linear SVC (Support Vector Classifier) is to fit to the data you provide, returning a "best fit" hyperplane that divides, or categorizes, your data.

```bash
print(confusion_matrix(y_test, predictions))

```
output= [[1445    3]
        [  10  214]]





# Accuracy-99%

```bash
from sklearn import metrics
metrics.accuracy_score(y_test,predictions)

```
output=0.9922248803827751