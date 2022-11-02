# Credit Card Risk Analysis with Supervised Machine Learning

## Overview
Machine learning models are able to process large amounts of data to arrive at a single decision. These models can specifically be applied to banks and financial institutions to help them monitor porfolios, predict credit risk, and lead to a more accurate identification of good candidates for loans, resulting in lower default rates. Jill, the lead data scientist at LendingClub, has asked me to analyze the credit card credit dataset from the LendingClub to predict credit risk. I will use six different machine learning models to predict the credit risk. The first two, RandomOverSampler and SMOTE, are algorithms used to oversample the data. The third algorithm, ClusterCentroids, is used to undersample the data. SMOTEENN is the fourth algorithm, which uses a combinatorial approach of over- and undersampling the data. The last two machine learning models, BalancedRandomForestClassifier and EasyEnsembleClassifier, will predict credit risk by reducing bias. 

### Purpose
The purpose of this analysis is to predict credit card risk with the six machine learning models. After calculating the models' balanced accuracy score and their precision and recall scores, I will recommend to Jill which model to use.

## Resources
* Data Source: LoanStats_2019Q1.csv
* Software: Jupyter Notebook 6.4.8

## Results
For each of the six machine learning models, the balanced accuracy score and the precision and recall score are listed below:
  
  ### RandomOverSampler
 ![image](https://user-images.githubusercontent.com/107401667/199387972-195a7c97-e11e-47b8-b042-5c930cdfc55d.png)
  * The balanced accuracy score is 65%.
  * The average precision score is 99%.
  * The average recall is 69%.
  
  ### SMOTE
  ![image](https://user-images.githubusercontent.com/107401667/199388177-b535ab89-8490-4947-a8f3-246a93a5c87c.png)
  * The balanced accuracy score is 62%.
  * The average precision score is 99%.
  * The average recall is 65%.
  
  ### ClusterCentroids
  ![image](https://user-images.githubusercontent.com/107401667/199388469-7b7b91e5-9b45-4086-9bdb-2d29c72dbb38.png)
  * The balanced accuracy score is 53%.
  * The average precision score is 99%.
  * The average recall is 45%.
  
  ### SMOTEENN
  ![image](https://user-images.githubusercontent.com/107401667/199388599-d108a17f-083c-444b-bf66-0cf3df287a50.png)
  * The balanced accuracy score 66%.
  * The average precision score is 99%.
  * The average recall is 59%.
  
  ### BalancedRandomForestClassifier
  ![image](https://user-images.githubusercontent.com/107401667/199388718-4d94c33d-b830-4c60-9b4f-4da647b0ee2f.png)
  * The balanced accuracy score is 79%.
  * The average precision score is 99%.
  * The average recall is 88%.
  
  ### EasyEnsembleClassifier
  ![image](https://user-images.githubusercontent.com/107401667/199388793-4e471222-88b5-4d14-b933-c6cea17112b6.png)
  * The balanced accuracy score is 92%.
  * The average precision score is 99%.
  * The average recall is 92%.

## Summary
While all six machine learning models resulted in a 99% precision score, only one machine learning model also had at least a 90% in the balanced accuracy score and average recall. This specific machine learning model is the EasyEnsembleClassifier, which supports multi-class resampling by sampling each class independently. Along with a high precision score, a high recall percentage is important because it helps measure how many people who were classified with low credit risk were correctly classified. A high accuracy score is important too because it will inform the percentage of low credit risk predictions that are correctly classified. Because EasyEnsembleClassifier has a high percentage for all three of these, I recommend this machine learning model to Jill to predict credit risk. 
