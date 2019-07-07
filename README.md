# Practical Machine Learning Project (Coursera)

## Background

Using devices such as Jawbone Up, Nike FuelBand, and Fitbit it is now possible to collect a large amount of data about personal activity relatively inexpensively. These type of devices are part of the quantified self movement – a group of enthusiasts who take measurements about themselves regularly to improve their health, to find patterns in their behavior, or because they are tech geeks. One thing that people regularly do is quantify how much of a particular activity they do, but they rarely quantify how well they do it. 

In this project, your goal will be to use data from accelerometers on the belt, forearm, arm, and dumbell of 6 participants. They were asked to perform barbell lifts correctly and incorrectly in 5 different ways. More information is available from the website here: http://web.archive.org/web/20161224072740/http:/groupware.les.inf.puc-rio.br/har (see the section on the Weight Lifting Exercise Dataset).

The goal of your project is to predict the manner in which they did the exercise. This is the "classe" variable in the training set. You may use any of the other variables to predict with. You should create a report describing how you built your model, how you used cross validation, what you think the expected out of sample error is, and why you made the choices you did. You will also use your prediction model to predict 20 different test cases.

## Modeling strategy and results

First, I cleaned the data by removing variables with large amounts (> 85%) of missing values, either blanks or NAs. Then, I randomly split the training data into two sets: "train" and "test". The new train dataset has 70% of the cleaned training data while the new test dataset has the remaining 30%. Then, I used three different modeling methods: decision trees, randomForest, and Gradient Boosting. Whichever model has the highest accuracy in predicting the 30% of new "test" cases will be the model used to predict the 20 test cases for the final quiz. 

The results were as follows: 

1. Decision tree success rate: **~50%**
2. Random Forest success rate: **~99%**
3. Gradient Boosting Model success rate: **~96%**

To predict the final 20 cases, I used the Random Forest model. 
