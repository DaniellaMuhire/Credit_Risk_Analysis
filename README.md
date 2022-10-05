# Credit_Risk_Analysis

## Project Overview

In this project, we apply machine learning to evaluate credit card risk. 

We used the following procedure:
- oversample the data using the RandomOverSampler and SMOTE algorithms, 
- undersample the data using the ClusterCentroids algorithm,
- use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm,
- Compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results

### Naive Random Oversampling
<img width="917" alt="Naive Random Oversampling" src="https://user-images.githubusercontent.com/77806210/194181064-926941e8-15f7-4367-a821-a2a8288c8a0c.png">
The balanced accuracy score for the Naive Random OverSampling model is 65%. 
- The high_risk precision is only 1% with a recall of 61%, which makes the model having a F1 of 2%. 
- The low_risk precision is of 100% with a recall of 68%. 

### SMOTE Oversampling
<img width="967" alt="SMOTE Oversampling" src="https://user-images.githubusercontent.com/77806210/194181576-c86e13fe-f98a-4a3c-a139-372240305eea.png">
The balanced accuracy score for the SMOTE OverSampling model is 62%. 
- The high_risk precision is only 1% with a recall of 61%, which makes the model having a F1 of 2%. 
- The low_risk precision is of 100% with a recall of 64%. 

### Undersampling
<img width="1035" alt="Undersampling" src="https://user-images.githubusercontent.com/77806210/194182293-73fdbd3f-d422-4557-8232-a8f4234a097d.png">
The balanced accuracy score for the Undersampling model is 52%. 
- The high_risk precision is only 1% with a recall of 60%, which makes the model having a F1 of 1%. 
- The low_risk precision is of 100% with a recall of 44%. 

### Combination (Over and Under) Sampling
<img width="1196" alt="Over and under Sampling" src="https://user-images.githubusercontent.com/77806210/194182415-c3ff228a-eecb-4ffe-a27e-de82f52d3068.png">
The balanced accuracy score for the Combination Sampling model is 64%. 
- The high_risk precision is only 1% with a recall of 70%, which makes the model having a F1 of 2%. 
- The low_risk precision is of 100% with a recall of 58%. 

### Balanced Random Forest Classifier
<img width="1012" alt="BalancedRandomForestClassifier" src="https://user-images.githubusercontent.com/77806210/194182568-465b8ae0-98d1-4585-9aa4-c9b7b057df38.png">
The balanced accuracy score for the Balanced Random Forest Classifier model is 79%. 
- The high_risk precision is only 4% with a recall of 67%, which makes the model having a F1 of 7%. 
- The low_risk precision is of 100% with a recall of 91%. 

### Easy Ensemble AdaBoost Classifier
<img width="1091" alt="EasyEnsembleAdaBoostClassifier" src="https://user-images.githubusercontent.com/77806210/194182675-3ed1fd97-8521-45e9-ae4f-550938057639.png">
The balanced accuracy score for the Easy Ensemble AdaBoost Classifier model is 93%. 
- The high_risk precision is only 7% with a recall of 91%, which makes the model having a F1 of 14%. 
- The low_risk precision is of 100% with a recall of 94%. 

## Summary
Most of the results show a weak precision in high_risk credit determination. 
The Easy Ensemble AdaBoost Classifier model is the only one with a better accuracy rate of 93% with 7% precision rate for high risk candidates.It has a recall of 91% for high_risk. The low_risk precision is of 100% with a recall of 94%.
Therefore, if a model needed to be recommended, it would be the Easy Ensemble AdaBoost Classifier model.

