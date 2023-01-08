# Credit_Risk_Analysis

## Overview of Project: 
Credit card risk analysis is the process of evaluating the potential risk of default on a credit card loan. In order to predict the risk of default on a credit card loan, I used statistical models and machine learning algorithms to analyze data about the borrower and the loan. These models can help to identify patterns and characteristics that are associated with a higher risk of default, and allow lenders to make informed decisions about whether to approve a loan or not. According to the target (loan_status), it is a classification problem and I used below models (Algorithms) to predict the credit risk. 

### Oversample Algorithms:

1. RandomOverSampler  
2. SMOTE

### Undersample Algorithm:

3. ClusterCentroids

### Combinatorial Algorithm:

4. SMOTEENN

### Ensemble algorithms: 

5. BalancedRandomForestClassifier
6. Easy Ensemble AdaBoost classifier

## Analysis Results:
#### Data set 

![Screenshot 2023-01-08 at 2 33 42 AM](https://user-images.githubusercontent.com/44387918/211191918-78715f96-4f59-48d5-a442-90ae61634400.png)

#### Balance of our target values:
* Low_risk   -    68470

* High_risk  -     347

![Screenshot 2023-01-08 at 2 40 16 AM](https://user-images.githubusercontent.com/44387918/211191973-a1390229-4058-4c02-8071-9df7c5b166ca.png)

### Random Over Sampler results 
* Balanced accuracy score: 0.6695203021237577
 
![Screenshot 2023-01-08 at 2 43 41 AM](https://user-images.githubusercontent.com/44387918/211192013-d8a41d8c-355c-42d2-ab2e-008bba621116.png)

* Precision and recall scores: 

![Screenshot 2023-01-08 at 2 43 52 AM](https://user-images.githubusercontent.com/44387918/211192027-2be40795-4914-477e-a6ce-fe4f6dc93ae5.png)

### SMOTE results

Balanced accuracy score: 0.6565183061804778

![Screenshot 2023-01-08 at 2 53 14 AM](https://user-images.githubusercontent.com/44387918/211192255-30936746-56b1-4c63-977b-bacb67bc7d5c.png)

Precision and recall scores: 

![Screenshot 2023-01-08 at 2 53 31 AM](https://user-images.githubusercontent.com/44387918/211192261-4e2d731d-e7a8-47b7-b104-e51cb19f1393.png)

### Cluster Centroids algorithm results

Balanced accuracy score: 0.5472771698357861

![Screenshot 2023-01-08 at 2 55 45 AM](https://user-images.githubusercontent.com/44387918/211192340-3ad65b56-2ff2-411c-9c5f-4a3226a3db9b.png)

Precision and recall scores:

![Screenshot 2023-01-08 at 2 55 50 AM](https://user-images.githubusercontent.com/44387918/211192343-5f340d78-492c-416a-93d4-6058c547812a.png)

### SMOTEENN algorithm 

Balanced accuracy score: 0.6514835855662273
 
![Screenshot 2023-01-08 at 2 59 14 AM](https://user-images.githubusercontent.com/44387918/211192433-57c11642-5257-45cb-9d66-8c3966bcf67e.png)
 
Precision and recall scores: 

![Screenshot 2023-01-08 at 2 58 25 AM](https://user-images.githubusercontent.com/44387918/211192438-03d97e2d-a70d-44ca-939e-2986b7766fbe.png)

### Balanced Random Forest Classifier
 
Balanced accuracy score: 0.7290249400290825

![Screenshot 2023-01-08 at 3 02 13 AM](https://user-images.githubusercontent.com/44387918/211192536-26d966f5-ea39-45d1-a572-78576d0e64be.png)

Precision and recall scores: 

![Screenshot 2023-01-08 at 3 02 21 AM](https://user-images.githubusercontent.com/44387918/211192540-651f5776-633e-42c4-8bc7-bf27eb6c4839.png)

### Easy Ensemble AdaBoost Classifier
 
Balanced accuracy score: 0.9316600714093861

![Screenshot 2023-01-08 at 3 03 26 AM](https://user-images.githubusercontent.com/44387918/211192609-6d845019-3861-4115-85bd-d29497390e38.png)

Precision and recall scores: 

![Screenshot 2023-01-08 at 3 03 41 AM](https://user-images.githubusercontent.com/44387918/211192617-f4eca5a4-64c9-4f66-a7fd-3cb96b2def37.png)

## Summary: 
Analyzed 6 machine learning models to predict the credit risk, using a dataset of 68817 customer records with 86 features. The models we considered included Oversample, Undersample, Combinatorial and Ensemble algorithms.

After preprocessing the data, I splitted the data into a training set (75%) and a test set (25%). Then trained each model on the training set and evaluated their performance on the test set. For evaluation, I considered balanced accuracy, precision and recall scores as the metric. 

#### The results were as follows:

RandomOverSampler: accuracy = 0.66, precision = 0.99, recall = 0.63

SMOTE:             accuracy = 0.65, precision = 0.99, recall = 0.68

ClusterCentroids:  accuracy = 0.54, precision = 0.99, recall = 0.40

SMOTEENN:          accuracy = 0.65, precision = 0.99, recall = 0.59

BalancedRandomForestClassifier:    accuracy = 0.72,  precision = 0.99, recall = 0.84

Easy Ensemble AdaBoost classifier: accuracy = 0.93,  precision = 0.99, recall = 0.94

Overall, I recommend the Easy Ensemble AdaBoost classifier. It performed the best out of the 6 models, with the highest accuracy score 0.93 along with precision and recall. The BalancedRandomForestClassifier model is next with high performance, also the F1 score above 0.9.
