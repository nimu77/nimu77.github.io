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

After you instatiate the class, feed in the training set to the **fit** method of class **Knn**, this is how it does its learning. When **predict** method is called for the test set, it does its learning by looking at similar points that are closest to the point of interest to determine the class of unlabeled set.

This class model is highly useful for classification task. It is a simple algorithm that classifies based on distance, and similarity occurences. The *k* is odd because it will produce a prediction of either *yes* or *no* for binary classification, that does not mean this cannot be used in multi-class classification. Generally, data scientist prefer odd number for *k*. 

You can write regular [markdown](http://markdowntutorial.com/) here and Jekyll will automatically convert it to a nice webpage.  I strongly encourage you to [take 5 minutes to learn how to write in markdown](http://markdowntutorial.com/) - it'll teach you how to transform regular text into bold/italics/headings/tables/etc.

**Here is some bold text**

## Here is a secondary heading

Here's a useless table:

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |


How about a yummy crepe?



It can also be centered!

![Crepe](https://s3-media3.fl.yelpcdn.com/bphoto/cQ1Yoa75m2yUFFbY2xwuqw/348s.jpg){: .center-block :}

Here's a code chunk:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

And here is the same code with syntax highlighting

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

And here is the same code yet again but with line numbers:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.
