# Credit Risk Analysis
![enter image description here](https://github.com/singhsmita/Credit_Risk_Analysis/blob/main/Results/images.jpg)

## Overview
The goal of this project is to develop and evaluate multiple supervised machine learning models to predict credit risk, and determine which model performs the best. The dataset used in this project has a class imbalance issue, with a larger number of low-risk loans compared to high-risk loans.
  
##  Purpose

To resolve this issue, the project team adopted various techniques such as oversampling the data using RandomOverSampler and SMOTE algorithms, undersampling the data using the ClusterCentroids algorithm, and using a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.

  

The team compared the performance of two machine learning models, BalancedRandomForestClassifier and EasyEnsembleClassifier, which reduce bias. The performance of these models was evaluated, and the team will make a recommendation on whether they should be used to predict credit risk.

  

Python was used to build and evaluate the machine learning models. The project aimed to identify the best model for predicting credit risk and contribute to the development of more accurate and reliable credit risk prediction systems.


## Results
### Random Oversampling
![enter image description here](https://github.com/singhsmita/Credit_Risk_Analysis/blob/main/Results/random_oversampling.png)
The result for this analysis are as follows:-
-   **Balanced accuracy score:**0.624
-   **Precision:**  0.01
-   **Recall:**  0.60
Now, the balanced accuracy score is high to about 62%.

The high_risk precision is still low at 1% only with 60% sensitivity which makes a F1 of only 2%.


### SMOTE Oversampling
![enter image description here](https://github.com/singhsmita/Credit_Risk_Analysis/blob/main/Results/smote_oversampling.png)
The result for this analysis are as follows:-
-   **Balanced accuracy score:**  0.651
-   **Precision:**  0.01
-   **Recall:**  0.64

Now, the balanced accuracy score is high to about 65%.

The high_risk precision is still low at 1 % only with 64 % sensitivity which makes a F1 of only 2%.


### Cluster Centroids Undersampling
![enter image description here](https://github.com/singhsmita/Credit_Risk_Analysis/blob/main/Results/cluster_centroids.png)
The result for this analysis are as follows:-
-   **Balanced accuracy score:**  0.651
-   **Precision:**  0.01
-   **Recall:**  0.64
Here the balanced accuracy score is down to about 65%.

The high_risk precision is still 1% only with 64% sensitivity which makes a F1 of 2%.




### SMOTEEENN Combination Sampling
![enter image description here](https://github.com/singhsmita/Credit_Risk_Analysis/blob/main/Results/Combination_Sampling.png)
The result for this analysis are as follows:-
-   **Balanced accuracy score:**  0.651
-   **Precision:**  0.01
-   **Recall:**  0.72
- Now, the balanced accuracy score is high to about 65%.

The high_risk precision is still low at 1% only with 72% sensitivity which makes a F1 of only 2%.


### Balanced Random Forest Classifier
![enter image description here](https://github.com/singhsmita/Credit_Risk_Analysis/blob/main/Results/Balanced_Random_Forest_Classifier.png)
The result for this analysis are as follows:-
-   **Balanced accuracy score:**  0.788
-   **Precision:**  0.03
-   **Recall:**  0.70
- 
Here the balanced accuracy score is down to about 78%.

The high_risk precision is still 3% only with 70% sensitivity which makes a F1 of 6%.





### Easy Ensemble AdaBoost Classifier
![enter image description here](https://github.com/singhsmita/Credit_Risk_Analysis/blob/main/Results/Easy_Ensemble_AdaBoost_Classifier.png)
The result for this analysis are as follows:-
-   **Balanced accuracy score:**  0.932
-   **Precision:**  0.09
-   **Recall:**  0.92
Now, the balanced accuracy score is high to about 93%.

The high_risk precision is still low at 9% only with 92% sensitivity which makes a F1 of only 16%.



## Summary
The credit risk analysis project used multiple machine learning models to predict credit risk. However, the precision of all models in determining high-risk credits was found to be weak.

  

The Ensemble models, including the BalancedRandomForestClassifier and EasyEnsembleClassifier, showed improvement in detecting high-risk credits, with the EasyEnsembleClassifier model having a high recall of 92%. However, the low precision score of these models resulted in many low-risk credits being falsely detected as high risk. This would negatively impact the bank's credit strategy and revenue by missing out on potential business opportunities. Therefore, it is not recommended for the bank to use any of these models to predict credit risk.

  

Out of the six machine learning models, the model that used the AdaBoost algorithm performed the best in terms of balanced accuracy, precision, and recall. Although it had a low precision score, it had a high recall score, which is more important in this context as the bank does not want to give loans to high-risk individuals who are more likely to default. However, the bank may miss out on potential opportunities by rejecting good loans.

  

It is recommended that revisions be made to the AdaBoost model to increase its precision score without significantly decreasing its accuracy. This can be achieved by using additional features in the model or exploring other machine learning algorithms. Overall, the AdaBoost model has the potential to provide more accurate and reliable credit risk predictions for the bank
