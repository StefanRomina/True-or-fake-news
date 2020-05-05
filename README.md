## Predicting fake news from a dataset

**Dataset Link : https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset#True.csv**

**Language :** Python

**Tool/Environment :** Jupyter Notebook

**Packages Used :** pandas, numpy, matplotlib, seaborn, sklearn, nltk

**Motivation:**

Fake news refers to misinformation, disinformation or mal-information which is spread through word of mouth and traditional media
and more recently through digital forms of communication such as edited videos, memes, unverified advertisements and social media
propagated rumours.
Fake news spread through social media has become a serious problem, with the potential of it resulting in mob violence, suicides etc 
as a result of misinformation circulated on social media.

Our aim is to train our model so that it can correctly predict whether a given piece of news is real or fake.

**Conclusions:**

The fake and real news data is given in two separate datasets with each dataset consisting around 20000 articles.
After cleaning and preparing the data using stopwords from nltk.corpus, CountVectorizer from sklearn, I trained and test data with train_test_split from sklean. The testing subset is used for building my model.

For testing the model using algorithms able to determine if an article is fake news or not I chose Logistic Regression and Random Forest.


The result of confusion_matrix(y_test, y_pred) tell us that:

Likely **Real** news are **5330**, Likely **Fake** News are **5857** .

Predicted **Fake** news as **Real** are **19**, predicted **Real** news as **Fake** are **19**.

I evaluated the performance of the classification models through confusion_matrix, a sklearn metrics, that shows Logistic Regression had accuracy of **0.9966**, slightly bigger than Random Forest Classifier that was **0.9608**. Both were good for prediction.
