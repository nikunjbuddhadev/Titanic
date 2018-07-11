# Titanic
The sinking of the RMS Titanic is one of the most infamous shipwrecks in history. On April 15, 1912, during her maiden voyage, the Titanic sank after colliding with an iceberg, killing 1502 out of 2224 passengers and crew. This sensational tragedy shocked the international community and led to better safety regulations for ships. In this challenge, we ask you to complete the analysis of what sorts of people were likely to survive. In particular, we ask you to apply the tools of machine learning to predict which passengers survived the tragedy.

To start with this a kaggle question (https://www.kaggle.com/c/titanic). We start by importing the dataset then by reading it and pre - processing it. We then use mice to impute missing values in the data. Then we create our base model with decision tree. We also made randomForest and glm models for this data. Then we applied stacking for improving accuracy by making a top layer model using glm. For feature engineering we apply PCA to the data and to this dimensionally reduced data and we check the accuracy and quality of these models by confusion matrix and ROC plot.

R As usual, we will first download our datasets locally, and then we will load them into data frames in both, R . Source of dataset : https://www.kaggle.com/c/titanic In R, we use read.csv to read CSV files into data.frame variables. Although the R function read.csv can work with URLs, https is a problem for R in many cases, so you need to use a package like RCurl to get around it. Libraries used : 1)library(caTools) #for sample.split . 2)library(mice) #for mice(). 3)library(rpart) #for prediction() , performance() . 4)library(rpart.plot) #for prp() .5) library(ROCR) #for ROC curve. 
