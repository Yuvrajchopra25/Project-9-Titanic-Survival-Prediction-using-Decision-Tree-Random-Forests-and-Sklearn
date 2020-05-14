# Titanic Survival Prediction using Decision Tree, Random Forests and Sklearn

![Titanic](titanic.gif)

## Introduction:
The Titanic Survival Prediction project was fun to build as we will be predicting whether someone would have survived if they were in the titanic ship or not. For this beginner’s project, we will use the Titanic dataset that contains real data of the survivors and people who died in the Titanic ship.

### RMS Titanic
The RMS Titanic was a British passenger liner that sank in the North Atlantic Ocean in the early morning hours of 15 April 1912, after it collided with an iceberg during its maiden voyage from Southampton to New York City. There were an estimated 2,224 passengers and crew aboard the ship, and more than 1,500 died, making it one of the deadliest commercial peacetime maritime disasters in modern history. The RMS Titanic was the largest ship afloat at the time it entered service and was the second of three Olympic-class ocean liners operated by the White Star Line. The Titanic was built by the Harland and Wolff shipyard in Belfast. Thomas Andrews, her architect, died in the disaster.

![Titanic](https://miro.medium.com/max/1024/0*KfHijq1bO1nDV5Dl.jpg)
 
 ## Problem Statement:
This will be a fun project to build as we will be predicting whether someone would have survived if they were in the titanic ship or not.

## Requirements:
- Jupyter Notebook

## Titanic Dataset:
The titanic data frames describe the survival status of individual passengers on the Titanic. The titanic data frame does not contain information from the crew, but it does contain actual ages of half of the passengers. The principal source for data about Titanic passengers is the Encyclopedia Titanica.

The training-set has 891 examples and 11 features + the target variable (survived). 2 of the features are floats, 5 are integers and 5 are objects.

## Importing the Modules:
- SkLearn
- Numpy
- Pandas
- Matplotlib
- Pydotplus

## Decision Trees:
- Simple Tree like structure, model makes a decision at every node
- Useful in simple tasks
- One of the most popular algorithm
- Easy explainability, easy to show how a decision process works!

### Why decision trees are popular?
   - Easy to interpret and present
   - Well defined Logic, mimic human level thought
   - Random Forests, Ensembles of decision trees are more powerful classifiers
   - Feature values are preferred to be **categorical**. If the values are continuous then they are discretized prior to building the model.

### Build Decision Trees
Two common algorithms - 
- CART (Classification and Regression Trees) → uses Gini Index(Classification) as metric.
- ID3 (Iterative Dichotomiser 3) → uses Entropy function and Information gain as metrics.

![](https://www.researchgate.net/profile/Joop_Hox/publication/317307818/figure/fig2/AS:633029202571264@1527937331016/Decision-tree-on-Titanic-survival-data-Source-https-en.png)

## Score:
For this model, the accuracy on the test set is **0.817**, which means the model made the right prediction for **81.7%** of the passengers in the given dataset. We can expect the model to be correct **81.7%** of the time for predicting whether someone would have survived if they were in the titanic ship or not.

## Random Forest:
Random Forest is a supervised learning algorithm. Like you can already see from it’s name, it creates a forest and makes it somehow random. The „forest“ it builds, is an ensemble of Decision Trees, most of the time trained with the “bagging” method. The general idea of the bagging method is that a combination of learning models increases the overall result.

To say it in simple words: Random forest builds multiple decision trees and merges them together to get a more accurate and stable prediction.

One big advantage of random forest is, that it can be used for both classification and regression problems, which form the majority of current machine learning systems. With a few exceptions a random-forest classifier has all the hyperparameters of a decision-tree classifier and also all the hyperparameters of a bagging classifier, to control the ensemble itself.

The random-forest algorithm brings extra randomness into the model, when it is growing the trees. Instead of searching for the best feature while splitting a node, it searches for the best feature among a random subset of features. This process creates a wide diversity, which generally results in a better model. Therefore when you are growing a tree in random forest, only a random subset of the features is considered for splitting a node. You can even make trees more random, by using random thresholds on top of it, for each feature rather than searching for the best possible thresholds (like a normal decision tree does).

Below you can see how a random forest would look like with two trees:

![](https://miro.medium.com/max/1400/1*GiCvHwZ03tObjkD-6mSqag.png)

## Score:
For this model, the accuracy on the test set is **0.820**, which means the model made the right prediction for **82%** of the passengers in the given dataset. We can expect the model to be correct **82%** of the time for predicting whether someone would have survived if they were in the titanic ship or not.

## Summary:
We started with the data exploration where we got a feeling for the dataset, checked about missing data and learned which features are important. During the data preprocessing part, we computed missing values, converted features into numeric ones, grouped values into categories and created a few new features. Afterwards we started training 2 different machine learning models, picked one of them (Decision tree) and applied cross validation on it. Then we discussed how random forest works, took a look at the importance it assigns to the different features. Lastly, we looked at score and computed the models accuracy.

![](https://www.kdnuggets.com/wp-content/uploads/socialcops-tree.jpg)
