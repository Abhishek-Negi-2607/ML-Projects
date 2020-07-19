Predicting Who’s going to Survive on Titanic Dataset
						Name: -       Abhishek Negi
						U. Roll No.: -  2012467
						Section: -        C

PROBLEM STATEMENT:- 
 
We will use the Titanic passenger’s data (Name, Age, Price of ticket, etc.) and      try to predict who will survive and who will die.



ABSTRACT:-
The purpose of this analysis is to build a predictive model that answers the question: “What sorts of people were more likely to survive?” 
using passenger’s data (i.e. name, age, gender, socio-economic class, etc.).
In this project I have implemented a machine learning model which will predict the chances of survival of a passenger on the basis of the given attributes.
If the value of survived attribute in output file if-
•	if it's a "1", the passenger survived.
•	if it's a "0", the passenger died.
After the completion of the project I uploaded the output file on Kaggle which resulted in 76.8% accuracy.




METHODOLOGY:-  

We will use machine learning techniques to solve a binary classification problem.
Random forest classifier is the one which I felt the best one for this project.




DATASET: -

train.csv contains the details of a subset of the passengers on board (891 passengers, to be exact -- where each passenger gets a different row in the table).
test.csv does not have a "Survived" column.
(we need to predict this)



ALGORITHMS/TECHNIQUES:-

In this project, Random Forrest (RF) will be implemented and the learning algorithms will be implemented by sklearn toolbox in this project.
RANDOM FORREST:-
RF is an ensemble classifier, it fits a number of decision tree classifiers on various sub-samples of the dataset and uses averaging to improve 
the predictive accuracy and control over-fitting. sklearn provides a function called RandomForestClassifier(). 
One typical tunable parameter is called ”n estimators”, which represents the number of trees in the forest.



HOW AND WHAT I DID:-

Firstly, I learned basics of Machine learning from 2 courses namely: -
1.	Machine Learning by Andrew Ng
2.	Machine Learning (Udemy Course)
Then I started Kaggle Machine Learning course to implement things practically.
This project was part of that course which helped me a lot to complete this project with less difficulty and errors.
Pre-processing phase: -
Basically in pre-processing phase I changed column Embarked to numerical format as pre-processing in string is difficult and with 
numerical format of data it will be easy to get co-relations btw attributes.
And changed sex column to 0,1 male=0, female=1.



EDA:-

Some sort of EDA is done on the basis of survived people, their age, them on board location and ages are classified as class e.g: class1, class 2, class 3.



Model Fitting:-

Random forest model was fitted on features_forest(which is basically our training set which contain 8 attributes. 
And our training set was target which contain survived attribute.
Than we printed our model score by invoking score method. We also used model_selection library of sklearn to calculate accuracy.




RESULT:-
Than finally we fitted our model on test set and predicted the result and stored it in a file named as random_forest.csv and submitted on Kaggle. Our accuracy was 76.8.
Form the result I concluded that male chances were more to survive than woman and young people who were in class 1 were having surviving chances high.










