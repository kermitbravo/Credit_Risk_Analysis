# Credit Risk Analysis

## Overview of the analysis

The objective of this analysis is to apply imbalanced learning techniques to predict credit card risk using machine learing. For this we will undersample, oversample and use a combinatorial approach to predict credit card risk. 

After we're done with this, we will compare different approaches and we will make a recommendation on whether they should be used or not to tackle this problem.

## Results

### Oversampling
1 Naive Random Oversampling 
  - Balanced Accuracy Score

![Balanced Accuracy Score](Resources/Images/1_Random_Oversampling_Balanced_Accuracy.png)
  - Imbalanced Classification Report 

![Imbalanced Classification Report](Resources/Images/1_Random_Oversampling.png)

2 SMOTE
  - Balanced Accuracy Score

![Balanced Accuracy Score](Resources/Images/2_SMOTE_Oversampling_Balanced_Accuracy.png)
  - Imbalanced Classification Report 

![Imbalanced Classification Report](Resources/Images/2_SMOTE_Oversampling.png)

3 Cluster Centroids
  - Balanced Accuracy Score

![Balanced Accuracy Score](Resources/Images/3_ClusterCentroids_Balanced_Accuracy.png)
  - Imbalanced Classification Report 

![Imbalanced Classification Report](Resources/Images/3_ClusterCentroids_Undersampling.png)

4 SMOTEENN
  - Balanced Accuracy Score

![Balanced Accuracy Score](Resources/Images/4_SMOTEENN_Balanced_Accuracy.png)
  - Imbalanced Classification Report

![Imbalanced Classification Report](Resources/Images/4_SMOTEENN.png)


5 Balanced Random Forest
  - Balanced Accuracy Score

![Balanced Accuracy Score](Resources/Images/5_Balanced_RandomForest_Balanced_Accuracy.png)
  - Imbalanced Classification Report 

![Imbalanced Classification Report](Resources/Images/5_Balanced_RandomForest.png)


6 EasyEnsembleClassifier
  - Balanced Accuracy Score

![Balanced Accuracy Score](Resources/Images/6_EasyEnsembleClassifier_Balance_Accuracy.png)
  - Imbalanced Classification Report

![Imbalanced Classification Report](Resources/Images/6_EasyEnsembleClassifier.png)
 
## Summary

As we can observe, the results of all of our models are quite accurate ( above 50% in balance ) but they are not very precise ( very low precision, specifically on high_risk credits ). This means that we are not flagging high risk credits appropriately and this models shouldn't be used for this specific purpose. We can also observe that our f1 scores are pretty low across the board for high_risk transactions which are very sensitive for this type of analysis, hence we would suggest looking for other alternatives to model this type of problem. 
