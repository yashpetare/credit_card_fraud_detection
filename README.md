# Credit_Card_Fraud_Detection
In this project I have built a machine learning model based on neural networks to classify credit card transactions as fraudulent or non fraudulent.
### Dataset :
 I have used the credit card fraud detection dataset from Kaggle for the project\
 The dataset contains transactions made by credit cards in September 2013 by European cardholders.\
 This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive 
 class (frauds) account for 0.172% of all transactions\.

 It contains only numerical input variables which are the result of a PCA transformation,in order to preserve the confidentiality of the users. Only variables which are not PCA transformed are 'Time' and 'Amount'.\
 link to dataset :https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

### Methodology Used:
  The dataset is divided into 60% Training Set and 40% Test Set\
  SMOTE is used to balance the training dataset.SMOTE hyperparameters:\
   oversampling rate=0.27\
   undersampling rate=0.5\
  The SMOTE transformed dataset is used to train a Neural Network.Neural Network architecture and hyperparameters are:\
   layer 1: units=16 activation= ReLU \
   layer 2: units=32 activation= ReLU\
   layer 3: units=1 activation= sigmoid\
   Optimizer : Adam Optimizer, rate=0.0018\
   No of Epochs: 13\
   Threshold Value for Binary Classification : 0.8
### Evaluation Metrics:
  F1 score for orignal Training Set : 0.8164\
  F1 score for Test Set             : 0.8121
