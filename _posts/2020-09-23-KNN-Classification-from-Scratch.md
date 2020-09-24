---
layout: post
title: KNN Classification from Scratch
subtitle: Implementation of prediction model using K Nearest Neighbor methodology.
bigimg: /img/kn_n.jpg
tags: [knn, data-science, classification, machine-learning]
---

Prediction is a big part of Data Science. Today, I am going to cover a model class that imitates KNearestNeighbor Classification. This model is only for practice and for better understanding of how the algorithm works in scikit learn library for KNearestNeighbor Classification. The class **Knn** model consists of two methods **fit** and **predict**. 

So, how does this class exactly works? To get started you first need to instantiate the class **Knn**. Class **Knn** takes in one argument *k* which is optional. The default value of *k* is 3. Here, 3 acts like a perimeter of circle, and in general it classifies on the basis of comparison of instances being queried with instances from the training set based on distance to closest k *(i.e 3 in this case, which you can change to any odd number)* number of points. 

```python
# fit the knn model built from scratch to the datasets

# instantiate the class
knn_scratch = Knn(k = 3) # k value 3 by default

# fit the model to the datasets
knn_scratch.fit(X_train, y_train)

# make prediction for test data
predictions = knn_scratch.predict(X_test)

predictions
```

After you instatiate the class, feed in the training set to the **fit** method of class **Knn**, this is how it does its learning. When **predict** method is called for the test set, it does its learning by looking at similar points that are closest to the point of interest to determine the class of unlabeled set. This is where most of the work is done.

This class model is highly useful for classification task. It is a simple algorithm that classifies based on distance, and similarity occurences. The *k* is odd because it will produce a prediction of either *yes* or *no* for binary classification, that does not mean this cannot be used in multi-class classification. Generally, data scientist prefer odd number for *k*. 

For demonstration purpose, I got the dataset from [Kaggle](https://www.kaggle.com/zeeshanmulla/heart-disease-dataset) for Heart Disease. It consists of 13 attributes and a binary class target. The goal is to determine whether the patient has heart disease, 1 means patient might have heart disease and 0 means their might be no sign of heart disease.

The notebook for the demonstration is [here](https://github.com/nimu77/CS-Data-Science-Build-Week-1/blob/nirmal/build-week-algorithm/knn_scratch.ipynb){:target="_blank"}.

### Notification

{: .box-note}
**Note:** In the notebook, I have normalized the data using StandardScaler. This will normally distribute data around 0, with a standard deviation of 1.

```python
from sklearn.preprocessing import StandardScaler

pre = StandardScaler()
pre.fit(X_train)
X_train = pre.transform(X_train)
X_test = pre.transform(X_test)
```
