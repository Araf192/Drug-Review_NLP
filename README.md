# Drug-Review_NLP

## Overview
This is the capstone project for AI Academy. The goal of this project is to predict patient's condition based on the drug review.
This is a multi-class text classification problem. The steps to finish this project are outlined below:
1. Business Problem
2. Data Understanding
3. Data Cleaning
4. Exploratory Data Analysis
5. Data Pre-Processing
6. Modeling
7. Evaluation
8. Next Steps

## Business Problem
If a new pharmaceutical company wants to break into the industry, they need to know which health condition's drug they need to invest in. 
They can use the review of drugs to predict the condition of patient. Once they know the condition of patient which are more popular, 
they can make decision of investing in making drugs of the most popular conditions. Drug reviews are easily accessible on the web.

## Data Understanding
Source of this Dataset: https://www.kaggle.com/datasets/jessicali9530/kuc-hackathon-winter-2018 \
This dataset contains 215063 rows and 7 columns. \
7 features are: uniqueID, drugName, condition, review, rating, date, usefulCount \
Target feature: condition

## Data Cleaning
"condition" feature has 0.5% missing values. All missing values of "condition" feature have been removed. 

## Exploratory Data Analysis
![image](https://user-images.githubusercontent.com/115564942/230515357-22b7eceb-822a-4b87-ac51-8991b1c716e3.png) \
"Birth Control" is the most common condition.

![image](https://user-images.githubusercontent.com/115564942/230515384-bf2e27e1-ad7a-463e-8488-4eb8c064f45e.png) \
Levonorgestrel is the top rated drugs with highest number of rating.

## Data Pre-processing
The top 5 conditions have been kept only for data pre-processing and modeling purpose. The "review" column has been pre-processed. Stopwords have been removed. Lemmatization have been used as well.Bag of Words Model have been created to vectorize the input features. Most of the Machine Learning models can not work with raw text, texts need to be converted into numbers to use ML models.

## Modeling
# Logistic Regression

