# Patient's Condition Prediction based on Drug Review

Link to the Presentation: 
https://github.com/Araf192/Drug-Review_NLP/blob/c685690c7954813c554fd587bbb607841e8f21d0/Patient's%20Condition%20Prediction%20based%20on%20Drug%20Review%20-Final.pdf

## Repository Structure
Drug-Review_NLP \
-- Capstone Project Proposal Template.pdf --> (Project Proposal) \
-- Deloitte_AI_Academy_ML_DrugReview.ipynb --> (Notebook containing all the code) \
-- Patient's Condition Prediction based on Drug Review -Final.pdf --> (Final Presentation) \
-- README.md (Read Me file containing the summary of the project and how to navigate the repository)

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
### Logistic Regression
#### This is the baseline model.
Accuracy: 94% \
Recall: 0.91 \
Precision: 0.92 \
F1-Score: 0.94 \
ROC-AUC Score: 0.99

![image](https://user-images.githubusercontent.com/115564942/230516149-ab9016aa-d969-46c8-9cef-08121ea4f577.png)

### Naive Bayes Classifier
Accuracy: 92% \
Recall: 0.88 \
Precision: 0.90 \
F1-Score: 0.89 \
ROC-AUC Score: 0.98 

![image](https://user-images.githubusercontent.com/115564942/230516179-aace6004-7185-496b-957f-3d7e819f25c2.png)

### XGBoost
Accuracy: 93% \
Recall: 0.89 \
Precision: 0.91 \
F1-Score: 0.90 \
ROC-AUC Score: 0.98

![image](https://user-images.githubusercontent.com/115564942/230516200-06ef19cb-2416-4c2a-9095-2996af064a44.png)

## Model Evaluation
For multi-class classification problem, Accuracy is the best metric. In terms of Accuracy, Logistic Regression > XGBoost > Naive Bayes Classifier
Based on the Accuracy metric, Logistic Regression is the best model to predict patient's condition based on drug review. 

## Next Steps
1. TF-IDF,  Word2vec, GloVe 
2. Few Shot Learning techniques (FastText, SetFit, etc.) 
3. Zero Shot Learning techniques
