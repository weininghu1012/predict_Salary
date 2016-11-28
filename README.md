---
title: "Show me how to make more than 60k a year"
author: "Weining Hu"
date: "November 27, 2016"
output: html_document
---

Everyone wish to have a decent job in the future with good salary, but what are the parameters that will actually influence our
income in the future? Is it your occupation, living area, age, or marriage status that determine your income?
In this report, I will briefly introduce my really rough steps when I participated in the [microsoft machine learning competition](https://www.facebook.com/events/142184086255896/) and try to learn from the dataset to findout what are some important factors in determining your future annual income.

### Data Exploration
Most of the data science tasks start with data exploration where we make visualizations or statistical tests to get some intuitive ideas for the dataset. Let's start with some factors that I personally think would affect the income. 

First, we could assume that as a person becomes more experienced, it's more likely that he/she would make more money in his/her career. The following graph shows the age group distributions with different response variables (morethan60kyr). As we could see from the graph, between the age group of 0-20, siginificantly more people make less than 60k a year while it's the opposite for age group of 35-55. This fact revealed from the plot agrees with my previous assumptions.

![title](/Users/weininghu/Documents/study/ubc2016w1/microsoft_predict/image/agegroup.jpeg)

So what we could get out of this image? We could see that the distribution 

![title](/Users/weininghu/Documents/study/ubc2016w1/microsoft_predict/image/career.jpeg)


###Preprocessing
In this step, I mainly apply a 'one-hot-encoding' to transform the categorical data into numeric data. Instead of apply 'ordinal mapping', which may bring extra information to the data, 'one-hot-encoding' would help preserve the original information.


### Ensemble Selection
I finally decided to apply XGboost for my model training due to its awesome performance regarding accuracy, efficiency and robustness.
The importance output gave us the key factors for gradient tree boosting when it initially made the splits. We could see from the below graph that 
![title](/Users/weininghu/Documents/study/ubc2016w1/microsoft_predict/image/importance.jpeg)


### What could we get?
